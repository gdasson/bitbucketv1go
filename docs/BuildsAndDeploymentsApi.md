# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Add**](BuildsAndDeploymentsApi.md#Add) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/builds | Store a build status
[**AddAnnotations**](BuildsAndDeploymentsApi.md#AddAnnotations) | **Post** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports/{key}/annotations | Add Code Insights annotations
[**CreateOrUpdateDeployment**](BuildsAndDeploymentsApi.md#CreateOrUpdateDeployment) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/deployments | Create or update a deployment
[**CreateRequiredBuildsMergeCheck**](BuildsAndDeploymentsApi.md#CreateRequiredBuildsMergeCheck) | **Post** /required-builds/latest/projects/{projectKey}/repos/{repositorySlug}/condition | Create a required builds merge check
[**Delete**](BuildsAndDeploymentsApi.md#Delete) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/builds | Delete a specific build status
[**Delete1**](BuildsAndDeploymentsApi.md#Delete1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/deployments | Delete a deployment
[**DeleteACodeInsightsReport**](BuildsAndDeploymentsApi.md#DeleteACodeInsightsReport) | **Delete** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports/{key} | Delete a Code Insights report
[**DeleteAnnotations**](BuildsAndDeploymentsApi.md#DeleteAnnotations) | **Delete** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports/{key}/annotations | Delete Code Insights annotations
[**DeleteRequiredBuildsMergeCheck**](BuildsAndDeploymentsApi.md#DeleteRequiredBuildsMergeCheck) | **Delete** /required-builds/latest/projects/{projectKey}/repos/{repositorySlug}/condition/{id} | Delete a required builds merge check
[**Get**](BuildsAndDeploymentsApi.md#Get) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/builds | Get a specific build status
[**Get1**](BuildsAndDeploymentsApi.md#Get1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/deployments | Get a deployment
[**GetACodeInsightsReport**](BuildsAndDeploymentsApi.md#GetACodeInsightsReport) | **Get** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports/{key} | Get a Code Insights report
[**GetAnnotations**](BuildsAndDeploymentsApi.md#GetAnnotations) | **Get** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports/{key}/annotations | Get Code Insights annotations for a report
[**GetAnnotations1**](BuildsAndDeploymentsApi.md#GetAnnotations1) | **Get** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/annotations | Get Code Insights annotations for a commit
[**GetBuildStatusStats**](BuildsAndDeploymentsApi.md#GetBuildStatusStats) | **Get** /build-status/latest/commits/stats/{commitId} | Get build status statistics for commit
[**GetPageOfRequiredBuildsMergeChecks**](BuildsAndDeploymentsApi.md#GetPageOfRequiredBuildsMergeChecks) | **Get** /required-builds/latest/projects/{projectKey}/repos/{repositorySlug}/conditions | Get required builds merge checks
[**GetReports**](BuildsAndDeploymentsApi.md#GetReports) | **Get** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports | Get all Code Insights reports for a commit
[**SetACodeInsightsReport**](BuildsAndDeploymentsApi.md#SetACodeInsightsReport) | **Put** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports/{key} | Create a Code Insights report
[**SetAnnotation**](BuildsAndDeploymentsApi.md#SetAnnotation) | **Put** /insights/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/reports/{key}/annotations/{externalId} | Create or replace a Code Insights annotation
[**UpdateRequiredBuildsMergeCheck**](BuildsAndDeploymentsApi.md#UpdateRequiredBuildsMergeCheck) | **Put** /required-builds/latest/projects/{projectKey}/repos/{repositorySlug}/condition/{id} | Update a required builds merge check

# **Add**
> Add(ctx, projectKey, commitId, repositorySlug, optional)
Store a build status

Store a build status.   The authenticated user must have **REPO_READ** permission for the repository that this build status is for. The request can also be made with anonymous 2-legged OAuth.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***BuildsAndDeploymentsApiAddOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiAddOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestBuildStatusSetRequest**](RestBuildStatusSetRequest.md)| The contents of the build status request are:
These fields are **required**:


- **key**: The string referring to this branch plan/job
- **state**: The build status state, one of: &quot;SUCCESSFUL&quot;, &quot;FAILED&quot;, &quot;INPROGRESS&quot;
- **url**: URL referring to the build result page in the CI tool.


These fields are optional:


- **buildNumber** (optional): A unique identifier for this particular run of a plan&lt;
- **dateAdded** (optional): milliseconds since epoch. If not provided current date is used.
- **description** (optional): Describes the build result
- **duration** (optional): Duration of a completed build in milliseconds.
- **name** (optional): A short string that describes the build plan
- **parent** (optional): The identifier for the plan or job that ran the branch plan that produced this build status.
- **ref** (optional): The fully qualified git reference e.g. refs/heads/master.
- **testResults** (optional): A summary of the passed, failed and skipped tests.
 | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AddAnnotations**
> AddAnnotations(ctx, projectKey, commitId, repositorySlug, key, optional)
Add Code Insights annotations

Add annotations to the given report. The request should be a JSON object mapping the string \"annotations\" to an array of maps containing the annotation data, as described below. See also the example request.  A few things to note:- Annotations are an extension of a report, so a report must first exist in order to post annotations.   Annotations are posted separately from the report, and can be posted in bulk using this endpoint. - Only the annotations that are on lines changed in the unified diff will be displayed. This means it is  likely not all annotations posted will be displayed on the pull request  It also means that if the user is viewing a side-by-side diff,  commit diff or iterative review diff they will not be able to view the annotations. - A report cannot have more than 1000 annotations by default, however this property is congurable at an  instance level. If the request would result in more than the maximum number of annotations being stored  then the entire request is rejected and no new annotations are stored.  - There is no de-duplication of annotations on Bitbucket so be sure that reruns of builds will first  delete the report and annotations before creating them.  # Annotation parameters  |Parameter|Description|Required?|Restrictions|Type| |--- |--- |--- |--- |--- | |path|The path of the file on which this annotation should be placed. This is the path of the filerelative to the git repository. If no path is provided, then it will appear in the overview modalon all pull requests where the tip of the branch is the given commit, regardless of which files weremodified.|No||String| |line|The line number that the annotation should belong to. If no line number is provided, then it willdefault to 0 and in a pull request it will appear at the top of the file specified by the path field.|No|Non-negative integer|Integer| |message|The message to display to users|Yes|The maximum length accepted is 2000 characters, however the user interface may truncate this valuefor display purposes. We recommend that the message is short and succinct, with further detailsavailable to the user if needed on the page linked to by the the annotation link.|String| |severity|The severity of the annotation|Yes|One of: LOW, MEDIUM, HIGH|String| |link|An http or https URL representing the location of the annotation in the external tool|No||String| |type|The type of annotation posted|No|One of: VULNERABILITY, CODE_SMELL, BUG|String| |externalId|If the caller requires a link to get or modify this annotation, then an ID must be provided. It isnot used or required by Bitbucket, but only by the annotation creator for updating or deleting thisspecific annotation.|No|A string value shorter than 450 characters|String|

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
  **key** | **string**| The key of the report to which this annotation belongs. | 
 **optional** | ***BuildsAndDeploymentsApiAddAnnotationsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiAddAnnotationsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **body** | [**optional.Interface of RestBulkAddInsightAnnotationRequest**](RestBulkAddInsightAnnotationRequest.md)| The annotations to add. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateOrUpdateDeployment**
> RestDeployment CreateOrUpdateDeployment(ctx, projectKey, commitId, repositorySlug, optional)
Create or update a deployment

Create or update a deployment.    The authenticated user must have REPO_READ permission for the repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| the commitId that was deployed as indicated by the path | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***BuildsAndDeploymentsApiCreateOrUpdateDeploymentOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiCreateOrUpdateDeploymentOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestDeploymentSetRequest**](RestDeploymentSetRequest.md)| the details of the deployment to create, as detailed by the request body | 

### Return type

[**RestDeployment**](RestDeployment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRequiredBuildsMergeCheck**
> RestRequiredBuildCondition CreateRequiredBuildsMergeCheck(ctx, projectKey, repositorySlug, optional)
Create a required builds merge check

Create a required build merge check for the given repository.  The authenticated user must have **REPO_ADMIN** permission for the target repository to register a required build merge check.  The contents of the required build merge check request are:  These fields are **required**:  - **buildParentKeys**: A non-empty list of build parent keys that require green builds for this merge check to pass - **refMatcher.id**: The value to match refs against in the target branch - **refMatcher.type.id**: The type of ref matcher, one of: \"ANY_REF\", \"BRANCH\", \"PATTERN\", \"MODEL_CATEGORY\" or \"MODEL_BRANCH\"   These fields are optional:  - **exemptRefMatcher.id** The value to exempt refs in the source branch from this check - **exemptRefMatcher.type.id**: The type of exempt ref matcher, one of: \"ANY_REF\", \"BRANCH\", \"PATTERN\", \"MODEL_CATEGORY\" or \"MODEL_BRANCH\"   

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project that the repository belongs to | 
  **repositorySlug** | **string**| The repository being used | 
 **optional** | ***BuildsAndDeploymentsApiCreateRequiredBuildsMergeCheckOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiCreateRequiredBuildsMergeCheckOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestRequiredBuildConditionSetRequest**](RestRequiredBuildConditionSetRequest.md)| The request specifying the required build parent keys, ref matcher and exemption matcher | 

### Return type

[**RestRequiredBuildCondition**](RestRequiredBuildCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete**
> Delete(ctx, projectKey, commitId, repositorySlug, optional)
Delete a specific build status

Delete a specific build status.   The authenticated user must have **REPO_ADMIN** permission for the provided repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***BuildsAndDeploymentsApiDeleteOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiDeleteOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **key** | **optional.String**| the key of the build status | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete1**
> Delete1(ctx, projectKey, commitId, repositorySlug, optional)
Delete a deployment

Delete the deployment matching the specified Repository, key, environmentKey and deploymentSequenceNumber.   The user must have REPO_ADMIN.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| the commitId that was deployed as indicated by the path | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***BuildsAndDeploymentsApiDelete1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiDelete1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **deploymentSequenceNumber** | **optional.String**| the sequence number of the deployment, as detailed by the query parameter | 
 **key** | **optional.String**| the key of the deployment, as detailed by the query parameter | 
 **environmentKey** | **optional.String**| the key of the environment, as detailed by the query parameter | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteACodeInsightsReport**
> DeleteACodeInsightsReport(ctx, projectKey, commitId, repositorySlug, key)
Delete a Code Insights report

Delete a report for the given commit. Also deletes any annotations associated with this report.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
  **key** | **string**| The key of the report to which this annotation belongs. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAnnotations**
> DeleteAnnotations(ctx, projectKey, commitId, repositorySlug, key, optional)
Delete Code Insights annotations

Delete annotations for a given report that match the given external IDs, or all annotations if no external IDs are provided.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
  **key** | **string**| The key of the report to which this annotation belongs. | 
 **optional** | ***BuildsAndDeploymentsApiDeleteAnnotationsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiDeleteAnnotationsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **externalId** | **optional.String**| The external IDs for the annotations that are to be deleted. Can be specified more than once to delete by more than one external ID, or can be unspecified to delete all annotations. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRequiredBuildsMergeCheck**
> DeleteRequiredBuildsMergeCheck(ctx, projectKey, id, repositorySlug)
Delete a required builds merge check

Deletes a required build existing merge check, given it's ID.  The authenticated user must have **REPO_ADMIN** permission for the target repository to delete a required build merge check.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project that the repository belongs to | 
  **id** | **int64**|  | 
  **repositorySlug** | **string**| The repository being used | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Get**
> RestBuildStatus Get(ctx, projectKey, commitId, repositorySlug, optional)
Get a specific build status

Get a specific build status.   The authenticated user must have **REPO_READ** permission for the provided repository.The request can also be made with anonymous 2-legged OAuth.<br>Since 7.14

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***BuildsAndDeploymentsApiGetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiGetOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **key** | **optional.String**| the key of the build status | 

### Return type

[**RestBuildStatus**](RestBuildStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Get1**
> RestDeployment Get1(ctx, projectKey, commitId, repositorySlug, optional)
Get a deployment

Get the deployment matching the specified Repository, key, environmentKey and deploymentSequenceNumber.   The user must have REPO_READ.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| the commitId that was deployed as indicated by the query parameter | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***BuildsAndDeploymentsApiGet1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiGet1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **deploymentSequenceNumber** | **optional.String**| the sequence number of the deployment, as detailed by the query param | 
 **key** | **optional.String**| the key of the deployment, as detailed by the query parameter | 
 **environmentKey** | **optional.String**| the key of the environment, as detailed by the query parameter | 

### Return type

[**RestDeployment**](RestDeployment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetACodeInsightsReport**
> RestInsightReport GetACodeInsightsReport(ctx, projectKey, commitId, repositorySlug, key)
Get a Code Insights report

Retrieve the specified report.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
  **key** | **string**| The report key. | 

### Return type

[**RestInsightReport**](RestInsightReport.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAnnotations**
> RestInsightAnnotationsResponse GetAnnotations(ctx, projectKey, commitId, repositorySlug, key)
Get Code Insights annotations for a report

Retrieve the specified report's annotations.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
  **key** | **string**| The report key. | 

### Return type

[**RestInsightAnnotationsResponse**](RestInsightAnnotationsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAnnotations1**
> RestInsightAnnotationsResponse GetAnnotations1(ctx, projectKey, commitId, repositorySlug, optional)
Get Code Insights annotations for a commit

Get annotations for the given commit ID, filtered by any query parameters given.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***BuildsAndDeploymentsApiGetAnnotations1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiGetAnnotations1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **severity** | **optional.String**| Return only annotations that have one of the given severities. Can be specified more than once to filter by more than one severity. Valid severities are &lt;code&gt;LOW&lt;/code&gt;, &lt;code&gt;MEDIUM&lt;/code&gt; and &lt;code&gt;HIGH&lt;/code&gt;. | 
 **path** | **optional.String**| Return only annotations that appear on one of the provided paths. Can be specified more than once to filter by more than one path. | 
 **externalId** | **optional.String**| Return only annotations that have one of the provided external IDs. Can be specified more than once to filter by more than one external ID. | 
 **type_** | **optional.String**| Return only annotations that have one of the given types. Can be specified more than once to filter by multiple types. Valid types are &lt;code&gt;BUG&lt;/code&gt;, &lt;code&gt;CODE_SMELL&lt;/code&gt;, and &lt;code&gt;VULNERABILITY&lt;/code&gt;. | 
 **key** | **optional.String**| Return only annotations that belong to one of the provided report keys. Can be specified more than once to filter by more than one report | 

### Return type

[**RestInsightAnnotationsResponse**](RestInsightAnnotationsResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetBuildStatusStats**
> RestBuildStats GetBuildStatusStats(ctx, commitId, optional)
Get build status statistics for commit

Gets statistics regarding the builds associated with a commit

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **commitId** | **string**| full SHA1 of the commit | 
 **optional** | ***BuildsAndDeploymentsApiGetBuildStatusStatsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiGetBuildStatusStatsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **includeUnique** | **optional.Bool**| include a unique build result if there is either only one failed build, only one in-progress build or only one successful build | 

### Return type

[**RestBuildStats**](RestBuildStats.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPageOfRequiredBuildsMergeChecks**
> InlineResponse2002 GetPageOfRequiredBuildsMergeChecks(ctx, projectKey, repositorySlug, optional)
Get required builds merge checks

Returns a page of required build merge checks that have been configured for this repository.  The authenticated user must have **REPO_READ** permission for the target repository to request a page of required build merge checks.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project that the repository belongs to | 
  **repositorySlug** | **string**| The repository being used | 
 **optional** | ***BuildsAndDeploymentsApiGetPageOfRequiredBuildsMergeChecksOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiGetPageOfRequiredBuildsMergeChecksOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2002**](inline_response_200_2.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetReports**
> InlineResponse2004 GetReports(ctx, projectKey, commitId, repositorySlug, optional)
Get all Code Insights reports for a commit

Retrieve all reports for the given commit.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***BuildsAndDeploymentsApiGetReportsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiGetReportsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2004**](inline_response_200_4.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetACodeInsightsReport**
> RestInsightReport SetACodeInsightsReport(ctx, projectKey, commitId, repositorySlug, key, optional)
Create a Code Insights report

Create a new insight report, or replace the existing one if a report already exists for the given repository, commit, and report key. A request to replace an existing report will be rejected if the authenticated user was not the creator of the specified report.  The report key should be a unique string chosen by the reporter and should be unique enough not to potentially clash with report keys from other reporters. We recommend using reverse DNS namespacing or a similar standard to ensure that collision is avoided.<h1>Report parameters</h1><table summary=\"Report parameters\">    <tr>        <th>Parameter</th>        <th>Description</th>        <th>Required?</th>        <th>Restrictions</th>        <th>Type</th>    </tr>    <tr>        <td>title</td>        <td>A short string representing the name of the report</td>        <td>Yes</td>        <td>Max length: 450 characters (but we recommend that it is shorter so that the display is nicer)</td>        <td>String</td>    </tr>    <tr>        <td>details</td>        <td>             A string to describe the purpose of the report. This string may contain             escaped newlines and if it does it will display the content accordingly.        </td>        <td>No</td>        <td>Max length: 2000 characters</td>        <td>String</td>    </tr>    <tr>        <td>result</td>        <td>Indicates whether the report is in a passed or failed state</td>        <td>No</td>        <td>One of: PASS, FAIL</td>        <td>String</td>    </tr>    <tr>        <td>data</td>        <td>An array of data fields (described below) to display information on the report</td>        <td>No</td>        <td>Maximum 6 data fields</td>        <td>Array</td>    </tr>    <tr>        <td>reporter</td>        <td>A string to describe the tool or company who created the report</td>        <td>No</td>        <td>Max length: 450 characters</td>        <td>String</td>    </tr>    <tr>        <td>link</td>        <td>A URL linking to the results of the report in an external tool.</td>        <td>No</td>        <td>Must be a valid http or https URL</td>        <td>String</td>    </tr>    <tr>        <td>logoUrl</td>        <td>A URL to the report logo. If none is provided, the default insights logo will be used.</td>        <td>No</td>        <td>Must be a valid http or https URL</td>        <td>String</td>    </tr></table><h1>Data parameters</h1>The data field on the report is an array with at most 6 data fields (JSON maps) containing information that is to be displayed on the report (see the request example).<table summary=\"Data parameters\">    <tr>        <th>Parameter</th>        <th>Description</th>        <th>Type</th>    </tr>    <tr>        <td>title</td>        <td>A string describing what this data field represents</td>        <td>String</td>    </tr>    <tr>        <td>type</td>        <td>             The type of data contained in the value field. If not provided,             then the value will be detected as a boolean, number or string.             One of: BOOLEAN, DATE, DURATION, LINK, NUMBER, PERCENTAGE, TEXT        </td>        <td>String</td>    </tr>    <tr>        <td>value</td>        <td>            A value based on the type provided. Either a raw value             (string, number or boolean) or a map. See below.        </td>    </tr></table><table summary=\"Types\">    <tr>        <th>Type Field</th>        <th>Value Field Type</th>        <th>Value Field Display</th>    </tr>    <tr>        <td>None/Omitted</td>        <td>Number, String or Boolean (not an array or object)</td>        <td>Plain text</td>    </tr>    <tr>        <td>BOOLEAN</td>        <td>Boolean</td>        <td>The value will be read as a JSON boolean and displayed as 'Yes' or 'No'.</td>    </tr>    <tr>        <td>DATE</td>        <td>Number</td>        <td>             The value will be read as a JSON number in the form of a Unix timestamp              (milliseconds) and will be displayed as a relative date if the date is less             than one week ago, otherwise it will be displayed as an absolute date.        </td>    </tr>    <tr>        <td>DURATION</td>        <td>Number</td>        <td>             The value will be read as a JSON number in milliseconds and             will be displayed in a human readable duration format.        </td>    </tr>    <tr>        <td>LINK</td>        <td>Object: {\"linktext\": \"Link text here\", \"href\": \"https://link.to.annotation/in/external/tool\"}</td>        <td>             The value will be read as a JSON object containing the fields \"linktext\"             and \"href\" and will be displayed as a clickable link on the report.        </td>    </tr>    <tr>        <td>NUMBER</td>        <td>Number</td>        <td>             The value will be read as a JSON number and large numbers will             be displayed in a human readable format (e.g. 14.3k).        </td>    </tr>    <tr>        <td>PERCENTAGE</td>        <td>Number (between 0 and 100)</td>        <td>             The value will be read as a JSON number between 0 and 100              and will be displayed with a percentage sign.        </td>    </tr>    <tr>        <td>TEXT</td>        <td>String</td>        <td>The value will be read as a JSON string and will be displayed as-is</td>    </tr></table>

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
  **key** | **string**| A unique string representing the report as chosen by the reporter. This should be unique enough to not clash with other report&#x27;s keys. To do this, we recommend namespacing the key using reverse DNS | 
 **optional** | ***BuildsAndDeploymentsApiSetACodeInsightsReportOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiSetACodeInsightsReportOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **body** | [**optional.Interface of RestSetInsightReportRequest**](RestSetInsightReportRequest.md)| The request object containing the details of the report to create (see example). | 

### Return type

[**RestInsightReport**](RestInsightReport.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetAnnotation**
> SetAnnotation(ctx, projectKey, externalId, commitId, repositorySlug, key, optional)
Create or replace a Code Insights annotation

Create an annotation with the given external ID, or replace it if it already exists. A request to replace an existing annotation will be rejected if the authenticated user was not the creator of the specified report.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **externalId** | **string**| The external ID of the annotation that is to be updated or created | 
  **commitId** | **string**| The commit ID on which to record the annotation. This must be a full 40 character commit hash. | 
  **repositorySlug** | **string**| The repository slug. | 
  **key** | **string**| The key of the report to which this annotation belongs | 
 **optional** | ***BuildsAndDeploymentsApiSetAnnotationOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiSetAnnotationOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------





 **body** | [**optional.Interface of RestSingleAddInsightAnnotationRequest**](RestSingleAddInsightAnnotationRequest.md)| The new annotation that is to replace the existing one. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateRequiredBuildsMergeCheck**
> RestRequiredBuildCondition UpdateRequiredBuildsMergeCheck(ctx, projectKey, id, repositorySlug, optional)
Update a required builds merge check

Update the required builds merge check for the given ID.  The authenticated user must have **REPO_ADMIN** permission for the target repository to update a required build merge check.  The contents of the required build merge check request are:  These fields are **required**:  - **buildParentKeys**: A non-empty list of build parent keys that require green builds for this merge check to pass - **refMatcher.id**: The value to match refs against in the target branch - **refMatcher.type.id**: The type of ref matcher, one of: \"ANY_REF\", \"BRANCH\", \"PATTERN\", \"MODEL_CATEGORY\" or \"MODEL_BRANCH\"   These fields are optional:  - **exemptRefMatcher.id** The value to exempt refs in the source branch from this check - **exemptRefMatcher.type.id**: The type of exempt ref matcher, one of: \"ANY_REF\", \"BRANCH\", \"PATTERN\", \"MODEL_CATEGORY\" or \"MODEL_BRANCH\"   

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project that the repository belongs to | 
  **id** | **int64**|  | 
  **repositorySlug** | **string**| The repository being used | 
 **optional** | ***BuildsAndDeploymentsApiUpdateRequiredBuildsMergeCheckOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a BuildsAndDeploymentsApiUpdateRequiredBuildsMergeCheckOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestRequiredBuildConditionSetRequest**](RestRequiredBuildConditionSetRequest.md)| The request specifying the required build parent keys, ref matcher and exemption matcher | 

### Return type

[**RestRequiredBuildCondition**](RestRequiredBuildCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

