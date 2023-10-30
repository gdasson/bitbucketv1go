# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Create3**](ProjectApi.md#Create3) | **Post** /api/latest/projects/{projectKey}/settings-restriction | Enforce project restriction
[**CreateProject**](ProjectApi.md#CreateProject) | **Post** /api/latest/projects | Create a new project
[**CreateRepository**](ProjectApi.md#CreateRepository) | **Post** /api/latest/projects/{projectKey}/repos | Create repository
[**CreateRestrictions**](ProjectApi.md#CreateRestrictions) | **Post** /branch-permissions/latest/projects/{projectKey}/restrictions | Create multiple ref restrictions
[**CreateWebhook**](ProjectApi.md#CreateWebhook) | **Post** /api/latest/projects/{projectKey}/webhooks | Create webhook
[**Delete7**](ProjectApi.md#Delete7) | **Delete** /api/latest/projects/{projectKey}/settings-restriction | Stop enforcing project restriction
[**DeleteAutoDeclineSettings**](ProjectApi.md#DeleteAutoDeclineSettings) | **Delete** /api/latest/projects/{projectKey}/settings/auto-decline | Delete auto decline settings
[**DeleteProject**](ProjectApi.md#DeleteProject) | **Delete** /api/latest/projects/{projectKey} | Delete project
[**DeleteRepository**](ProjectApi.md#DeleteRepository) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug} | Delete repository
[**DeleteRestriction**](ProjectApi.md#DeleteRestriction) | **Delete** /branch-permissions/latest/projects/{projectKey}/restrictions/{id} | Delete a ref restriction
[**DeleteWebhook**](ProjectApi.md#DeleteWebhook) | **Delete** /api/latest/projects/{projectKey}/webhooks/{webhookId} | Delete webhook
[**DisableHook**](ProjectApi.md#DisableHook) | **Delete** /api/latest/projects/{projectKey}/settings/hooks/{hookKey}/enabled | Disable repository hook
[**EnableHook**](ProjectApi.md#EnableHook) | **Put** /api/latest/projects/{projectKey}/settings/hooks/{hookKey}/enabled | Enable repository hook
[**FindWebhooks**](ProjectApi.md#FindWebhooks) | **Get** /api/latest/projects/{projectKey}/webhooks | Find webhooks
[**ForkRepository**](ProjectApi.md#ForkRepository) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug} | Fork repository
[**Get5**](ProjectApi.md#Get5) | **Get** /api/latest/projects/{projectKey}/settings-restriction | Get enforcing project setting
[**GetAll**](ProjectApi.md#GetAll) | **Get** /api/latest/projects/{projectKey}/settings-restriction/all | Get all enforcing project settings
[**GetAutoDeclineSettings**](ProjectApi.md#GetAutoDeclineSettings) | **Get** /api/latest/projects/{projectKey}/settings/auto-decline | Get auto decline settings
[**GetAvatar**](ProjectApi.md#GetAvatar) | **Get** /api/latest/hooks/{hookKey}/avatar | Get project avatar
[**GetConfigurations**](ProjectApi.md#GetConfigurations) | **Get** /api/latest/projects/{projectKey}/hook-scripts | Get configured hook scripts
[**GetDefaultBranch2**](ProjectApi.md#GetDefaultBranch2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/default-branch | Get repository default branch
[**GetForkedRepositories**](ProjectApi.md#GetForkedRepositories) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/forks | Get repository forks
[**GetGroupsWithAnyPermission1**](ProjectApi.md#GetGroupsWithAnyPermission1) | **Get** /api/latest/projects/{projectKey}/permissions/groups | Get groups with permission to project
[**GetGroupsWithoutAnyPermission1**](ProjectApi.md#GetGroupsWithoutAnyPermission1) | **Get** /api/latest/projects/{projectKey}/permissions/groups/none | Get groups without project permission
[**GetLatestInvocation**](ProjectApi.md#GetLatestInvocation) | **Get** /api/latest/projects/{projectKey}/webhooks/{webhookId}/latest | Get last webhook invocation details
[**GetProject**](ProjectApi.md#GetProject) | **Get** /api/latest/projects/{projectKey} | Get a project
[**GetProjectAvatar**](ProjectApi.md#GetProjectAvatar) | **Get** /api/latest/projects/{projectKey}/avatar.png | Get avatar for project
[**GetProjects**](ProjectApi.md#GetProjects) | **Get** /api/latest/projects | Get projects
[**GetPullRequestSettings**](ProjectApi.md#GetPullRequestSettings) | **Get** /api/latest/projects/{projectKey}/settings/pull-requests/{scmId} | Get merge strategy
[**GetRelatedRepositories**](ProjectApi.md#GetRelatedRepositories) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/related | Get related repository
[**GetRepositories**](ProjectApi.md#GetRepositories) | **Get** /api/latest/projects/{projectKey}/repos | Get repositories for project
[**GetRepository**](ProjectApi.md#GetRepository) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug} | Get repository
[**GetRepositoryHook**](ProjectApi.md#GetRepositoryHook) | **Get** /api/latest/projects/{projectKey}/settings/hooks/{hookKey} | Get a repository hook
[**GetRepositoryHooks**](ProjectApi.md#GetRepositoryHooks) | **Get** /api/latest/projects/{projectKey}/settings/hooks | Get repository hooks
[**GetRestriction**](ProjectApi.md#GetRestriction) | **Get** /branch-permissions/latest/projects/{projectKey}/restrictions/{id} | Get a ref restriction
[**GetRestrictions**](ProjectApi.md#GetRestrictions) | **Get** /branch-permissions/latest/projects/{projectKey}/restrictions | Search for ref restrictions
[**GetSettings**](ProjectApi.md#GetSettings) | **Get** /api/latest/projects/{projectKey}/settings/hooks/{hookKey}/settings | Get repository hook settings
[**GetUsersWithAnyPermission1**](ProjectApi.md#GetUsersWithAnyPermission1) | **Get** /api/latest/projects/{projectKey}/permissions/users | Get users with permission to project
[**GetUsersWithoutPermission**](ProjectApi.md#GetUsersWithoutPermission) | **Get** /api/latest/projects/{projectKey}/permissions/users/none | Get users without project permission
[**GetWebhook**](ProjectApi.md#GetWebhook) | **Get** /api/latest/projects/{projectKey}/webhooks/{webhookId} | Get webhook
[**HasAllUserPermission**](ProjectApi.md#HasAllUserPermission) | **Get** /api/latest/projects/{projectKey}/permissions/{permission}/all | Check default project permission
[**ModifyAllUserPermission**](ProjectApi.md#ModifyAllUserPermission) | **Post** /api/latest/projects/{projectKey}/permissions/{permission}/all | Grant project permission
[**RemoveConfiguration**](ProjectApi.md#RemoveConfiguration) | **Delete** /api/latest/projects/{projectKey}/hook-scripts/{scriptId} | Remove a hook script
[**RetryCreateRepository**](ProjectApi.md#RetryCreateRepository) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/recreate | Retry repository creation
[**RevokePermissions**](ProjectApi.md#RevokePermissions) | **Delete** /api/latest/projects/{projectKey}/permissions | Revoke project permissions
[**RevokePermissionsForGroup1**](ProjectApi.md#RevokePermissionsForGroup1) | **Delete** /api/latest/projects/{projectKey}/permissions/groups | Revoke group project permission
[**RevokePermissionsForUser1**](ProjectApi.md#RevokePermissionsForUser1) | **Delete** /api/latest/projects/{projectKey}/permissions/users | Revoke user project permission
[**SearchPermissions**](ProjectApi.md#SearchPermissions) | **Get** /api/latest/projects/{projectKey}/permissions/search | Search project permissions
[**SetAutoDeclineSettings**](ProjectApi.md#SetAutoDeclineSettings) | **Put** /api/latest/projects/{projectKey}/settings/auto-decline | Create/Update auto decline settings
[**SetConfiguration**](ProjectApi.md#SetConfiguration) | **Put** /api/latest/projects/{projectKey}/hook-scripts/{scriptId} | Create/update a hook script
[**SetDefaultBranch2**](ProjectApi.md#SetDefaultBranch2) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/default-branch | Update default branch for repository
[**SetPermissionForGroups1**](ProjectApi.md#SetPermissionForGroups1) | **Put** /api/latest/projects/{projectKey}/permissions/groups | Update group project permission
[**SetPermissionForUsers1**](ProjectApi.md#SetPermissionForUsers1) | **Put** /api/latest/projects/{projectKey}/permissions/users | Update user project permission
[**SetSettings**](ProjectApi.md#SetSettings) | **Put** /api/latest/projects/{projectKey}/settings/hooks/{hookKey}/settings | Update repository hook settings
[**StreamContributing**](ProjectApi.md#StreamContributing) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/contributing | Get repository contributing guidelines
[**StreamLicense**](ProjectApi.md#StreamLicense) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/license | Get repository license
[**StreamReadme**](ProjectApi.md#StreamReadme) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/readme | Get repository readme
[**UpdateProject**](ProjectApi.md#UpdateProject) | **Put** /api/latest/projects/{projectKey} | Update project
[**UpdatePullRequestSettings**](ProjectApi.md#UpdatePullRequestSettings) | **Post** /api/latest/projects/{projectKey}/settings/pull-requests/{scmId} | Update merge strategy
[**UpdateRepository**](ProjectApi.md#UpdateRepository) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug} | Update repository
[**UpdateWebhook**](ProjectApi.md#UpdateWebhook) | **Put** /api/latest/projects/{projectKey}/webhooks/{webhookId} | Update webhook
[**UploadAvatar**](ProjectApi.md#UploadAvatar) | **Post** /api/latest/projects/{projectKey}/avatar.png | Update project avatar

# **Create3**
> RestProjectSettingsRestriction Create3(ctx, body, projectKey)
Enforce project restriction

Create a new project settings restriction for the given project.  The authenticated user must have **PROJECT_ADMIN** permission for the target project to create a settings restriction.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestProjectSettingsRestrictionRequest**](RestProjectSettingsRestrictionRequest.md)| The project settings restriction to create | 
  **projectKey** | **string**| The project key. | 

### Return type

[**RestProjectSettingsRestriction**](RestProjectSettingsRestriction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateProject**
> RestProject CreateProject(ctx, optional)
Create a new project

Create a new project.   To include a custom avatar for the project, the project definition should contain an additional attribute with the key <code>avatar</code> and the value a data URI containing Base64-encoded image data. The URI should be in the following format: <pre>    data:(content type, e.g. image/png);base64,(data) </pre>If the data is not Base64-encoded, or if a character set is defined in the URI, or the URI is otherwise invalid, <em>project creation will fail</em>.   The authenticated user must have <strong>PROJECT_CREATE</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***ProjectApiCreateProjectOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiCreateProjectOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestProject**](RestProject.md)| The project. | 

### Return type

[**RestProject**](RestProject.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRepository**
> RestRepository CreateRepository(ctx, projectKey, optional)
Create repository

Create a new repository. Requires an existing project in which this repository will be created. The only parameters which will be used are name and scmId.   The authenticated user must have <strong>REPO_CREATE</strong> permission or higher, for the context project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiCreateRepositoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiCreateRepositoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestRepository**](RestRepository.md)| The repository | 

### Return type

[**RestRepository**](RestRepository.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRestrictions**
> RestRefRestriction CreateRestrictions(ctx, projectKey, optional)
Create multiple ref restrictions

Allows creating multiple restrictions at once.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiCreateRestrictionsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiCreateRestrictionsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of []RestRestrictionRequest**](RestRestrictionRequest.md)| The request containing a list of the details of the restrictions to create. | 

### Return type

[**RestRefRestriction**](RestRefRestriction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/vnd.atl.bitbucket.bulk+json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateWebhook**
> RestWebhook CreateWebhook(ctx, projectKey, optional)
Create webhook

Create a webhook for the project specified via the URL.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiCreateWebhookOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiCreateWebhookOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestWebhook**](RestWebhook.md)| The webhook to be created for this project. | 

### Return type

[**RestWebhook**](RestWebhook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete7**
> Delete7(ctx, projectKey, namespace, featureKey, optional)
Stop enforcing project restriction

Delete a specified project settings restriction.  If a restriction does not exist for the specified project, namespace, featureKey, and componentKey, the request will be ignored and a 204 response will be returned.  The authenticated user must have **PROJECT_ADMIN** permission for the target project to delete a settings restriction.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **namespace** | **string**| A namespace used to identify the provider of the feature | 
  **featureKey** | **string**| A key to uniquely identify the feature within the provided namespace | 
 **optional** | ***ProjectApiDelete7Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiDelete7Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **componentKey** | **optional.String**| A key to uniquely identify individually restrictable subcomponents of a feature within the provided feature key and namespace | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAutoDeclineSettings**
> DeleteAutoDeclineSettings(ctx, projectKey)
Delete auto decline settings

Delete auto decline settings for the supplied project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for this project to call the resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteProject**
> DeleteProject(ctx, projectKey)
Delete project

Delete the project matching the supplied <strong>projectKey</strong>.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRepository**
> DeleteRepository(ctx, projectKey, repositorySlug)
Delete repository

Schedule the repository matching the supplied <strong>projectKey</strong> and <strong>repositorySlug</strong> to be deleted.   The authenticated user must have sufficient permissions specified by the repository delete policy to call this resource. The default permission required is <strong>REPO_ADMIN</strong> permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRestriction**
> DeleteRestriction(ctx, projectKey, id)
Delete a ref restriction

Deletes a restriction as specified by a restriction id.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission or higher to call this resource. Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The restriction id. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteWebhook**
> DeleteWebhook(ctx, projectKey, webhookId)
Delete webhook

Delete a webhook for the project specified via the URL.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| The ID of the webhook to be deleted. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DisableHook**
> RestRepositoryHook DisableHook(ctx, projectKey, hookKey)
Disable repository hook

Disable a repository hook for this project.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 

### Return type

[**RestRepositoryHook**](RestRepositoryHook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EnableHook**
> RestRepositoryHook EnableHook(ctx, projectKey, hookKey, optional)
Enable repository hook

Enable a repository hook for this project and optionally apply new configuration.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.   A JSON document may be provided to use as the settings for the hook. These structure and validity of the document is decided by the plugin providing the hook.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 
 **optional** | ***ProjectApiEnableHookOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiEnableHookOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentLength** | **optional.Int64**| The content length. | 

### Return type

[**RestRepositoryHook**](RestRepositoryHook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindWebhooks**
> FindWebhooks(ctx, projectKey, optional)
Find webhooks

Find webhooks in this project.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiFindWebhooksOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiFindWebhooksOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **event** | **optional.String**| List of &lt;code&gt;com.atlassian.webhooks.WebhookEvent&lt;/code&gt; IDs to filter for | 
 **statistics** | **optional.Bool**| &lt;code&gt;true&lt;/code&gt; if statistics should be provided for all found webhooks | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ForkRepository**
> RestRepository ForkRepository(ctx, projectKey, repositorySlug, optional)
Fork repository

Create a new repository forked from an existing repository.   The JSON body for this <code>POST</code> is not required to contain <i>any</i> properties. Even the name may be omitted. The following properties will be used, if provided:   - <code>\"name\":\"Fork name\"</code> - Specifies the forked repository's name    - Defaults to the name of the origin repository if not specified - <code>\"defaultBranch\":\"main\"</code> - Specifies the forked repository's default branch   - Defaults to the origin repository's default branch if not specified - <code>\"project\":{\"key\":\"TARGET_KEY\"}</code> - Specifies the forked repository's target project by key   - Defaults to the current user's personal project if not specified   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository and <strong>PROJECT_ADMIN</strong> on the target project to call this resource. Note that users <i>always</i> have <b>PROJECT_ADMIN</b> permission on their personal projects.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiForkRepositoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiForkRepositoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestRepository**](RestRepository.md)| The rest fork. | 

### Return type

[**RestRepository**](RestRepository.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Get5**
> RestProjectSettingsRestriction Get5(ctx, projectKey, namespace, featureKey, optional)
Get enforcing project setting

Get a specified project settings restriction for the given namespace, feature key and component key. Note that not providing the component key will **not** return restrictions for the namespace and feature key with a component key set.  The authenticated user must have **PROJECT_VIEW** permission for the target project to retrieve a settings restriction.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **namespace** | **string**| The namespace used to identify the provider of the feature | 
  **featureKey** | **string**| The feature key to uniquely identify the feature within the provided namespace | 
 **optional** | ***ProjectApiGet5Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGet5Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **componentKey** | **optional.String**| The component key to uniquely identify individually restrictable subcomponents of a feature within the provided feature key and namespace | 

### Return type

[**RestProjectSettingsRestriction**](RestProjectSettingsRestriction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAll**
> InlineResponse20047 GetAll(ctx, projectKey, namespace, featureKey, optional)
Get all enforcing project settings

Get all project settings restrictions for the given namespace and feature key, including those with a component key set.  The authenticated user must have **PROJECT_VIEW** permission for the target project to retrieve a settings restrictions.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **namespace** | **string**| A namespace used to identify the provider of the feature | 
  **featureKey** | **string**| A key to uniquely identify the feature within the provided namespace | 
 **optional** | ***ProjectApiGetAllOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetAllOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20047**](inline_response_200_47.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAutoDeclineSettings**
> RestAutoDeclineSettings GetAutoDeclineSettings(ctx, projectKey)
Get auto decline settings

Retrieves the auto decline settings for the supplied project. Default settings are returned if no explicit settings have been set for the project.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 

### Return type

[**RestAutoDeclineSettings**](RestAutoDeclineSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAvatar**
> GetAvatar(ctx, hookKey, optional)
Get project avatar

Retrieve the avatar for the project matching the supplied <strong>moduleKey</strong>.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **hookKey** | **string**| The complete module key of the hook module. | 
 **optional** | ***ProjectApiGetAvatarOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetAvatarOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **version** | **optional.String**| (optional) Version used for HTTP caching only - any non-blank version will result in a large max-age Cache-Control header. Note that this does not affect the Last-Modified header. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetConfigurations**
> InlineResponse20031 GetConfigurations(ctx, projectKey, optional)
Get configured hook scripts

Return a page of hook scripts configured for the specified project.   This endpoint requires **PROJECT_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiGetConfigurationsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetConfigurationsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20031**](inline_response_200_31.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetDefaultBranch2**
> RestMinimalRef GetDefaultBranch2(ctx, projectKey, repositorySlug)
Get repository default branch

Retrieves the repository's <i>configured</i> default branch.   Every repository has a <i>configured</i> default branch, but that branch may not actually <i>exist</i> in the repository. For example, a newly-created repository will have a configured default branch even though no branches have been pushed yet.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestMinimalRef**](RestMinimalRef.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetForkedRepositories**
> InlineResponse20029 GetForkedRepositories(ctx, projectKey, repositorySlug, optional)
Get repository forks

Retrieve repositories which have been forked from this one. Unlike #getRelatedRepositories(Repository, PageRequest) related repositories, this only looks at a given repository's direct forks. If those forks have themselves been the origin of more forks, such \"grandchildren\" repositories will not be retrieved.   Only repositories to which the authenticated user has <b>REPO_READ</b> permission will be included, even if other repositories have been forked from this one.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiGetForkedRepositoriesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetForkedRepositoriesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20029**](inline_response_200_29.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetGroupsWithAnyPermission1**
> InlineResponse20018 GetGroupsWithAnyPermission1(ctx, projectKey, optional)
Get groups with permission to project

Retrieve a page of groups that have been granted at least one permission for the specified project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiGetGroupsWithAnyPermission1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetGroupsWithAnyPermission1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only group names containing the supplied string will be returned | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20018**](inline_response_200_18.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetGroupsWithoutAnyPermission1**
> InlineResponse20016 GetGroupsWithoutAnyPermission1(ctx, projectKey, optional)
Get groups without project permission

Retrieve a page of groups that have no granted permissions for the specified project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiGetGroupsWithoutAnyPermission1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetGroupsWithoutAnyPermission1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only group names containing the supplied string will be returned | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20016**](inline_response_200_16.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetLatestInvocation**
> RestDetailedInvocation GetLatestInvocation(ctx, projectKey, webhookId, optional)
Get last webhook invocation details

Get the latest invocations for a specific webhook.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| ID of the webhook | 
 **optional** | ***ProjectApiGetLatestInvocationOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetLatestInvocationOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **event** | **optional.String**| The string ID of a specific event to retrieve the last invocation for. | 
 **outcome** | **optional.String**| The outcome to filter for. Can be SUCCESS, FAILURE, ERROR. None specified means that the all will be considered | 

### Return type

[**RestDetailedInvocation**](RestDetailedInvocation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetProject**
> RestProject GetProject(ctx, projectKey)
Get a project

Retrieve the project matching the supplied <strong>projectKey</strong>.   The authenticated user must have <strong>PROJECT_VIEW</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 

### Return type

[**RestProject**](RestProject.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetProjectAvatar**
> GetProjectAvatar(ctx, projectKey, optional)
Get avatar for project

Retrieve the avatar for the project matching the supplied <strong>projectKey</strong>.   The authenticated user must have <strong>PROJECT_VIEW</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiGetProjectAvatarOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetProjectAvatarOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **s** | **optional.String**| The desired size of the image. The server will return an image as close as possible to the specified size. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetProjects**
> InlineResponse20030 GetProjects(ctx, optional)
Get projects

Retrieve a page of projects.   Only projects for which the authenticated user has the <strong>PROJECT_VIEW</strong> permission will be returned.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***ProjectApiGetProjectsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetProjectsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **optional.String**| Name to filter by. | 
 **permission** | **optional.String**| Permission to filter by | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20030**](inline_response_200_30.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPullRequestSettings**
> RestPullRequestSettings GetPullRequestSettings(ctx, projectKey, scmId)
Get merge strategy

Retrieve the merge strategy configuration for this project and SCM.   The authenticated user must have <strong>PROJECT_READ</strong> permission for the context repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **scmId** | **string**| The SCM to get strategies for. | 

### Return type

[**RestPullRequestSettings**](RestPullRequestSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRelatedRepositories**
> InlineResponse20029 GetRelatedRepositories(ctx, projectKey, repositorySlug, optional)
Get related repository

Retrieve repositories which are related to this one. Related repositories are from the same Repository#getHierarchyId() hierarchy as this repository.   Only repositories to which the authenticated user has <b>REPO_READ</b> permission will be included, even if more repositories are part of this repository's hierarchy.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiGetRelatedRepositoriesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetRelatedRepositoriesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20029**](inline_response_200_29.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositories**
> InlineResponse20029 GetRepositories(ctx, projectKey, optional)
Get repositories for project

Retrieve repositories from the project corresponding to the supplied <strong>projectKey</strong>.   The authenticated user must have <strong>PROJECT_READ</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiGetRepositoriesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetRepositoriesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20029**](inline_response_200_29.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepository**
> RestRepository GetRepository(ctx, projectKey, repositorySlug)
Get repository

Retrieve the repository matching the supplied <strong>projectKey</strong> and <strong>repositorySlug</strong>.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestRepository**](RestRepository.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositoryHook**
> RestRepositoryHook GetRepositoryHook(ctx, projectKey, hookKey)
Get a repository hook

Retrieve a repository hook for this project.   The authenticated user must have <strong>PROJECT_READ</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 

### Return type

[**RestRepositoryHook**](RestRepositoryHook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositoryHooks**
> InlineResponse20044 GetRepositoryHooks(ctx, projectKey, optional)
Get repository hooks

Retrieve a page of repository hooks for this project.   The authenticated user must have <strong>PROJECT_READ</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiGetRepositoryHooksOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetRepositoryHooksOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **type_** | **optional.String**| The optional type to filter by. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20044**](inline_response_200_44.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRestriction**
> RestRefRestriction GetRestriction(ctx, projectKey, id)
Get a ref restriction

Returns a restriction as specified by a restriction id.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission or higher to call this resource. Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The restriction id. | 

### Return type

[**RestRefRestriction**](RestRefRestriction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRestrictions**
> InlineResponse20013 GetRestrictions(ctx, projectKey, optional)
Search for ref restrictions

Search for restrictions using the supplied parameters.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission or higher to call this resource. Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiGetRestrictionsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetRestrictionsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **matcherType** | **optional.String**| Matcher type to filter on | 
 **matcherId** | **optional.String**| Matcher id to filter on. Requires the matcherType parameter to be specified also. | 
 **type_** | **optional.String**| Types of restrictions to filter on. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20013**](inline_response_200_13.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSettings**
> ExampleSettings GetSettings(ctx, projectKey, hookKey)
Get repository hook settings

Retrieve the settings for a repository hook for this project.   The authenticated user must have <strong>PROJECT_READ</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 

### Return type

[**ExampleSettings**](ExampleSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUsersWithAnyPermission1**
> InlineResponse20032 GetUsersWithAnyPermission1(ctx, projectKey, optional)
Get users with permission to project

Retrieve a page of users that have been granted at least one permission for the specified project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiGetUsersWithAnyPermission1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetUsersWithAnyPermission1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only user names containing the supplied string will be returned | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20032**](inline_response_200_32.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUsersWithoutPermission**
> InlineResponse2005 GetUsersWithoutPermission(ctx, projectKey, optional)
Get users without project permission

Retrieve a page of <i>licensed</i> users that have no granted permissions for the specified project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiGetUsersWithoutPermissionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetUsersWithoutPermissionOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only user names containing the supplied string will be returned | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2005**](inline_response_200_5.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetWebhook**
> RestWebhook GetWebhook(ctx, projectKey, webhookId, optional)
Get webhook

Get a webhook by ID.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| ID of the webhook | 
 **optional** | ***ProjectApiGetWebhookOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiGetWebhookOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **statistics** | **optional.String**| &lt;code&gt;true&lt;/code&gt; if statistics should be provided for the webhook | 

### Return type

[**RestWebhook**](RestWebhook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **HasAllUserPermission**
> RestPermitted HasAllUserPermission(ctx, projectKey, permission)
Check default project permission

Check whether the specified permission is the default permission (granted to all users) for a project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **permission** | **string**| The permission to grant. Available project permissions are:  - PROJECT_READ - PROJECT_WRITE - PROJECT_ADMIN    | 

### Return type

[**RestPermitted**](RestPermitted.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ModifyAllUserPermission**
> ModifyAllUserPermission(ctx, projectKey, permission, optional)
Grant project permission

Grant or revoke a project permission to all users, i.e. set the default permission.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **permission** | **string**| The permission to grant. Available project permissions are:  - PROJECT_READ - PROJECT_WRITE - PROJECT_ADMIN    | 
 **optional** | ***ProjectApiModifyAllUserPermissionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiModifyAllUserPermissionOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **allow** | **optional.String**| &lt;em&gt;true&lt;/em&gt; to grant the specified permission to all users, or &lt;em&gt;false&lt;/em&gt; to revoke it | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RemoveConfiguration**
> RemoveConfiguration(ctx, projectKey, scriptId)
Remove a hook script

Removes the hook script from the set of hook scripts configured to run in all repositories under the project.   This endpoint requires **PROJECT_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **scriptId** | **string**| The ID of the hook script | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RetryCreateRepository**
> RestRepository RetryCreateRepository(ctx, projectKey, repositorySlug)
Retry repository creation

If a create or fork operation fails, calling this method will clean up the broken repository and try again. The repository must be in an INITIALISATION_FAILED state.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestRepository**](RestRepository.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokePermissions**
> RevokePermissions(ctx, projectKey, optional)
Revoke project permissions

Revoke all permissions for the specified project for the given groups and users.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.  In addition, a user may not revoke a group's permission if their own permission would be revoked as a result, nor may they revoke their own permission unless they have a global permission that already implies that permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiRevokePermissionsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiRevokePermissionsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **user** | **optional.String**| The names of the users | 
 **group** | **optional.String**| The names of the groups | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokePermissionsForGroup1**
> RevokePermissionsForGroup1(ctx, projectKey, optional)
Revoke group project permission

 Revoke all permissions for the specified project for a group.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.  In addition, a user may not revoke a group's permissions if it will reduce their own permission level.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiRevokePermissionsForGroup1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiRevokePermissionsForGroup1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **name** | **optional.String**| The name of the group | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokePermissionsForUser1**
> RevokePermissionsForUser1(ctx, projectKey, optional)
Revoke user project permission

Revoke all permissions for the specified project for a user.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.  In addition, a user may not revoke their own project permissions if they do not have a higher global permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiRevokePermissionsForUser1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiRevokePermissionsForUser1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **name** | **optional.String**| The name of the user | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SearchPermissions**
> SearchPermissions(ctx, projectKey, optional)
Search project permissions

Search direct and implied permissions of principals (users and groups). This endpoint returns a superset of the results returned by the /users and /groups endpoints because it allows filtering by global permissions too.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiSearchPermissionsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiSearchPermissionsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **permission** | **optional.String**| Permissions to filter by. See the [permissions documentation](https://confluence.atlassian.com/display/BitbucketServer/Using+project+permissions)for a detailed explanation of what each permission entails. This parameter can be specified multiple times to filter by more than one permission, and can contain global and project permissions.   | 
 **filterText** | **optional.String**| Name of the user or group to filter the name of | 
 **type_** | **optional.String**| Type of entity (user or group)Valid entity types are:  - USER- GROUP | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json;charset=UTF-8

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetAutoDeclineSettings**
> RestAutoDeclineSettings SetAutoDeclineSettings(ctx, projectKey, optional)
Create/Update auto decline settings

Creates or updates the auto decline settings for the supplied project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for this project to call the resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiSetAutoDeclineSettingsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiSetAutoDeclineSettingsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestAutoDeclineSettingsRequest**](RestAutoDeclineSettingsRequest.md)| The settings to create or update | 

### Return type

[**RestAutoDeclineSettings**](RestAutoDeclineSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetConfiguration**
> RestHookScriptConfig SetConfiguration(ctx, projectKey, scriptId, optional)
Create/update a hook script

Creates/updates the hook script configuration for the provided hook script and project.   This endpoint requires **PROJECT_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **scriptId** | **string**| The ID of the hook script | 
 **optional** | ***ProjectApiSetConfigurationOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiSetConfigurationOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestHookScriptTriggers**](RestHookScriptTriggers.md)| The hook triggers for which the hook script should be run | 

### Return type

[**RestHookScriptConfig**](RestHookScriptConfig.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetDefaultBranch2**
> SetDefaultBranch2(ctx, projectKey, repositorySlug, optional)
Update default branch for repository

Update the default branch of a repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiSetDefaultBranch2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiSetDefaultBranch2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestBranch**](RestBranch.md)| The branch to set as default | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetPermissionForGroups1**
> SetPermissionForGroups1(ctx, projectKey, optional)
Update group project permission

Promote or demote a group's permission level for the specified project.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource. In addition, a user may not demote a group's permission level if theirown permission level would be reduced as a result.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiSetPermissionForGroups1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiSetPermissionForGroups1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **name** | **optional.String**| The names of the groups | 
 **permission** | **optional.String**| The permission to grant.See the [permissions documentation](https://confluence.atlassian.com/display/BitbucketServer/Using+project+permissions)for a detailed explanation of what each permission entails. Available project permissions are:  - PROJECT_READ - PROJECT_WRITE - PROJECT_ADMIN    | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetPermissionForUsers1**
> SetPermissionForUsers1(ctx, projectKey, optional)
Update user project permission

Promote or demote a user's permission level for the specified project.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project or a higher global permission to call this resource. In addition, a user may not reduce their own permission level unless they have a global permission that already implies that permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***ProjectApiSetPermissionForUsers1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiSetPermissionForUsers1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **name** | **optional.String**| The names of the users | 
 **permission** | **optional.String**| The permission to grant.See the [permissions documentation](https://confluence.atlassian.com/display/BitbucketServer/Using+project+permissions)for a detailed explanation of what each permission entails. Available project permissions are:  - PROJECT_READ - PROJECT_WRITE - PROJECT_ADMIN    | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetSettings**
> ExampleSettings SetSettings(ctx, projectKey, hookKey, optional)
Update repository hook settings

Modify the settings for a repository hook for this project.   The service will reject any settings which are too large, the current limit is 32KB once serialized.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.   A JSON document can be provided to use as the settings for the hook. These structure and validity of the document is decided by the plugin providing the hook.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The complete module key of the hook module. | 
 **optional** | ***ProjectApiSetSettingsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiSetSettingsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of ExampleSettings**](ExampleSettings.md)| The raw settings. | 

### Return type

[**ExampleSettings**](ExampleSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamContributing**
> StreamContributing(ctx, projectKey, repositorySlug, optional)
Get repository contributing guidelines

Retrieves the contributing guidelines for the repository, if they've been defined.   This checks the repository for a CONTRIBUTING file, optionally with an md or txt extension, and, if found, streams it. By default, the <i>raw content</i> of the file is streamed. Appending <code>?markup</code> to the URL will stream an HTML-rendered version instead.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiStreamContributingOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiStreamContributingOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **at** | **optional.String**| A specific commit or ref to retrieve the guidelines at, or the default branch if not specified | 
 **markup** | **optional.String**| If present or &lt;code&gt;\&quot;true\&quot;&lt;/code&gt;, triggers the raw content to be markup-rendered and returned as HTML; otherwise, if not specified, or any value other than &lt;code&gt;\&quot;true\&quot;&lt;/code&gt;, the content is streamed without markup | 
 **htmlEscape** | **optional.String**| (Optional) true if HTML should be escaped in the input markup, false otherwise. If not specified, the value of the &lt;code&gt;markup.render.html.escape&lt;/code&gt; property, which is &lt;code&gt;true&lt;/code&gt; by default, will be used | 
 **includeHeadingId** | **optional.String**| (Optional) true if headings should contain an ID based on the heading content. If not specified, the value of the &lt;code&gt;markup.render.headerids&lt;/code&gt; property, which is false by default, will be used | 
 **hardwrap** | **optional.String**| (Optional) Whether the markup implementation should convert newlines to breaks. If not specified, the value of the &lt;code&gt;markup.render.hardwrap&lt;/code&gt; property, which is &lt;code&gt;true&lt;/code&gt; by default, will be used | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamLicense**
> StreamLicense(ctx, projectKey, repositorySlug, optional)
Get repository license

Retrieves the license for the repository, if it's been defined.   This checks the repository for a <pre>LICENSE</pre> file, optionally with an <pre>md</pre> or <pre>txt</pre>extension, and, if found, streams it. By default, the <i>raw content</i> of the file is streamed. Appending <pre>?markup</pre> to the URL will stream an HTML-rendered version instead.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiStreamLicenseOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiStreamLicenseOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **at** | **optional.String**| A specific commit or ref to retrieve the guidelines at, or the default branch if not specified | 
 **markup** | **optional.String**| If present or &lt;code&gt;\&quot;true\&quot;&lt;/code&gt;, triggers the raw content to be markup-rendered and returned as HTML; otherwise, if not specified, or any value other than &lt;code&gt;\&quot;true\&quot;&lt;/code&gt;, the content is streamed without markup | 
 **htmlEscape** | **optional.String**| (Optional) true if HTML should be escaped in the input markup, false otherwise. If not specified, the value of the &lt;code&gt;markup.render.html.escape&lt;/code&gt; property, which is &lt;code&gt;true&lt;/code&gt; by default, will be used | 
 **includeHeadingId** | **optional.String**| (Optional) true if headings should contain an ID based on the heading content. If not specified, the value of the &lt;code&gt;markup.render.headerids&lt;/code&gt; property, which is false by default, will be used | 
 **hardwrap** | **optional.String**| (Optional) Whether the markup implementation should convert newlines to breaks. If not specified, the value of the &lt;code&gt;markup.render.hardwrap&lt;/code&gt; property, which is &lt;code&gt;true&lt;/code&gt; by default, will be used | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamReadme**
> StreamReadme(ctx, projectKey, repositorySlug, optional)
Get repository readme

Retrieves the README for the repository, if it's been defined.   This checks the repository for a <pre>README</pre> file, optionally with an <pre>md</pre> or <pre>txt</pre>extension, and, if found, streams it. By default, the <i>raw content</i> of the file is streamed. Appending <pre>?markup</pre> to the URL will stream an HTML-rendered version instead. Note that, when streaming HTML, relative URLs in the README will not work if applied relative to this URL.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiStreamReadmeOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiStreamReadmeOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **at** | **optional.String**| A specific commit or ref to retrieve the guidelines at, or the default branch if not specified | 
 **markup** | **optional.String**| If present or &lt;code&gt;\&quot;true\&quot;&lt;/code&gt;, triggers the raw content to be markup-rendered and returned as HTML; otherwise, if not specified, or any value other than &lt;code&gt;\&quot;true\&quot;&lt;/code&gt;, the content is streamed without markup | 
 **htmlEscape** | **optional.String**| (Optional) true if HTML should be escaped in the input markup, false otherwise. If not specified, the value of the &lt;code&gt;markup.render.html.escape&lt;/code&gt; property, which is &lt;code&gt;true&lt;/code&gt; by default, will be used | 
 **includeHeadingId** | **optional.String**| (Optional) true if headings should contain an ID based on the heading content. If not specified, the value of the &lt;code&gt;markup.render.headerids&lt;/code&gt; property, which is false by default, will be used | 
 **hardwrap** | **optional.String**| (Optional) Whether the markup implementation should convert newlines to breaks. If not specified, the value of the &lt;code&gt;markup.render.hardwrap&lt;/code&gt; property, which is &lt;code&gt;true&lt;/code&gt; by default, will be used | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateProject**
> RestProject UpdateProject(ctx, projectKey, optional)
Update project

Update the project matching the <strong>projectKey</strong> supplied in the resource path.   To include a custom avatar for the updated project, the project definition should contain an additional attribute with the key <code>avatar</code> and the value a data URI containing Base64-encoded image data. The URI should be in the following format:  ```    data:(content type, e.g. image/png);base64,(data)```  If the data is not Base64-encoded, or if a character set is defined in the URI, or the URI is otherwise invalid, <em>project creation will fail</em>.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiUpdateProjectOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiUpdateProjectOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestProject**](RestProject.md)| Project parameters to update. | 

### Return type

[**RestProject**](RestProject.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdatePullRequestSettings**
> RestPullRequestSettings UpdatePullRequestSettings(ctx, projectKey, scmId, optional)
Update merge strategy

Update the pull request merge strategy configuration for this project and SCM.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the context repository to call this resource.   Only the strategies provided will be enabled, the default must be set and included in the set of strategies.   An explicitly set pull request merge strategy configuration can be deleted by POSTing a document with an empty \"mergeConfig\" attribute. i.e:  <pre>{      \"mergeConfig\": {}  }  </pre>  Upon completion of this request, the effective configuration will be the configuration explicitly set for the SCM, or if no such explicit configuration is set then the default configuration will be used.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **scmId** | **string**| The SCM to get strategies for. | 
 **optional** | ***ProjectApiUpdatePullRequestSettingsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiUpdatePullRequestSettingsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestPullRequestSettings**](RestPullRequestSettings.md)| The settings. | 

### Return type

[**RestPullRequestSettings**](RestPullRequestSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateRepository**
> RestRepository UpdateRepository(ctx, projectKey, repositorySlug, optional)
Update repository

Update the repository matching the <strong>repositorySlug</strong> supplied in the resource path.   The repository's slug is derived from its name. If the name changes the slug may also change.   This resource can be used to change the repository's default branch by specifying a new default branch in the request. For example: <code>\"defaultBranch\":\"main\"</code>  This resource can be used to move the repository to a different project by specifying a new project in the request. For example: <code>\"project\":{\"key\":\"NEW_KEY\"}</code>  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***ProjectApiUpdateRepositoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiUpdateRepositoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestRepository**](RestRepository.md)| The updated repository. | 

### Return type

[**RestRepository**](RestRepository.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateWebhook**
> RestWebhook UpdateWebhook(ctx, projectKey, webhookId, optional)
Update webhook

Update an existing webhook.   The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| Id of the existing webhook | 
 **optional** | ***ProjectApiUpdateWebhookOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiUpdateWebhookOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestWebhook**](RestWebhook.md)| The representation of the updated values for the webhook | 

### Return type

[**RestWebhook**](RestWebhook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UploadAvatar**
> UploadAvatar(ctx, projectKey, optional)
Update project avatar

Update the avatar for the project matching the supplied <strong>projectKey</strong>.   This resource accepts POST multipart form data, containing a single image in a form-field named 'avatar'.   There are configurable server limits on both the dimensions (1024x1024 pixels by default) and uploaded file size (1MB by default). Several different image formats are supported, but <strong>PNG</strong> and <strong>JPEG</strong> are preferred due to the file size limit.   This resource has Cross-Site Request Forgery (XSRF) protection. To allow the request to pass the XSRF check the caller needs to send an <code>X-Atlassian-Token</code> HTTP header with the value <code>no-check</code>.   An example <a href=\"http://curl.haxx.se/\">curl</a> request to upload an image name 'avatar.png' would be: ```curl -X POST -u username:password -H \"X-Atlassian-Token: no-check\" http://example.com/rest/api/1.0/projects/STASH/avatar.png -F avatar=@avatar.png ```  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***ProjectApiUploadAvatarOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a ProjectApiUploadAvatarOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **avatar** | **optional.Interface of *os.File****optional.**|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

