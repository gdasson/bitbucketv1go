# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddBuildStatus**](DeprecatedApi.md#AddBuildStatus) | **Post** /build-status/latest/commits/{commitId} | Create build status for commit
[**AddGroupToUser**](DeprecatedApi.md#AddGroupToUser) | **Post** /api/latest/admin/users/add-group | Add user to group
[**AddUserToGroup**](DeprecatedApi.md#AddUserToGroup) | **Post** /api/latest/admin/groups/add-user | Add user to group
[**Approve**](DeprecatedApi.md#Approve) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/approve | Approve pull request
[**CountPullRequestTasks**](DeprecatedApi.md#CountPullRequestTasks) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/tasks/count | Get pull request task count
[**CreateTask**](DeprecatedApi.md#CreateTask) | **Post** /api/latest/tasks | Create task
[**DeleteTask**](DeprecatedApi.md#DeleteTask) | **Delete** /api/latest/tasks/{taskId} | Delete task
[**GetBuildStatus**](DeprecatedApi.md#GetBuildStatus) | **Get** /build-status/latest/commits/{commitId} | Get build statuses for commit
[**GetBuildStatusStats**](DeprecatedApi.md#GetBuildStatusStats) | **Get** /build-status/latest/commits/stats/{commitId} | Get build status statistics for commit
[**GetDefaultBranch1**](DeprecatedApi.md#GetDefaultBranch1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/branches/default | Get default branch
[**GetLikers**](DeprecatedApi.md#GetLikers) | **Get** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId}/likes | Get comment likes
[**GetLikers1**](DeprecatedApi.md#GetLikers1) | **Get** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId}/likes | Get pull request comment likes
[**GetPullRequestTasks**](DeprecatedApi.md#GetPullRequestTasks) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/tasks | Get pull request tasks
[**GetTask**](DeprecatedApi.md#GetTask) | **Get** /api/latest/tasks/{taskId} | Get task
[**Like**](DeprecatedApi.md#Like) | **Post** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId}/likes | Like a commit comment
[**Like1**](DeprecatedApi.md#Like1) | **Post** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId}/likes | Like a pull request comment
[**OnAddonDisabled**](DeprecatedApi.md#OnAddonDisabled) | **Post** /mirroring/latest/upstreamServers/{upstreamId}/addon/disabled | On disable of mirror addon
[**OnAddonEnabled**](DeprecatedApi.md#OnAddonEnabled) | **Post** /mirroring/latest/upstreamServers/{upstreamId}/addon/enabled | On enabled of mirror addon
[**RemoveUserFromGroup**](DeprecatedApi.md#RemoveUserFromGroup) | **Post** /api/latest/admin/groups/remove-user | Remove user from group
[**SetDefaultBranch1**](DeprecatedApi.md#SetDefaultBranch1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/branches/default | Update default branch
[**SynchronizeRepositoryWithUpstream**](DeprecatedApi.md#SynchronizeRepositoryWithUpstream) | **Post** /mirroring/latest/upstreamServers/{upstreamId}/repos/{upstreamRepoId}/synchronization | Get upstream settings
[**SynchronizeWithUpstream**](DeprecatedApi.md#SynchronizeWithUpstream) | **Post** /mirroring/latest/upstreamServers/{upstreamId}/synchronization | Change upstream settings
[**UnassignParticipantRole1**](DeprecatedApi.md#UnassignParticipantRole1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants | Unassign pull request participant
[**Unlike**](DeprecatedApi.md#Unlike) | **Delete** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId}/likes | Unlike a commit comment
[**Unlike1**](DeprecatedApi.md#Unlike1) | **Delete** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId}/likes | Unlike a pull request comment
[**UpdateTask**](DeprecatedApi.md#UpdateTask) | **Put** /api/latest/tasks/{taskId} | Update task
[**WithdrawApproval**](DeprecatedApi.md#WithdrawApproval) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/approve | Unapprove pull request

# **AddBuildStatus**
> AddBuildStatus(ctx, commitId, optional)
Create build status for commit

Associates a build status with a commit.The <code>state</code>, the <code>key</code> and the <code>url</code> fields are mandatory. The <code>name</code> and<code>description</code> fields are optional.All fields (mandatory or optional) are limited to 255 characters, except for the <code>url</code>,which is limited to 450 characters.Supported values for the <code>state</code> are <code>SUCCESSFUL</code>, <code>FAILED</code>and <code>INPROGRESS</code>.The authenticated user must have <strong>LICENSED</strong> permission or higher to call this resource.  <strong>Deprecated in 7.14, please use the repository based builds resource instead.</strong>

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **commitId** | **string**| full SHA1 of the commit | 
 **optional** | ***DeprecatedApiAddBuildStatusOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiAddBuildStatusOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestBuildStatus**](RestBuildStatus.md)| build status to associate with the commit | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AddGroupToUser**
> AddGroupToUser(ctx, optional)
Add user to group

<strong>Deprecated since 2.10</strong>. Use /rest/users/add-groups instead.  Add a user to a group. This is very similar to <code>groups/add-user</code>, but with the <em>context</em> and <em>itemName</em> attributes of the supplied request entity reversed. On the face of it this may appear redundant, but it facilitates a specific UI component in the application.  In the request entity, the <em>context</em> attribute is the user and the <em>itemName</em> is the group.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***DeprecatedApiAddGroupToUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiAddGroupToUserOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of GroupPickerContext**](GroupPickerContext.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AddUserToGroup**
> AddUserToGroup(ctx, optional)
Add user to group

<strong>Deprecated since 2.10</strong>. Use /rest/users/add-groups instead.  Add a user to a group.  In the request entity, the <em>context</em> attribute is the group and the <em>itemName</em> is the user.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***DeprecatedApiAddUserToGroupOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiAddUserToGroupOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of UserPickerContext**](UserPickerContext.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Approve**
> RestPullRequestParticipant Approve(ctx, projectKey, pullRequestId, repositorySlug)
Approve pull request

Approve a pull request as the current user. Implicitly adds the user as a participant if they are not already.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.   <strong>Deprecated since 4.2</strong>. Use /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants/{userSlug} instead

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestPullRequestParticipant**](RestPullRequestParticipant.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CountPullRequestTasks**
> CountPullRequestTasks(ctx, projectKey, pullRequestId, repositorySlug)
Get pull request task count

Retrieve the total number of OPEN and RESOLVED tasks associated with a pull request.    <strong>Deprecated since 7.2</strong>. Tasks are now managed using Comments with BLOCKER severity. Use /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments?count=true instead.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateTask**
> CreateTask(ctx, )
Create task

Create a new task.   <strong>Removed in 8.0</strong>. Tasks are now managed using Comments with severity BLOCKER. Call <code>POST /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments</code> instead,passing the attribute 'severity' set to 'BLOCKER'.

### Required Parameters
This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteTask**
> DeleteTask(ctx, taskId)
Delete task

Delete a task.  <strong>Removed in 8.0</strong>. Tasks are now managed using Comments with BLOCKER severity. Call <code>DELETE /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId}</code>instead. @deprecated since 7.2, changed to 404 in 8.0, remove in 9.0. Call DELETE /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} instead.  Note that only the task's creator, the context's author or an admin of the context's repository can delete a task. (For a pull request task, those are the task's creator, the pull request's author or an admin on the repository containing the pull request). Additionally a task cannot be deleted if it has already been resolved.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **taskId** | **string**| the id identifying the task to delete | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetBuildStatus**
> InlineResponse2001 GetBuildStatus(ctx, commitId, optional)
Get build statuses for commit

Gets build statuses associated with a commit.  <strong>Deprecated in 7.14, please use the repository based builds resource instead.</strong>

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **commitId** | **string**| Full SHA1 of the commit (ex: &lt;code&gt;e00cf62997a027bbf785614a93e2e55bb331d268&lt;/code&gt;) | 
 **optional** | ***DeprecatedApiGetBuildStatusOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiGetBuildStatusOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **orderBy** | **optional.String**| How the results should be ordered. Options are NEWEST, OLDEST, STATUS | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2001**](inline_response_200_1.md)

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
 **optional** | ***DeprecatedApiGetBuildStatusStatsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiGetBuildStatusStatsOpts struct
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

# **GetDefaultBranch1**
> RestBranch GetDefaultBranch1(ctx, projectKey, repositorySlug)
Get default branch

Retrieves the repository's default branch, if it has been created. If the repository is empty, 204 No Content will be returned. For non-empty repositories, if the configured default branch has not yet been created a 404 Not Found will be returned.   This URL is deprecated. Callers should use <code>GET /projects/{key}/repos/{slug}/default-branch</code> instead, which allows retrieving the <i>configured</i> default branch even if the ref has not been created yet.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestBranch**](RestBranch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetLikers**
> InlineResponse2005 GetLikers(ctx, projectKey, commentId, commitId, repositorySlug, optional)
Get comment likes

Get a page of users who liked a commit comment in the specified repository, identified by <code>commitId</code> and <code>commentId</code>.  The authenticated user must have the **REPO_READ** (or higher) permission for the specified repository to access this resource.  <strong>Deprecated in 8.0 to be removed in 9.0.</strong>

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **int64**|  | 
  **commitId** | **string**| The commit id. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***DeprecatedApiGetLikersOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiGetLikersOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




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

# **GetLikers1**
> InlineResponse2005 GetLikers1(ctx, projectKey, commentId, pullRequestId, repositorySlug, optional)
Get pull request comment likes

Get a page of users who liked a pull request comment in the specified repository, identified by <code>pullRequestId</code> and <code>commentId</code>.   The authenticated user must have the <strong>REPO_READ</strong> (or higher) permission for the specified repository to access this resource.  **Deprecated in 8.0 to be removed in 9.0.**

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The comment id. | 
  **pullRequestId** | **string**| The pull request id. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***DeprecatedApiGetLikers1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiGetLikers1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




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

# **GetPullRequestTasks**
> GetPullRequestTasks(ctx, projectKey, pullRequestId, repositorySlug)
Get pull request tasks

Retrieve the tasks associated with a pull request.   **Removed in 8.0**. Tasks are now managed using Comments with BLOCKER severity. Use /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments instead   **Deprecated since 7.2, changed to 404 in 8.0, remove in 9.0.** Use /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments instead

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetTask**
> GetTask(ctx, taskId)
Get task

Retrieve an existing task.  <strong>Removed in 8.0</strong>. Tasks are now managed using Comments with BLOCKER severity. Call <code>GET /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} </code>instead. @deprecated since 7.2, changed to 404 in 8.0, remove in 9.0. Call GET /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} instead.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **taskId** | **string**| the id identifying the task | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Like**
> Like(ctx, projectKey, commentId, commitId, repositorySlug)
Like a commit comment

Like a commit comment in the specified repository, identified by <code>commitId</code> and <code>commentId</code>.  The authenticated user must have the <strong>REPO_READ</strong> (or higher) permission for the specified repository to access this resource.  <strong>Deprecated in 8.0 to be removed in 9.0.</strong> Likes have been replaced with reactions. For backwards compatibility, the <pre>thumbsup</pre> reaction is treated as a like.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **int64**|  | 
  **commitId** | **string**| The commit id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Like1**
> Like1(ctx, projectKey, commentId, pullRequestId, repositorySlug)
Like a pull request comment

Like a pull request comment in the specified repository, identified by <code>pullRequestId</code> and <code>commentId</code>. The like will be recorded against the requesting user.  The authenticated user must have the <strong>REPO_READ</strong> (or higher) permission for the specified repository to access this resource.  **Deprecated in 8.0 to be removed in 9.0.** Likes have been replaced with reactions. For backwards compatibility, the <pre>thumbsup</pre> reaction is treated as a like.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The comment id. | 
  **pullRequestId** | **string**| The pull request id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **OnAddonDisabled**
> OnAddonDisabled(ctx, upstreamId)
On disable of mirror addon

This REST endpoint is retained for backwards compatibility only. It is a no-op. Starting from 4.6.0, mirrors no longer specify a disabled lifecycle callback in their addon descriptor. Prior to 4.6.0, this was the callback method that was called when the mirroring atlassian-connect add-on has been disabled in the upstream server identified by <code> upstreamId</code>.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **upstreamId** | **string**| the upstream server ID to retrieve settings for | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **OnAddonEnabled**
> OnAddonEnabled(ctx, upstreamId)
On enabled of mirror addon

This REST endpoint is retained for backwards compatibility only. It is a no-op. Starting from 4.6.0, mirrors no longer specify an enabled lifecycle callback in their addon descriptor. Prior to 4.6.0, this was the callback method that was called when the mirroring atlassian-connect add-on has been enabled in the upstream server identified by <code>upstreamId</code>.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **upstreamId** | **string**| the upstream server ID to retrieve settings for | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RemoveUserFromGroup**
> RemoveUserFromGroup(ctx, optional)
Remove user from group

<strong>Deprecated since 2.10</strong>. Use /rest/users/remove-groups instead.  Remove a user from a group.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.  In the request entity, the <em>context</em> attribute is the group and the <em>itemName</em> is the user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***DeprecatedApiRemoveUserFromGroupOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiRemoveUserFromGroupOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of UserPickerContext**](UserPickerContext.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetDefaultBranch1**
> SetDefaultBranch1(ctx, projectKey, repositorySlug, optional)
Update default branch

Update the default branch of a repository.   This URL is deprecated. Callers should use <code>PUT /projects/{key}/repos/{slug}/default-branch</code> instead.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***DeprecatedApiSetDefaultBranch1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiSetDefaultBranch1Opts struct
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

# **SynchronizeRepositoryWithUpstream**
> SynchronizeRepositoryWithUpstream(ctx, upstreamRepoId, upstreamId, optional)
Get upstream settings

This method is no longer supported

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **upstreamRepoId** | **string**|  | 
  **upstreamId** | **string**| the upstream server ID to retrieve settings for | 
 **optional** | ***DeprecatedApiSynchronizeRepositoryWithUpstreamOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiSynchronizeRepositoryWithUpstreamOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **level** | **optional.String**| the level of synchronization to perform | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SynchronizeWithUpstream**
> SynchronizeWithUpstream(ctx, upstreamId, optional)
Change upstream settings

This method is no longer supported

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **upstreamId** | **string**| the upstream server ID to retrieve settings for | 
 **optional** | ***DeprecatedApiSynchronizeWithUpstreamOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiSynchronizeWithUpstreamOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **level** | **optional.String**|  | [default to DEFAULT]

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UnassignParticipantRole1**
> UnassignParticipantRole1(ctx, projectKey, pullRequestId, repositorySlug, optional)
Unassign pull request participant

Unassigns a participant from the REVIEWER role they may have been given in a pull request.   If the participant has no explicit role this method has no effect.   Afterwards, the user will still remain a participant in the pull request but their role will be reduced to PARTICIPANT. This is because once made a participant of a pull request, a user will forever remain a participant. Only their role may be altered.   The authenticated user must have <strong>REPO_WRITE</strong> permission for the repository that this pull request targets to call this resource.   <strong>Deprecated since 4.2</strong>. Use /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants/{userSlug} instead.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***DeprecatedApiUnassignParticipantRole1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DeprecatedApiUnassignParticipantRole1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **username** | **optional.String**|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Unlike**
> Unlike(ctx, projectKey, commentId, commitId, repositorySlug)
Unlike a commit comment

Unlike a commit comment in the specified repository, identified by <code>commitId</code> and <code>commentId</code>.  The authenticated user must have the <strong>REPO_READ</strong> (or higher) permission for the specified repository to access this resource.  <strong>Deprecated in 8.0 to be removed in 9.0.</strong> Likes have been replaced with reactions. For backwards compatibility, the <pre>thumbsup</pre> reaction is treated as a like.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **int64**|  | 
  **commitId** | **string**| The commit id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Unlike1**
> Unlike1(ctx, projectKey, commentId, pullRequestId, repositorySlug)
Unlike a pull request comment

Unlike a pull request comment in the specified repository, identified by <code>pullRequestId</code> and <code>commentId</code>.  The authenticated user must have the <strong>REPO_READ</strong> (or higher) permission for the specified repository to access this resource.  **Deprecated in 8.0 to be removed in 9.0.** Likes have been replaced with reactions. For backwards compatibility, the <pre>thumbsup</pre> reaction is treated as a like.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The comment id. | 
  **pullRequestId** | **string**| The pull request id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateTask**
> UpdateTask(ctx, taskId)
Update task

Update an existing task.     <strong>Removed in 8.0</strong>.  Tasks are now managed using Comments with BLOCKER severity.  Call <code>PUT /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} </code> instead.  To resolve a task, pass the attribute 'state' set to 'RESOLVED'.  @deprecated since 7.2, changed to 404 in 8.0, remove in 9.0. Call <code>PUT  /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} </code> instead.    As of Stash 3.3, only the state and text of a task can be updated.    Updating the state of a task is allowed for any user having <em>READ</em> access to the repository.  However only the task's creator, the context's author or an admin of the context's repository can update the task's text. (For a pull request task, those are the task's creator, the pull request's author or an admin on the repository containing the pull request). Additionally the task's text cannot be updated if it has been resolved.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **taskId** | **string**| the id identifying the task to update | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **WithdrawApproval**
> RestPullRequestParticipant WithdrawApproval(ctx, projectKey, pullRequestId, repositorySlug)
Unapprove pull request

Remove approval from a pull request as the current user. This does not remove the user as a participant.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.   <strong>Deprecated since 4.2</strong>. Use /rest/api/1.0/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants/{userSlug} instead

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestPullRequestParticipant**](RestPullRequestParticipant.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

