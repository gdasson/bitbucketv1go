# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateIssue**](JiraIntegrationApi.md#CreateIssue) | **Post** /jira/latest/comments/{commentId}/issues | Create Jira Issue
[**GetCommitsByIssueKey**](JiraIntegrationApi.md#GetCommitsByIssueKey) | **Get** /jira/latest/issues/{issueKey}/commits | Get changesets for issue key
[**GetEnhancedEntityLinkForProject**](JiraIntegrationApi.md#GetEnhancedEntityLinkForProject) | **Get** /jira/latest/projects/{projectKey}/primary-enhanced-entitylink | Get entity link
[**GetIssueKeysForPullRequest**](JiraIntegrationApi.md#GetIssueKeysForPullRequest) | **Get** /jira/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/issues | Get issues for a pull request

# **CreateIssue**
> RestCommentJiraIssue CreateIssue(ctx, commentId, optional)
Create Jira Issue

Create a Jira issue and associate it with a comment on a pull request.  This resource can only be used with comments on a pull request. Attempting to call this resource with a different type of comment (for example, a comment on a commit) will result in an error.    The authenticated user must have <strong>REPO_READ</strong> permission for the repository containing the comment to call this resource.  The JSON structure for the create issue format is specified by Jira's REST v2 API.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **commentId** | **string**| the comment to associate the created Jira issue to | 
 **optional** | ***JiraIntegrationApiCreateIssueOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a JiraIntegrationApiCreateIssueOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of string**](string.md)| A String representation of the JSON format Jira create issue request see: &lt;a href&#x3D;&quot;https://docs.atlassian.com/jira/REST/server/#api/2/issue-createIssue&quot;&gt;Jira REST API&lt;/a&gt; | 
 **applicationId** | **optional.**| id of the Jira server | 

### Return type

[**RestCommentJiraIssue**](RestCommentJiraIssue.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetCommitsByIssueKey**
> InlineResponse2006 GetCommitsByIssueKey(ctx, issueKey, optional)
Get changesets for issue key

Retrieve a page of changesets associated with the given issue key.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **issueKey** | **string**| The issue key to search by | 
 **optional** | ***JiraIntegrationApiGetCommitsByIssueKeyOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a JiraIntegrationApiGetCommitsByIssueKeyOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **maxChanges** | **optional.String**| The maximum number of changes to retrieve for each changeset | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2006**](inline_response_200_6.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetEnhancedEntityLinkForProject**
> RestEnhancedEntityLink GetEnhancedEntityLinkForProject(ctx, projectKey)
Get entity link

Retrieves the enchanced primary entitylink   The authenticated user must have <strong>PROJECT_READ</strong> permission for the project having the primary enhanced entitylink.   

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 

### Return type

[**RestEnhancedEntityLink**](RestEnhancedEntityLink.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetIssueKeysForPullRequest**
> []RestJiraIssue GetIssueKeysForPullRequest(ctx, projectKey, pullRequestId, repositorySlug)
Get issues for a pull request

Retrieves Jira issue keys that are associated with the commits in the specified pull request. The number of commits checked for issues is limited to a default of 100.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **pullRequestId** | **string**| The pull request id | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

[**[]RestJiraIssue**](RestJiraIssue.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json;charset=UTF-8

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

