# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddLabel**](RepositoryApi.md#AddLabel) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/labels | Add repository label
[**CreateBranch**](RepositoryApi.md#CreateBranch) | **Post** /branch-utils/latest/projects/{projectKey}/repos/{repositorySlug}/branches | Create branch
[**CreateBranchForRepository**](RepositoryApi.md#CreateBranchForRepository) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/branches | Create branch
[**CreateComment**](RepositoryApi.md#CreateComment) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments | Add a new commit comment
[**CreateRestrictions1**](RepositoryApi.md#CreateRestrictions1) | **Post** /branch-permissions/latest/projects/{projectKey}/repos/{repositorySlug}/restrictions | Create multiple ref restrictions
[**CreateTag**](RepositoryApi.md#CreateTag) | **Post** /git/latest/projects/{projectKey}/repos/{repositorySlug}/tags | Create tag
[**CreateTagForRepository**](RepositoryApi.md#CreateTagForRepository) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/tags | Create tag
[**CreateWebhook1**](RepositoryApi.md#CreateWebhook1) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/webhooks | Create webhook
[**DeleteAttachment**](RepositoryApi.md#DeleteAttachment) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/attachments/{attachmentId} | Delete an attachment
[**DeleteAttachmentMetadata**](RepositoryApi.md#DeleteAttachmentMetadata) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/attachments/{attachmentId}/metadata | Delete attachment metadata
[**DeleteAutoDeclineSettings1**](RepositoryApi.md#DeleteAutoDeclineSettings1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/auto-decline | Delete auto decline settings
[**DeleteBranch**](RepositoryApi.md#DeleteBranch) | **Delete** /branch-utils/latest/projects/{projectKey}/repos/{repositorySlug}/branches | Delete branch
[**DeleteComment**](RepositoryApi.md#DeleteComment) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId} | Delete a commit comment
[**DeleteRepositoryHook**](RepositoryApi.md#DeleteRepositoryHook) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/hooks/{hookKey} | Delete repository hook
[**DeleteRestriction1**](RepositoryApi.md#DeleteRestriction1) | **Delete** /branch-permissions/latest/projects/{projectKey}/repos/{repositorySlug}/restrictions/{id} | Delete a ref restriction
[**DeleteTag**](RepositoryApi.md#DeleteTag) | **Delete** /git/latest/projects/{projectKey}/repos/{repositorySlug}/tags/{name} | Delete tag
[**DeleteWebhook1**](RepositoryApi.md#DeleteWebhook1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/webhooks/{webhookId} | Delete webhook
[**DisableHook1**](RepositoryApi.md#DisableHook1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/hooks/{hookKey}/enabled | Disable repository hook
[**EditFile**](RepositoryApi.md#EditFile) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/browse/{path} | Edit file
[**EnableHook1**](RepositoryApi.md#EnableHook1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/hooks/{hookKey}/enabled | Enable repository hook
[**FindBranches**](RepositoryApi.md#FindBranches) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/ref-change-activities/branches | Get branches with ref change activities for repository
[**FindByCommit**](RepositoryApi.md#FindByCommit) | **Get** /branch-utils/latest/projects/{projectKey}/repos/{repositorySlug}/branches/info/{commitId} | Get branch
[**FindWebhooks1**](RepositoryApi.md#FindWebhooks1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/webhooks | Find webhooks
[**GetAllLabelsForRepository**](RepositoryApi.md#GetAllLabelsForRepository) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/labels | Get repository labels
[**GetArchive**](RepositoryApi.md#GetArchive) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/archive | Stream archive of repository
[**GetAttachment**](RepositoryApi.md#GetAttachment) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/attachments/{attachmentId} | Get an attachment
[**GetAttachmentMetadata**](RepositoryApi.md#GetAttachmentMetadata) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/attachments/{attachmentId}/metadata | Get attachment metadata
[**GetAutoDeclineSettings1**](RepositoryApi.md#GetAutoDeclineSettings1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/auto-decline | Get auto decline settings
[**GetBranches**](RepositoryApi.md#GetBranches) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/branches | Find branches
[**GetChanges**](RepositoryApi.md#GetChanges) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/changes | Get changes in commit
[**GetChanges1**](RepositoryApi.md#GetChanges1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/changes | Get changes made in commit
[**GetComment**](RepositoryApi.md#GetComment) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId} | Get a commit comment
[**GetComments**](RepositoryApi.md#GetComments) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments | Search for commit comments
[**GetCommit**](RepositoryApi.md#GetCommit) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId} | Get commit by ID
[**GetCommits**](RepositoryApi.md#GetCommits) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits | Get commits
[**GetConfigurations1**](RepositoryApi.md#GetConfigurations1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/hook-scripts | Get hook scripts
[**GetContent**](RepositoryApi.md#GetContent) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/browse | Get file content at revision
[**GetContent1**](RepositoryApi.md#GetContent1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/browse/{path} | Get file content
[**GetDefaultBranch1**](RepositoryApi.md#GetDefaultBranch1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/branches/default | Get default branch
[**GetLatestInvocation1**](RepositoryApi.md#GetLatestInvocation1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/webhooks/{webhookId}/latest | Get last webhook invocation details
[**GetPullRequestSettings1**](RepositoryApi.md#GetPullRequestSettings1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/pull-requests | Get pull request settings
[**GetRefChangeActivity**](RepositoryApi.md#GetRefChangeActivity) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/ref-change-activities | Get ref change activity
[**GetRepositories1**](RepositoryApi.md#GetRepositories1) | **Get** /api/latest/repos | Search for repositories
[**GetRepositoriesRecentlyAccessed**](RepositoryApi.md#GetRepositoriesRecentlyAccessed) | **Get** /api/latest/profile/recent/repos | Get recently accessed repositories
[**GetRepositoryHook1**](RepositoryApi.md#GetRepositoryHook1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/hooks/{hookKey} | Get repository hook
[**GetRepositoryHooks1**](RepositoryApi.md#GetRepositoryHooks1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/hooks | Get repository hooks
[**GetRestriction1**](RepositoryApi.md#GetRestriction1) | **Get** /branch-permissions/latest/projects/{projectKey}/repos/{repositorySlug}/restrictions/{id} | Get a ref restriction
[**GetRestrictions1**](RepositoryApi.md#GetRestrictions1) | **Get** /branch-permissions/latest/projects/{projectKey}/repos/{repositorySlug}/restrictions | Search for ref restrictions
[**GetSettings1**](RepositoryApi.md#GetSettings1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/hooks/{hookKey}/settings | Get repository hook settings
[**GetStatus**](RepositoryApi.md#GetStatus) | **Get** /sync/latest/projects/{projectKey}/repos/{repositorySlug} | Get synchronization status
[**GetTag**](RepositoryApi.md#GetTag) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/tags/{name} | Get tag
[**GetTags**](RepositoryApi.md#GetTags) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/tags | Find tag
[**GetWebhook1**](RepositoryApi.md#GetWebhook1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/webhooks/{webhookId} | Get webhook
[**React**](RepositoryApi.md#React) | **Put** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId}/reactions/{emoticon} | React to a comment
[**RemoveConfiguration1**](RepositoryApi.md#RemoveConfiguration1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/hook-scripts/{scriptId} | Remove a hook script
[**RemoveLabel**](RepositoryApi.md#RemoveLabel) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/labels/{labelName} | Remove repository label
[**SaveAttachmentMetadata**](RepositoryApi.md#SaveAttachmentMetadata) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/attachments/{attachmentId}/metadata | Save attachment metadata
[**SearchWebhooks**](RepositoryApi.md#SearchWebhooks) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/webhooks/search | Search webhooks
[**SetAutoDeclineSettings1**](RepositoryApi.md#SetAutoDeclineSettings1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/auto-decline | Create auto decline settings
[**SetConfiguration1**](RepositoryApi.md#SetConfiguration1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/hook-scripts/{scriptId} | Create/update a hook script
[**SetDefaultBranch1**](RepositoryApi.md#SetDefaultBranch1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/branches/default | Update default branch
[**SetEnabled**](RepositoryApi.md#SetEnabled) | **Post** /sync/latest/projects/{projectKey}/repos/{repositorySlug} | Disable synchronization
[**SetSettings1**](RepositoryApi.md#SetSettings1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/hooks/{hookKey}/settings | Update repository hook settings
[**Stream**](RepositoryApi.md#Stream) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/last-modified | Stream files
[**Stream1**](RepositoryApi.md#Stream1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/last-modified/{path} | Stream files with last modified commit in path
[**StreamChanges**](RepositoryApi.md#StreamChanges) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/compare/changes | Compare commits
[**StreamCommits**](RepositoryApi.md#StreamCommits) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/compare/commits | Get accessible commits
[**StreamDiff**](RepositoryApi.md#StreamDiff) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/diff/{path} | Get diff between revisions
[**StreamDiff1**](RepositoryApi.md#StreamDiff1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/compare/diff{path} | Get diff between commits
[**StreamFiles**](RepositoryApi.md#StreamFiles) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/files/{path} | Get files in directory
[**StreamFiles1**](RepositoryApi.md#StreamFiles1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/files | Get files in directory
[**StreamPatch**](RepositoryApi.md#StreamPatch) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/patch | Get patch content at revision
[**StreamRaw**](RepositoryApi.md#StreamRaw) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/raw/{path} | Get raw content of a file at revision
[**StreamRawDiff**](RepositoryApi.md#StreamRawDiff) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/diff | Get raw diff for path
[**StreamRawDiff1**](RepositoryApi.md#StreamRawDiff1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/diff/{path} | Get raw diff for path
[**Synchronize**](RepositoryApi.md#Synchronize) | **Post** /sync/latest/projects/{projectKey}/repos/{repositorySlug}/synchronize | Manual synchronization
[**UnReact**](RepositoryApi.md#UnReact) | **Delete** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId}/reactions/{emoticon} | Remove a reaction from comment
[**Unwatch**](RepositoryApi.md#Unwatch) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/watch | Stop watching commit
[**Unwatch2**](RepositoryApi.md#Unwatch2) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/watch | Stop watching repository
[**UpdateComment**](RepositoryApi.md#UpdateComment) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/comments/{commentId} | Update a commit comment
[**UpdatePullRequestSettings1**](RepositoryApi.md#UpdatePullRequestSettings1) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/pull-requests | Update pull request settings
[**UpdateWebhook1**](RepositoryApi.md#UpdateWebhook1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/webhooks/{webhookId} | Update webhook
[**Watch**](RepositoryApi.md#Watch) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/watch | Watch commit
[**Watch2**](RepositoryApi.md#Watch2) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/watch | Watch repository

# **AddLabel**
> RestLabel AddLabel(ctx, projectKey, repositorySlug, optional)
Add repository label

Applies a label to the repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiAddLabelOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiAddLabelOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestLabel**](RestLabel.md)| The label to apply | 

### Return type

[**RestLabel**](RestLabel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateBranch**
> RestBranch CreateBranch(ctx, body, projectKey, repositorySlug)
Create branch

 Creates a branch in the specified repository.   The authenticated user must have an effective <strong>REPO_WRITE</strong> permission to call this resource. If branch permissions are set up in the repository, the authenticated user must also have access to the branch name that is to be created.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestBranchCreateRequest**](RestBranchCreateRequest.md)|  | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestBranch**](RestBranch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateBranchForRepository**
> RestBranch CreateBranchForRepository(ctx, projectKey, repositorySlug, optional)
Create branch

Creates a branch using the information provided in the RestCreateBranchRequest request   The authenticated user must have <strong>REPO_WRITE</strong> permission for the context repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiCreateBranchForRepositoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiCreateBranchForRepositoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestCreateBranchRequest**](RestCreateBranchRequest.md)| The request to create a branch containing a &lt;strong&gt;name&lt;/strong&gt;, &lt;strong&gt;startPoint&lt;/strong&gt;, and optionally a &lt;strong&gt;message&lt;/strong&gt; | 

### Return type

[**RestBranch**](RestBranch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateComment**
> RestComment CreateComment(ctx, projectKey, commitId, repositorySlug, optional)
Add a new commit comment

Add a new comment.  Comments can be added in a few places by setting different attributes:  General commit comment:  ```{       \"text\": \"An insightful general comment on a commit.\" }  </pre> Reply to a comment: <pre>{       \"text\": \"A measured reply.\",       \"parent\": {           \"id\": 1       } } </pre> General file comment: <pre>{       \"text\": \"An insightful general comment on a file.\",       \"anchor\": {           \"diffType\": \"COMMIT\",           \"fromHash\": \"6df3858eeb9a53a911cd17e66a9174d44ffb02cd\",           \"path\": \"path/to/file\",           \"srcPath\": \"path/to/file\",           \"toHash\": \"04c7c5c931b9418ca7b66f51fe934d0bd9b2ba4b\"       } } </pre> File line comment: <pre>{       \"text\": \"A pithy comment on a particular line within a file.\",       \"anchor\": {           \"diffType\": \"COMMIT\",           \"line\": 1,           \"lineType\": \"CONTEXT\",           \"fileType\": \"FROM\",           \"fromHash\": \"6df3858eeb9a53a911cd17e66a9174d44ffb02cd\",           \"path\": \"path/to/file\",           \"srcPath\": \"path/to/file\",           \"toHash\": \"04c7c5c931b9418ca7b66f51fe934d0bd9b2ba4b\"       } } ```  Note: general file comments are an experimental feature and may change in the near future!  For file and line comments, 'path' refers to the path of the file to which the comment should be applied and 'srcPath' refers to the path the that file used to have (only required for copies and moves). Also, fromHash and toHash refer to the sinceId / untilId (respectively) used to produce the diff on which the comment was added. Finally diffType refers to the type of diff the comment was added on.  For line comments, 'line' refers to the line in the diff that the comment should apply to. 'lineType' refers to the type of diff hunk, which can be:- 'ADDED' - for an added line;</li>- 'REMOVED' - for a removed line; or</li>- 'CONTEXT' - for a line that was unmodified but is in the vicinity of the diff.</li>'fileType' refers to the file of the diff to which the anchor should be attached - which is of relevance when displaying the diff in a side-by-side way. Currently the supported values are:- 'FROM' - the source file of the diff</li>- 'TO' - the destination file of the diff</li>If the current user is not a participant the user is added as one and updated to watch the commit.  The authenticated user must have REPO_READ permission for the repository that the commit is in to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiCreateCommentOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiCreateCommentOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestComment**](RestComment.md)| the comment | 
 **since** | **optional.**| For a merge commit, a parent can be provided to specify which diff the comments should be on. For a commit range, a sinceId can be provided to specify where the comments should be anchored from. | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRestrictions1**
> RestRefRestriction CreateRestrictions1(ctx, projectKey, repositorySlug, optional)
Create multiple ref restrictions

Allows creating multiple restrictions at once.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiCreateRestrictions1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiCreateRestrictions1Opts struct
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

# **CreateTag**
> RestTag CreateTag(ctx, projectKey, repositorySlug, optional)
Create tag

Creates a tag in the specified repository.  The authenticated user must have an effective <strong>REPO_WRITE</strong> permission to call this resource.  'LIGHTWEIGHT' and 'ANNOTATED' are the two type of tags that can be created. The 'startPoint' can either be a ref or a 'commit'.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiCreateTagOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiCreateTagOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestGitTagCreateRequest**](RestGitTagCreateRequest.md)| The create git tag request. | 

### Return type

[**RestTag**](RestTag.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateTagForRepository**
> RestTag CreateTagForRepository(ctx, projectKey, repositorySlug, optional)
Create tag

Creates a tag using the information provided in the RestCreateTagRequest request   The authenticated user must have <strong>REPO_WRITE</strong> permission for the context repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiCreateTagForRepositoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiCreateTagForRepositoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestCreateTagRequest**](RestCreateTagRequest.md)| The request to create a tag containing a &lt;strong&gt;name&lt;/strong&gt;, &lt;strong&gt;startPoint&lt;/strong&gt;, and optionally a &lt;strong&gt;message&lt;/strong&gt; | 

### Return type

[**RestTag**](RestTag.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateWebhook1**
> RestWebhook CreateWebhook1(ctx, projectKey, repositorySlug, optional)
Create webhook

Create a webhook for the repository specified via the URL.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiCreateWebhook1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiCreateWebhook1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestWebhook**](RestWebhook.md)| The webhook to be created for this repository. | 

### Return type

[**RestWebhook**](RestWebhook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAttachment**
> DeleteAttachment(ctx, projectKey, attachmentId, repositorySlug)
Delete an attachment

Delete an attachment.  The user must be authenticated and have <strong>REPO_ADMIN</strong> permission for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **attachmentId** | **string**| the attachment ID | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAttachmentMetadata**
> DeleteAttachmentMetadata(ctx, projectKey, attachmentId, repositorySlug)
Delete attachment metadata

Delete attachment metadata.  The user must be authenticated and have <strong>REPO_ADMIN</strong> permission for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **attachmentId** | **string**| the attachment ID | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAutoDeclineSettings1**
> DeleteAutoDeclineSettings1(ctx, projectKey, repositorySlug)
Delete auto decline settings

Delete auto decline settings for the supplied repository.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for this repository to call the resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteBranch**
> DeleteBranch(ctx, projectKey, repositorySlug, optional)
Delete branch

 Deletes a branch in the specified repository.    If the branch does not exist, this operation will not raise an error. In other words after calling this resource  and receiving a 204 response the branch provided in the request is guaranteed to not exist in the specified  repository any more, regardless of its existence beforehand.    The optional 'endPoint' parameter of the request may contain a commit ID that the provided ref name is  expected to point to. Should the ref point to a different commit ID, a 400 response will be returned with  appropriate error details.    The authenticated user must have an effective <strong>REPO_WRITE</strong> permission to call this resource. If  branch permissions are set up in the repository, the authenticated user must also have access to the branch name  that is to be deleted.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiDeleteBranchOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiDeleteBranchOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestBranchDeleteRequest**](RestBranchDeleteRequest.md)| Branch delete request | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteComment**
> DeleteComment(ctx, projectKey, commentId, commitId, repositorySlug, optional)
Delete a commit comment

Delete a commit comment. Anyone can delete their own comment. Only users with <strong>REPO_ADMIN</strong> and above may delete comments created by other users. Comments which have replies <i>may not be deleted</i>, regardless of the user's granted permissions.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that the commit is in to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commentId** | **string**| the comment | 
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiDeleteCommentOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiDeleteCommentOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **version** | **optional.String**| The expected version of the comment. This must match the server&#x27;s version of the comment or the delete will fail. To determine the current version of the comment, the comment should be fetched from the server prior to the delete. Look for the &#x27;version&#x27; attribute in the returned JSON structure. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRepositoryHook**
> DeleteRepositoryHook(ctx, projectKey, hookKey, repositorySlug)
Delete repository hook

Delete repository hook configuration for the supplied <strong>hookKey</strong> and <strong>repositorySlug</strong>  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRestriction1**
> DeleteRestriction1(ctx, projectKey, id, repositorySlug)
Delete a ref restriction

Deletes a restriction as specified by a restriction id.  The authenticated user must have <strong>REPO_ADMIN</strong> permission or higher to call this resource. Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The restriction id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteTag**
> DeleteTag(ctx, projectKey, name, repositorySlug)
Delete tag

Deletes a tag in the specified repository.  The authenticated user must have an effective <strong>REPO_WRITE</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **name** | **string**| The name of the tag to be deleted. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteWebhook1**
> DeleteWebhook1(ctx, projectKey, webhookId, repositorySlug)
Delete webhook

Delete a webhook for the repository specified via the URL.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| The ID of the webhook to be deleted. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DisableHook1**
> RestRepositoryHook DisableHook1(ctx, projectKey, hookKey, repositorySlug)
Disable repository hook

Disable a repository hook for this repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestRepositoryHook**](RestRepositoryHook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EditFile**
> RestCommit EditFile(ctx, path, projectKey, repositorySlug, optional)
Edit file

Update the content of path, on the given repository and branch.   This resource accepts PUT multipart form data, containing the file in a form-field named content.   An example <a href=\"http://curl.haxx.se/\">curl</a> request to update 'README.md' would be:  ```curl -X PUT -u username:password -F content=@README.md  -F 'message=Updated using file-edit REST API' -F branch=master -F  sourceCommitId=5636641a50b  http://example.com/rest/api/latest/projects/PROJECT_1/repos/repo_1/browse/README.md ```  - branch:  the branch on which the path should be modified or created - content: the full content of the file at path  - message: the message associated with this change, to be used as the commit message. Or null if the default message should be used. - sourceCommitId: the commit ID of the file before it was edited, used to identify if content has changed. Or null if this is a new file   The file can be updated or created on a new branch. In this case, the sourceBranch parameter should be provided to identify the starting point for the new branch and the branch parameter identifies the branch to create the new commit on.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The path of the file that is to be modified or created | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiEditFileOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiEditFileOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **branch** | **optional.**|  | 
 **content** | **optional.**|  | 
 **message** | **optional.**|  | 
 **sourceBranch** | **optional.**|  | 
 **sourceCommitId** | **optional.**|  | 

### Return type

[**RestCommit**](RestCommit.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EnableHook1**
> RestRepositoryHook EnableHook1(ctx, projectKey, hookKey, repositorySlug, optional)
Enable repository hook

Enable a repository hook for this repository and optionally apply new configuration.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.   A JSON document may be provided to use as the settings for the hook. These structure and validity of the document is decided by the plugin providing the hook.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiEnableHook1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiEnableHook1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **contentLength** | **optional.String**| The content length. | 

### Return type

[**RestRepositoryHook**](RestRepositoryHook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindBranches**
> InlineResponse2003 FindBranches(ctx, projectKey, repositorySlug, optional)
Get branches with ref change activities for repository

Retrieve a page of branches with ref change activities for a specific repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiFindBranchesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiFindBranchesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filterText** | **optional.String**| (optional) Partial match for a ref ID to filter minimal refs for | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2003**](inline_response_200_3.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindByCommit**
> InlineResponse2003 FindByCommit(ctx, projectKey, commitId, repositorySlug, optional)
Get branch

Gets the branch information associated with a single commit from a given repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commitId** | **string**|  | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiFindByCommitOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiFindByCommitOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2003**](inline_response_200_3.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindWebhooks1**
> FindWebhooks1(ctx, projectKey, repositorySlug, optional)
Find webhooks

Find webhooks in this repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiFindWebhooks1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiFindWebhooks1Opts struct
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

# **GetAllLabelsForRepository**
> RestLabel GetAllLabelsForRepository(ctx, projectKey, repositorySlug)
Get repository labels

Get all labels applied to the given repository.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestLabel**](RestLabel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetArchive**
> GetArchive(ctx, projectKey, repositorySlug, optional)
Stream archive of repository

Streams an archive of the repository's contents at the requested commit. If no `at=` commit is requested, an archive of the default branch is streamed.  The <code>filename=</code> query parameter may be used to specify the exact filename to include in the \"Content-Disposition\" header. If an explicit filename is not provided, one will be automatically generated based on what is being archived. Its format depends on the at= value:   - No <code>at=</code> commit:     &lt;slug&gt;-&lt;default-branch-name&gt;@&lt;commit&gt;.&lt;format&gt;;     e.g. example-master@43c2f8a0fe8.zip - <code>at=</code>sha: &lt;slug&gt;-&lt;at&gt;.&lt;format&gt;; e.g.     example-09bcbb00100cfbb5310fb6834a1d5ce6cac253e9.tar.gz - <code>at=</code>branchOrTag: &lt;slug&gt;-&lt;branchOrTag&gt;@&lt;commit&gt;.&lt;format&gt;;     e.g. example-feature@bbb225f16e1.tar       - If the branch or tag is qualified (e.g. refs/heads/master, the short name         (master) will be included in the filename     - If the branch or tag's <i>short name</i> includes slashes (e.g. release/4.6),         they will be converted to hyphens in the filename (release-4.5)     Archives may be requested in the following formats by adding the <code>format=</code> query parameter:   - zip: A zip file using standard compression (Default) - tar: An uncompressed tarball - tar.gz or tgz: A GZip-compressed tarball   The contents of the archive may be filtered by using the <code>path=</code> query parameter to specify paths to include. <code>path=</code> may be specified multiple times to include multiple paths.   The <code>prefix=</code> query parameter may be used to define a directory (or multiple directories) where the archive's contents should be placed. If the prefix does not end with /, one will be added automatically. The prefix is <i>always</i> treated as a directory; it is not possible to use it to prepend characters to the entries in the archive.   Archives of public repositories may be streamed by any authenticated or anonymous user. Streaming archives for non-public repositories requires an <i>authenticated user</i> with at least <b>REPO_READ</b> permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetArchiveOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetArchiveOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **path** | **optional.String**| Paths to include in the streamed archive; may be repeated to include multiple paths | 
 **filename** | **optional.String**| A filename to include the \&quot;Content-Disposition\&quot; header | 
 **at** | **optional.String**| The commit to stream an archive of; if not supplied, an archive of the default branch is streamed | 
 **prefix** | **optional.String**| A prefix to apply to all entries in the streamed archive; if the supplied prefix does not end with a trailing /, one will be added automatically | 
 **format** | **optional.String**| The format to stream the archive in; must be one of: zip, tar, tar.gz or tgz | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAttachment**
> GetAttachment(ctx, projectKey, attachmentId, repositorySlug, optional)
Get an attachment

Retrieve the attachment.  The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository that is associated to the attachment.  Range requests (see IETF RFC7233) are supported. However only a single range issupported. If multiple ranges are passed the ranges will be ignored and the entire content will be returned in the response.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **attachmentId** | **string**| the attachment ID | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiGetAttachmentOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetAttachmentOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **userAgent** | **optional.String**|  | 
 **range_** | **optional.String**|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAttachmentMetadata**
> RestAttachmentMetadata GetAttachmentMetadata(ctx, projectKey, attachmentId, repositorySlug)
Get attachment metadata

Retrieve the attachment metadata.  The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository that is associated to the attachment that has the attachment metadata.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **attachmentId** | **string**| the attachment ID | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

[**RestAttachmentMetadata**](RestAttachmentMetadata.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAutoDeclineSettings1**
> RestAutoDeclineSettings GetAutoDeclineSettings1(ctx, projectKey, repositorySlug)
Get auto decline settings

Retrieves the auto decline settings for the supplied repository. Project settings will be returned if no explicit settings have been set for the repository. In the case that there are no project settings, the default settings will be returned.  The authenticated user must have <strong>REPO_READ</strong> permission for this repository to call the resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

[**RestAutoDeclineSettings**](RestAutoDeclineSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetBranches**
> InlineResponse20033 GetBranches(ctx, projectKey, repositorySlug, optional)
Find branches

Retrieve the branches matching the supplied <strong>filterText</strong> param.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetBranchesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetBranchesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **boostMatches** | **optional.Bool**| Controls whether exact and prefix matches will be boosted to the top | 
 **orderBy** | **optional.String**| Ordering of refs either ALPHABETICAL (by name) or MODIFICATION (last updated) | 
 **details** | **optional.Bool**| Whether to retrieve plugin-provided metadata about each branch | 
 **filterText** | **optional.String**| The text to match on | 
 **base** | **optional.String**| Base branch or tag to compare each branch to (for the metadata providers that uses that information | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20033**](inline_response_200_33.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetChanges**
> InlineResponse20034 GetChanges(ctx, projectKey, commitId, repositorySlug, optional)
Get changes in commit

Retrieve a page of changes made in a specified commit.    <strong>Note:</strong> The implementation will apply a hard cap (<code>page.max.changes</code>) and it is not possible to request subsequent content when that cap is exceeded.    The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| The commit to retrieve changes for | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiGetChangesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetChangesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **withComments** | **optional.String**| &lt;code&gt;true&lt;/code&gt; to apply comment counts in the changes (the default); otherwise, &lt;code&gt;false&lt;/code&gt; to stream changes without comment counts | 
 **since** | **optional.String**| The commit to which &lt;code&gt;until&lt;/code&gt; should be compared to produce a page of changes. If not specified the commit&#x27;s first parent is assumed (if one exists) | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20034**](inline_response_200_34.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetChanges1**
> InlineResponse20034 GetChanges1(ctx, projectKey, repositorySlug, optional)
Get changes made in commit

Retrieve a page of changes made in a specified commit.   <strong>Note:</strong> The implementation will apply a hard cap ({@code page.max.changes}) and it is not possible to request subsequent content when that cap is exceeded.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetChanges1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetChanges1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **until** | **optional.String**| The commit to retrieve changes for | 
 **since** | **optional.String**| The commit to which &lt;code&gt;until&lt;/code&gt; should be compared to produce a page of changes. If not specified the commit&#x27;s first parent is assumed (if one exists) | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20034**](inline_response_200_34.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetComment**
> RestComment GetComment(ctx, projectKey, commentId, commitId, repositorySlug)
Get a commit comment

Retrieves a commit discussion comment.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that the commit is in to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commentId** | **string**| The ID of the comment to retrieve | 
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetComments**
> InlineResponse20036 GetComments(ctx, projectKey, commitId, repositorySlug, optional)
Search for commit comments

Retrieves the commit discussion comments that match the specified search criteria.  It is possible to retrieve commit discussion comments that are anchored to a range of commits by providing the sinceId that the comments anchored from.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that the commit is in to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiGetCommentsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetCommentsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **path** | **optional.String**| The path to the file on which comments were made | 
 **since** | **optional.String**| For a merge commit, a parent can be provided to specify which diff the comments are on. For a commit range, a sinceId can be provided to specify where the comments are anchored from. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20036**](inline_response_200_36.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetCommit**
> RestCommit GetCommit(ctx, projectKey, commitId, repositorySlug, optional)
Get commit by ID

Retrieve a single commit <i>identified by its ID</i>. In general, that ID is a SHA1. <u>From 2.11, ref names like \"refs/heads/master\" are no longer accepted by this resource.</u>  The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| The commit ID to retrieve | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiGetCommitOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetCommitOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **path** | **optional.String**| An optional path to filter the commit by. If supplied the details returned &lt;i&gt;may not&lt;/i&gt; be for the specified commit. Instead, starting from the specified commit, they will be the details for the first commit affecting the specified path. | 

### Return type

[**RestCommit**](RestCommit.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetCommits**
> InlineResponse20035 GetCommits(ctx, projectKey, repositorySlug, optional)
Get commits

Retrieve a page of commits from a given starting commit or \"between\" two commits. If no explicit commit is specified, the tip of the repository's default branch is assumed. commits may be identified by branch or tag name or by ID. A path may be supplied to restrict the returned commits to only those which affect that path.   The authenticated user must have <b>REPO_READ</b> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiGetCommitsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetCommitsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **avatarScheme** | **optional.String**| The desired scheme for the avatar URL. If the parameter is not present URLs will use the same scheme as this request | 
 **path** | **optional.String**| An optional path to filter commits by | 
 **withCounts** | **optional.String**| Optionally include the total number of commits and total number of unique authors | 
 **followRenames** | **optional.String**| If &lt;code&gt;true&lt;/code&gt;, the commit history of the specified file will be followed past renames. Only valid for a path to a single file. | 
 **until** | **optional.String**| The commit ID (SHA1) or ref (inclusively) to retrieve commits before | 
 **avatarSize** | **optional.String**| If present the service adds avatar URLs for commit authors. Should be an integer specifying the desired size in pixels. If the parameter is not present, avatar URLs will not be set | 
 **since** | **optional.String**| The commit ID or ref (exclusively) to retrieve commits after | 
 **merges** | **optional.String**| If present, controls how merge commits should be filtered. Can be either &lt;code&gt;exclude&lt;/code&gt;, to exclude merge commits, &lt;code&gt;include&lt;/code&gt;, to include both merge commits and non-merge commits or &lt;code&gt;only&lt;/code&gt;, to only return merge commits. | 
 **ignoreMissing** | **optional.String**| &lt;code&gt;true&lt;/code&gt; to ignore missing commits, &lt;code&gt;false&lt;/code&gt; otherwise | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20035**](inline_response_200_35.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetConfigurations1**
> InlineResponse20031 GetConfigurations1(ctx, projectKey, repositorySlug, optional)
Get hook scripts

Return a page of hook scripts configured for the specified repository.   This endpoint requires **REPO_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetConfigurations1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetConfigurations1Opts struct
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

# **GetContent**
> GetContent(ctx, projectKey, repositorySlug, optional)
Get file content at revision

Retrieve a page of content for a file path at a specified revision.   Responses from this endpoint vary widely depending on the query parameters. The example JSON is for a request that does not use size, type, blame or noContent.   1. size will return a response like {\"size\":10000} 2. type will return a response like {\"type\":\"FILE\"}, where possible values are    \"DIRECTORY\", \"FILE\" and \"SUBMODULE\" 3. blame <i>without</i> noContent will include blame for the lines of    content returned on the page 4. blame <i>with</i> noContent will omit file contents and only return    blame for the requested lines 5. noContent without blame is ignored and does nothing   The various parameters are \"processed\" in the above order. That means ?size=true&amp;type=truewill return a size response, not a type one; the type parameter will be ignored.   The blame and noContent query parameters are handled differently from size and type. For blame and noContent, the <i>presence</i> of the parameter implies \"true\" if no value is specified; size and and type both require an explicit=true or they're treated as \"false\".   - ?blame is the same as ?blame=true - ?blame&amp;noContent is the same as ?blame=true&amp;noContent=true - ?size is the same as ?size=false - ?type is the same as ?type=false   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetContentOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetContentOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **noContent** | **optional.String**| If blame&amp;amp;noContent only the blame is retrieved instead of the contents | 
 **at** | **optional.String**| The commit ID or ref to retrieve the content for | 
 **size** | **optional.String**| If true only the size will be returned for the file path instead of the contents | 
 **blame** | **optional.String**| If present and not equal to &#x27;false&#x27;, the blame will be returned for the file as well | 
 **type_** | **optional.String**| If true only the type will be returned for the file path instead of the contents | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetContent1**
> GetContent1(ctx, path, projectKey, repositorySlug, optional)
Get file content

Retrieve a page of content for a file path at a specified revision.   Responses from this endpoint vary widely depending on the query parameters. The example JSON is for a request that does not use size, type, blame or noContent.   1. size will return a response like {\"size\":10000} 2. type will return a response like {\"type\":\"FILE\"}, where possible values are    \"DIRECTORY\", \"FILE\" and \"SUBMODULE\" 3. blame <i>without</i> noContent will include blame for the lines of    content returned on the page 4. blame <i>with</i> noContent will omit file contents and only return    blame for the requested lines 5. noContent without blame is ignored and does nothing   The various parameters are \"processed\" in the above order. That means ?size=true&amp;type=truewill return a size response, not a type one; the type parameter will be ignored.   The blame and noContent query parameters are handled differently from size and type. For blame and noContent, the <i>presence</i> of the parameter implies \"true\" if no value is specified; size and and type both require an explicit=true or they're treated as \"false\".   - ?blame is the same as ?blame=true - ?blame&amp;noContent is the same as ?blame=true&amp;noContent=true - ?size is the same as ?size=false - ?type is the same as ?type=false   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The file path to retrieve content from | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetContent1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetContent1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **noContent** | **optional.String**| If blame&amp;amp;noContent only the blame is retrieved instead of the contents | 
 **at** | **optional.String**| The commit ID or ref to retrieve the content for | 
 **size** | **optional.String**| If true only the size will be returned for the file path instead of the contents | 
 **blame** | **optional.String**| If present and not equal to &#x27;false&#x27;, the blame will be returned for the file as well | 
 **type_** | **optional.String**| If true only the type will be returned for the file path instead of the contents | 

### Return type

 (empty response body)

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

# **GetLatestInvocation1**
> RestDetailedInvocation GetLatestInvocation1(ctx, projectKey, webhookId, repositorySlug, optional)
Get last webhook invocation details

Get the latest invocations for a specific webhook.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| ID of the webhook | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetLatestInvocation1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetLatestInvocation1Opts struct
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

# **GetPullRequestSettings1**
> RestRepositoryPullRequestSettings GetPullRequestSettings1(ctx, projectKey, repositorySlug)
Get pull request settings

Retrieve the pull request settings for the context repository.   The authenticated user must have <strong>REPO_READ</strong> permission for the context repository to call this resource.   This resource will call all RestFragments that are registered with the key <strong>bitbucket.repository.settings.pullRequests</strong>. If any fragment fails validations by returning a non-empty Map of errors, then no fragments will execute.   The property keys for the settings that are bundled with the application are   - mergeConfig - the merge strategy configuration for pull requests - requiredApprovers - (Deprecated, please use com.atlassian.bitbucket.server.bundled-hooks.requiredApproversMergeHook instead) the number of approvals required on a pull request for it to be mergeable, or 0 if the merge check is disabled - com.atlassian.bitbucket.server.bundled-hooks.requiredApproversMergeHook - the merge check configuration for required approvers - requiredAllApprovers - whether or not all approvers must approve a pull request for it to be mergeable - requiredAllTasksComplete - whether or not all tasks on a pull request need to be completed for it to be mergeable - requiredSuccessfulBuilds - (Deprecated, please use com.atlassian.bitbucket.server.bitbucket-build.requiredBuildsMergeCheck instead) the number of successful builds on a pull request for it to be mergeable, or 0 if the merge check is disabled - com.atlassian.bitbucket.server.bitbucket-build.requiredBuildsMergeCheck - the merge check configuration for required builds   

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestRepositoryPullRequestSettings**](RestRepositoryPullRequestSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRefChangeActivity**
> InlineResponse20041 GetRefChangeActivity(ctx, projectKey, repositorySlug, optional)
Get ref change activity

Retrieve a page of repository ref change activity.   The authenticated user must have <strong>REPO_ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetRefChangeActivityOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetRefChangeActivityOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **ref** | **optional.String**| (optional) exact match for a ref ID to filter ref change activity for | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20041**](inline_response_200_41.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositories1**
> InlineResponse20029 GetRepositories1(ctx, optional)
Search for repositories

Retrieve a page of repositories based on query parameters that control the search. See the documentation of the parameters for more details.   This resource is anonymously accessible.   <b>Note on permissions.</b> In absence of the <code>permission</code> query parameter the implicit 'read' permission is assumed. Please note that this permission is lower than the <tt>REPO_READ</tt> permission rather than being equal to it. The implicit 'read' permission for a given repository is assigned to any user that has any of the higher permissions, such as <tt>REPO_READ</tt>, as well as to anonymous users if the repository is marked as public. The important implication of the above is that an anonymous request to this resource with a permission level <tt>REPO_READ</tt> is guaranteed to receive an empty list of repositories as a result. For anonymous requests it is therefore recommended to not specify the <tt>permission</tt> parameter at all.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***RepositoryApiGetRepositories1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetRepositories1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **archived** | **optional.String**| (optional) if specified, this will limit the resulting repository list to ones whose are &lt;tt&gt;ACTIVE&lt;/tt&gt;, &lt;tt&gt;ARCHIVED&lt;/tt&gt; or &lt;tt&gt;ALL&lt;/tt&gt; for both. The match performed is case-insensitive. This filter defaults to &lt;tt&gt;ACTIVE&lt;/tt&gt; when not set. &lt;em&gt;Available since 8.0&lt;/em&gt; | 
 **projectname** | **optional.String**| (optional) if specified, this will limit the resulting repository list to ones whose project&#x27;s name matches this parameter&#x27;s value. The match performed is case-insensitive and any leading and/or trailing whitespace characters on the &lt;code&gt;projectname&lt;/code&gt; parameter will be stripped. | 
 **projectkey** | **optional.String**| (optional) if specified, this will limit the resulting repository list to ones whose project&#x27;s key matches this parameter&#x27;s value. The match performed is case-insensitive and any leading  and/or trailing whitespace characters on the &lt;code&gt;projectKey&lt;/code&gt; parameter will be stripped. &lt;em&gt;Available since 8.0&lt;/em&gt; | 
 **visibility** | **optional.String**| (optional) if specified, this will limit the resulting repository list based on the repositories visibility. Valid values are &lt;em&gt;public&lt;/em&gt; or &lt;em&gt;private&lt;/em&gt;. | 
 **name** | **optional.String**| (optional) if specified, this will limit the resulting repository list to ones whose name matches this parameter&#x27;s value. The match performed is case-insensitive and any leading and/or trailing whitespace characters on the &lt;code&gt;name&lt;/code&gt; parameter will be stripped. | 
 **permission** | **optional.String**| (optional) if specified, it must be a valid repository permission level name and will limit the resulting repository list to ones that the requesting user has the specified permission level to. If not specified, the default implicit &#x27;read&#x27; permission level will be assumed. The currently supported explicit permission values are &lt;tt&gt;REPO_READ&lt;/tt&gt;, &lt;tt&gt;REPO_WRITE&lt;/tt&gt; and &lt;tt&gt;REPO_ADMIN&lt;/tt&gt;. | 
 **state** | **optional.String**| (optional) if specified, it must be a valid repository state name and will limit the resulting repository list to ones that are in the specified state. The currently supported explicit state values are &lt;tt&gt;AVAILABLE&lt;/tt&gt;, &lt;tt&gt;INITIALISING&lt;/tt&gt; and &lt;tt&gt;INITIALISATION_FAILED&lt;/tt&gt;.&lt;br&gt; &lt;em&gt;Available since 5.13&lt;/em&gt; | 
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

# **GetRepositoriesRecentlyAccessed**
> InlineResponse20029 GetRepositoriesRecentlyAccessed(ctx, optional)
Get recently accessed repositories

Retrieve a page of recently accessed repositories for the currently authenticated user.   Repositories are ordered from most recently to least recently accessed. <p>Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***RepositoryApiGetRepositoriesRecentlyAccessedOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetRepositoriesRecentlyAccessedOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **permission** | **optional.String**| (optional) If specified, it must be a valid repository permission level name and will limit the resulting repository list to ones that the requesting user has the specified permission level to. If not specified, the default &lt;code&gt;REPO_READ&lt;/code&gt; permission level will be assumed. | [default to REPO_READ]
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

# **GetRepositoryHook1**
> RestRepositoryHook GetRepositoryHook1(ctx, projectKey, hookKey, repositorySlug)
Get repository hook

Retrieve a repository hook for this repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestRepositoryHook**](RestRepositoryHook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositoryHooks1**
> InlineResponse20044 GetRepositoryHooks1(ctx, projectKey, repositorySlug, optional)
Get repository hooks

Retrieve a page of repository hooks for this repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetRepositoryHooks1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetRepositoryHooks1Opts struct
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

# **GetRestriction1**
> RestRefRestriction GetRestriction1(ctx, projectKey, id, repositorySlug)
Get a ref restriction

Returns a restriction as specified by a restriction id.   The authenticated user must have <strong>REPO_ADMIN</strong> permission or higher to call this resource. Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The restriction id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestRefRestriction**](RestRefRestriction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRestrictions1**
> InlineResponse20013 GetRestrictions1(ctx, projectKey, repositorySlug, optional)
Search for ref restrictions

Search for restrictions using the supplied parameters.  The authenticated user must have <strong>REPO_ADMIN</strong> permission or higher to call this resource. Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetRestrictions1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetRestrictions1Opts struct
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

# **GetSettings1**
> ExampleSettings GetSettings1(ctx, projectKey, hookKey, repositorySlug)
Get repository hook settings

Retrieve the settings for a repository hook for this repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**ExampleSettings**](ExampleSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetStatus**
> RestRefSyncStatus GetStatus(ctx, projectKey, repositorySlug, optional)
Get synchronization status

Retrieves the synchronization status for the specified repository. In addition to listing refs which cannot be synchronized, if any, the status also provides the timestamp for the most recent synchronization and indicates whether synchronization is available and enabled. If \"?at\" is specified in the URL, the synchronization status for the specified ref is returned, rather than the complete repository status.  The authenticated user must have <b>REPO_READ</b> permission for the repository, or it must be public if the request is anonymous. Additionally, after synchronization is enabled for a repository, meaning synchronization was available at that time, permission changes and other actions can cause it to become unavailable. Even when synchronization is enabled, if it is no longer available for the repository it will not be performed.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetStatusOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetStatusOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **at** | **optional.String**| Retrieves the synchronization status for the specified ref within the repository, rather than for the entire repository | 

### Return type

[**RestRefSyncStatus**](RestRefSyncStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetTag**
> RestTag GetTag(ctx, projectKey, name, repositorySlug)
Get tag

Retrieve a tag in the specified repository.   The authenticated user must have <strong>REPO_READ</strong> permission for the context repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **name** | **string**| The name of the tag to be retrieved. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestTag**](RestTag.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetTags**
> InlineResponse20046 GetTags(ctx, projectKey, repositorySlug, optional)
Find tag

Retrieve the tags matching the supplied <strong>filterText</strong> param.   The authenticated user must have <strong>REPO_READ</strong> permission for the context repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetTagsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetTagsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **orderBy** | **optional.String**| Ordering of refs either ALPHABETICAL (by name) or MODIFICATION (last updated) | 
 **filterText** | **optional.String**| The text to match on. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20046**](inline_response_200_46.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetWebhook1**
> RestWebhook GetWebhook1(ctx, projectKey, webhookId, repositorySlug, optional)
Get webhook

Get a webhook by ID.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| ID of the webhook | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiGetWebhook1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiGetWebhook1Opts struct
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

# **React**
> RestUserReaction React(ctx, projectKey, commentId, commitId, emoticon, repositorySlug)
React to a comment

Add an emoticon reaction to a comment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The comment id | 
  **commitId** | **string**| The commit id | 
  **emoticon** | **string**| The emoticon to add | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestUserReaction**](RestUserReaction.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RemoveConfiguration1**
> RemoveConfiguration1(ctx, projectKey, scriptId, repositorySlug)
Remove a hook script

Removes the hook script from the set of hook scripts configured to run in the repository.   This endpoint requires **REPO_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **scriptId** | **string**| The ID of the hook script | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RemoveLabel**
> RemoveLabel(ctx, projectKey, labelName, repositorySlug)
Remove repository label

Remove label that is applied to the given repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **labelName** | **string**| The label to remove | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SaveAttachmentMetadata**
> SaveAttachmentMetadata(ctx, projectKey, attachmentId, repositorySlug, optional)
Save attachment metadata

Save attachment metadata.  The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository that is associated to the attachment that has the attachment metadata.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **attachmentId** | **string**| the attachment ID | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiSaveAttachmentMetadataOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSaveAttachmentMetadataOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of string**](string.md)| The attachment metadata can be any valid JSON content | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SearchWebhooks**
> SearchWebhooks(ctx, projectKey, repositorySlug, optional)
Search webhooks

Search webhooks in this repository and parent project. This endpoint returns a superset of the results returned by the /webhooks endpoint because it allows filtering by project scope too, not just repository webhooks.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiSearchWebhooksOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSearchWebhooksOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **scopeType** | **optional.String**| Scopes to filter by. This parameter can be specified once e.g. \&quot;scopeType&#x3D;repository\&quot;, or twice e.g. \&quot;scopeType&#x3D;repository&amp;scopeType&#x3D;project\&quot;, to filter by more than one scope level.  | 
 **event** | **optional.String**| List of &lt;code&gt;com.atlassian.webhooks.WebhookEvent&lt;/code&gt; ids to filter for | 
 **statistics** | **optional.Bool**| &lt;code&gt;true&lt;/code&gt; if statistics should be provided for all found webhooks | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetAutoDeclineSettings1**
> RestAutoDeclineSettings SetAutoDeclineSettings1(ctx, projectKey, repositorySlug, optional)
Create auto decline settings

Creates or updates the auto decline settings for the supplied repository.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for this repository to call the resource

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiSetAutoDeclineSettings1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSetAutoDeclineSettings1Opts struct
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

# **SetConfiguration1**
> RestHookScriptConfig SetConfiguration1(ctx, projectKey, scriptId, repositorySlug, optional)
Create/update a hook script

Creates/updates the hook script configuration for the provided hook script and repository.   This endpoint requires **REPO_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **scriptId** | **string**| The ID of the hook script | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiSetConfiguration1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSetConfiguration1Opts struct
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
 **optional** | ***RepositoryApiSetDefaultBranch1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSetDefaultBranch1Opts struct
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

# **SetEnabled**
> RestRefSyncStatus SetEnabled(ctx, projectKey, repositorySlug, optional)
Disable synchronization

Enables or disables synchronization for the specified repository. When synchronization is enabled, branches within the repository are immediately synchronized and the status is updated with the outcome. That initial synchronization is performed before the REST request returns, allowing it to return the updated status.  The authenticated user must have <b>REPO_ADMIN</b> permission for the specified repository. Anonymous users cannot manage synchronization, even on public repositories. Additionally, synchronization must be available for the specified repository. Synchronization is only available if:  - The repository is a fork, since its origin is used as upstream - The owning user still has access to the fork's origin,  if the repository is a <i>personalfork</i>

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiSetEnabledOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSetEnabledOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestRefSyncStatus**](RestRefSyncStatus.md)|  | 

### Return type

[**RestRefSyncStatus**](RestRefSyncStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetSettings1**
> ExampleSettings SetSettings1(ctx, projectKey, hookKey, repositorySlug, optional)
Update repository hook settings

Modify the settings for a repository hook for this repository.   The service will reject any settings which are too large, the current limit is 32KB once serialized.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.   A JSON document can be provided to use as the settings for the hook. These structure and validity of the document is decided by the plugin providing the hook.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **hookKey** | **string**| The hook key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiSetSettings1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSetSettings1Opts struct
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

# **Stream**
> ExampleFiles Stream(ctx, projectKey, repositorySlug, optional)
Stream files

Streams files from the repository's root with the last commit to modify each file. Commit modifications are traversed starting from the <code>at</code> commit or, if not specified, from the tip of the default branch.  Unless the repository is public, the authenticated user must have <b>REPO_READ</b> access to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiStreamOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **at** | **optional.String**| The commit to use as the starting point when listing files and calculating modifications | 

### Return type

[**ExampleFiles**](ExampleFiles.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Stream1**
> ExampleFiles Stream1(ctx, path, projectKey, repositorySlug, optional)
Stream files with last modified commit in path

Streams files in the requested <code>path</code> with the last commit to modify each file. Commit modifications are traversed starting from the <code>at</code> commit or, if not specified, from the tip of the default branch.  Unless the repository is public, the authenticated user must have <b>REPO_READ</b> access to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The path within the repository whose files should be streamed | 
  **projectKey** | **string**| The project key | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiStream1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStream1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **at** | **optional.String**| The commit to use as the starting point when listing files and calculating modifications | 

### Return type

[**ExampleFiles**](ExampleFiles.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamChanges**
> InlineResponse20034 StreamChanges(ctx, projectKey, repositorySlug, optional)
Compare commits

Gets the file changes available in the <code> from</code> commit but not in the <code> to</code> commit.   If either the <code> from</code> or <code> to</code> commit are not specified, they will be replaced by the default branch of their containing repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamChangesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamChangesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fromRepo** | **optional.String**| an optional parameter specifying the source repository containing the source commit if that commit is not present in the current repository; the repository can be specified by either its ID &lt;em&gt;fromRepo&#x3D;42&lt;/em&gt; or by its project key plus its repo slug separated by a slash: &lt;em&gt;fromRepo&#x3D;projectKey/repoSlug&lt;/em&gt; | 
 **from** | **optional.String**| the source commit (can be a partial/full commit ID or qualified/unqualified ref name) | 
 **to** | **optional.String**| the target commit (can be a partial/full commit ID or qualified/unqualified ref name) | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20034**](inline_response_200_34.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamCommits**
> InlineResponse20035 StreamCommits(ctx, projectKey, repositorySlug, optional)
Get accessible commits

Gets the commits accessible from the <code>from</code> commit but not in the <code>to</code> commit.  If either the <code>from</code> or <code>to</code> commit are not specified, they will be replaced by the default branch of their containing repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamCommitsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamCommitsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fromRepo** | **optional.String**| an optional parameter specifying the source repository containing the source commit if that commit is not present in the current repository; the repository can be specified by either its ID &lt;em&gt;fromRepo&#x3D;42&lt;/em&gt; or by its project key plus its repo slug separated by a slash: &lt;em&gt;fromRepo&#x3D;projectKey/repoSlug&lt;/em&gt; | 
 **from** | **optional.String**| the source commit (can be a partial/full commit ID or qualified/unqualified ref name) | 
 **to** | **optional.String**| the target commit (can be a partial/full commit ID or qualified/unqualified ref name) | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20035**](inline_response_200_35.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamDiff**
> RestDiff StreamDiff(ctx, commitId, repositorySlug, path, projectKey, optional)
Get diff between revisions

Retrieve the diff between two provided revisions.  To stream a raw text representation of the diff, this endpoint can be called with the request header 'Accept: text/plain'.   Note:</strong> This resource is currently <i>not paged</i>. The server will internally apply a hard cap to the streamed lines, and it is not possible to request subsequent pages if that cap is exceeded. In the event that the cap is reached, the diff will be cut short and one or more {@code truncated} flags will be set to true on the \"segments\", \"hunks\" and \"diffs\" properties, as well as the top-level object, in the returned JSON response.  The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 
  **path** | **string**| The path to the file which should be diffed (optional) | 
  **projectKey** | **string**| The project key | 
 **optional** | ***RepositoryApiStreamDiffOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamDiffOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **srcPath** | **optional.String**| The source path for the file, if it was copied, moved or renamed | 
 **avatarSize** | **optional.String**| If present the service adds avatar URLs for comment authors where the provided value specifies the desired avatar size in pixels. Not applicable if streaming raw diff | 
 **filter** | **optional.String**| Text used to filter files and lines (optional). Not applicable if streaming raw diff | 
 **avatarScheme** | **optional.String**| The security scheme for avatar URLs. If the scheme is not present then it is inherited from the request. It can be set to \&quot;https\&quot; to force the use of secure URLs. Not applicable if streaming raw diff | 
 **contextLines** | **optional.String**| The number of context lines to include around added/removed lines in the diff.Not applicable if streaming raw diff | 
 **autoSrcPath** | **optional.String**| &lt;code&gt;true&lt;/code&gt; to automatically try to find the source path when it&#x27;s not provided, &lt;code&gt;false&lt;/code&gt; otherwise. Requires the path to be provided. | 
 **whitespace** | **optional.String**| Optional whitespace flag which can be set to ignore-all | 
 **withComments** | **optional.String**| &lt;code&gt;true&lt;/code&gt; to embed comments in the diff (the default); otherwise &lt;code&gt;false&lt;/code&gt; to stream the diff without comments. Not applicable if streaming raw diff | 
 **since** | **optional.String**| The base revision to diff from. If omitted the parent revision of the until revision is used | 

### Return type

[**RestDiff**](RestDiff.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamDiff1**
> InlineResponse20037 StreamDiff1(ctx, path, projectKey, repositorySlug, optional)
Get diff between commits

Gets a diff of the changes available in the <code>from</code> commit but not in the <code> to</code> commit.  If either the <code> from</code> or <code> to</code> commit are not specified, they will be replaced by the default branch of their containing repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| the path to the file to diff (optional) | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamDiff1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamDiff1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **contextLines** | **optional.String**| an optional number of context lines to include around each added or removed lines in the diff | 
 **fromRepo** | **optional.String**| an optional parameter specifying the source repository containing the source commit if that commit is not present in the current repository; the repository can be specified by either its ID &lt;em&gt;fromRepo&#x3D;42&lt;/em&gt; or by its project key plus its repo slug separated by a slash: &lt;em&gt;fromRepo&#x3D;projectKey/repoSlug&lt;/em&gt; | 
 **srcPath** | **optional.String**| source path | 
 **from** | **optional.String**| the source commit (can be a partial/full commit ID or qualified/unqualified ref name) | 
 **to** | **optional.String**| the target commit (can be a partial/full commit ID or qualified/unqualified ref name) | 
 **whitespace** | **optional.String**| an optional whitespace flag which can be set to &lt;code&gt;ignore-all&lt;/code&gt; | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20037**](inline_response_200_37.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamFiles**
> InlineResponse20038 StreamFiles(ctx, path, projectKey, repositorySlug, optional)
Get files in directory

Retrieve a page of files from particular directory of a repository. The search is done recursively, so all files from any sub-directory of the specified directory will be returned.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The directory to list files for. | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamFilesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamFilesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **at** | **optional.String**| The commit ID or ref (e.g. a branch or tag) to list the files at. If not specified the default branch will be used instead. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20038**](inline_response_200_38.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamFiles1**
> InlineResponse20038 StreamFiles1(ctx, projectKey, repositorySlug, optional)
Get files in directory

Retrieve a page of files from particular directory of a repository. The search is done recursively, so all files from any sub-directory of the specified directory will be returned.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamFiles1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamFiles1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **at** | **optional.String**| The commit ID or ref (e.g. a branch or tag) to list the files at. If not specified the default branch will be used instead. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20038**](inline_response_200_38.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamPatch**
> StreamPatch(ctx, projectKey, repositorySlug, optional)
Get patch content at revision

Retrieve the patch content for a repository at a specified revision.   Cache headers are added to the response (only if full commit hashes are used, not in the case of short hashes).   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamPatchOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamPatchOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **until** | **optional.String**| The target revision from which to generate the patch (required) | 
 **allAncestors** | **optional.String**| indicates whether or not to generate a patch which includes all the ancestors of the &#x27;until&#x27; revision. If true, the value provided by &#x27;since&#x27; is ignored. | 
 **since** | **optional.String**| The base revision from which to generate the patch. This is only applicable when &#x27;allAncestors&#x27; is false. If omitted the patch will represent one single commit, the &#x27;until&#x27;. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamRaw**
> StreamRaw(ctx, path, projectKey, repositorySlug, optional)
Get raw content of a file at revision

Retrieve the raw content for a file path at a specified revision.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The file path to retrieve content from | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamRawOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamRawOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **at** | **optional.String**| A specific commit or ref to retrieve the raw content at, or the default branch if not specified | 
 **markup** | **optional.String**| If present or \&quot;true\&quot;, triggers the raw content to be markup-rendered and returned as HTML; otherwise, if not specified, or any value other than \&quot;true\&quot;, the content is streamed without markup | 
 **htmlEscape** | **optional.String**| (Optional) true if HTML should be escaped in the input markup, false otherwise. If not specified, the value of the markup.render.html.escape property, which is true by default, will be used | 
 **includeHeadingId** | **optional.String**| (Optional) true if headings should contain an ID based on the heading content. If not specified, the value of the markup.render.headerids property, which is false by default, will be used | 
 **hardwrap** | **optional.String**| (Optional) Whether the markup implementation should convert newlines to breaks. If not specified, the value of the markup.render.hardwrap property, which is true by default, will be used | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamRawDiff**
> StreamRawDiff(ctx, projectKey, repositorySlug, optional)
Get raw diff for path

Stream the raw diff between two provided revisions.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamRawDiffOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamRawDiffOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contextLines** | **optional.String**| The number of context lines to include around added/removed lines in the diff | 
 **srcPath** | **optional.String**| The source path for the file, if it was copied, moved or renamed | 
 **until** | **optional.String**| The target revision to diff to (required) | 
 **whitespace** | **optional.String**| Optional whitespace flag which can be set to &lt;code&gt;ignore-all&lt;/code&gt; | 
 **since** | **optional.String**| The base revision to diff from. If omitted the parent revision of the until revision is used | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamRawDiff1**
> StreamRawDiff1(ctx, path, projectKey, repositorySlug, optional)
Get raw diff for path

Stream the raw diff between two provided revisions.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The path to the file which should be diffed (required) | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiStreamRawDiff1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiStreamRawDiff1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **contextLines** | **optional.String**| The number of context lines to include around added/removed lines in the diff | 
 **srcPath** | **optional.String**| The source path for the file, if it was copied, moved or renamed | 
 **until** | **optional.String**| The target revision to diff to (required) | 
 **whitespace** | **optional.String**| Optional whitespace flag which can be set to &lt;code&gt;ignore-all&lt;/code&gt; | 
 **since** | **optional.String**| The base revision to diff from. If omitted the parent revision of the until revision is used | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Synchronize**
> RestRejectedRef Synchronize(ctx, projectKey, repositorySlug, optional)
Manual synchronization

Allows developers to apply a manual operation to bring a ref back in sync with upstream when it becomes out of sync due to conflicting changes. The following actions are supported:  - <tt>MERGE</tt>: Merges in commits from the upstream ref. After applying this action, the   synchronized ref will be <tt>AHEAD</tt> (as it still includes commits that do not exist   upstream.    - This action is only supported for <tt>DIVERGED</tt> refs    - If a \"commitMessage\" is provided in the context, it will be used on the merge commit.      Otherwise a default message is used. - <tt>DISCARD</tt>: <i>Throws away</i> local changes in favour of those made upstream. This is a   <i>destructive</i> operation where commits in the local repository are lost.    - No context entries are supported for this action    - If the upstream ref has been deleted, the local ref is deleted as well    - Otherwise, the local ref is updated to reference the same commit as upstream, even if      the update is not fast-forward (similar to a forced push)   The authenticated user must have <b>REPO_WRITE</b> permission for the specified repository. Anonymous users cannot synchronize refs, even on public repositories. Additionally, synchronization must be <i>enabled</i> and <i>available</i> for the specified repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiSynchronizeOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiSynchronizeOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestRefSyncRequest**](RestRefSyncRequest.md)|  | 

### Return type

[**RestRejectedRef**](RestRejectedRef.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UnReact**
> UnReact(ctx, projectKey, commentId, commitId, emoticon, repositorySlug)
Remove a reaction from comment

Remove an emoticon reaction from a comment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The comment id | 
  **commitId** | **string**| The commit id | 
  **emoticon** | **string**| The emoticon to remove | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Unwatch**
> Unwatch(ctx, projectKey, commitId, repositorySlug)
Stop watching commit

Remove the authenticated user as a watcher for the specified commit.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository containing the commit to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Unwatch2**
> Unwatch2(ctx, projectKey, repositorySlug)
Stop watching repository

Remove the authenticated user as a watcher for the specified repository.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository to call this resource.

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

# **UpdateComment**
> RestComment UpdateComment(ctx, projectKey, commentId, commitId, repositorySlug, optional)
Update a commit comment

Update a comment, with the following restrictions:  - only the author of the comment may update the <i>text</i> of the comment - only the author of the comment or repository admins and above may update the other   fields of a comment   <strong>Note:</strong> the supplied supplied JSON object must contain a <code>version</code> that must match the server's version of the comment or the update will fail. To determine the current version of the comment, the comment should be fetched from the server prior to the update. Look for the 'version' attribute in the returned JSON structure.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that the commit is in to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commentId** | **string**| The ID of the comment to retrieve | 
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***RepositoryApiUpdateCommentOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiUpdateCommentOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **body** | [**optional.Interface of RestComment**](RestComment.md)| The comment to update | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdatePullRequestSettings1**
> RestRepositoryPullRequestSettings UpdatePullRequestSettings1(ctx, projectKey, repositorySlug, optional)
Update pull request settings

Update the pull request settings for the context repository.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the context repository to call this resource.   This resource will call all RestFragments that are registered with the key <strong>bitbucket.repository.settings.pullRequests</strong>. If any fragment fails validations by returning a non-empty Map of errors, then no fragments will execute.   Only the settings that should be updated need to be included in the request.   The property keys for the settings that are bundled with the application are   - mergeConfig - the merge strategy configuration for pull requests - requiredApprovers - (Deprecated, please use com.atlassian.bitbucket.server.bundled-hooks.requiredApproversMergeHook instead) the number of approvals required on a pull request for it to be mergeable, or 0 to disable the merge check - com.atlassian.bitbucket.server.bundled-hooks.requiredApproversMergeHook - a json map containing the keys 'enabled' (a boolean to enable or disable this merge check) and 'count' (an integer to set the number of required approvals) - requiredAllApprovers - whether or not all approvers must approve a pull request for it to be mergeable - requiredAllTasksComplete - whether or not all tasks on a pull request need to be completed for it to be mergeable - requiredSuccessfulBuilds - (Deprecated, please use com.atlassian.bitbucket.server.bitbucket-build.requiredBuildsMergeCheck instead) the number of successful builds on a pull request for it to be mergeable, or 0 to disable the merge check - com.atlassian.bitbucket.server.bitbucket-build.requiredBuildsMergeCheck - a json map containing the keys 'enabled' (a boolean to enable or disable this merge check) and 'count' (an integer to set the number of required builds)   <strong>Merge strategy configuration deletion:</strong>  An explicitly set pull request merge strategy configuration can be deleted by POSTing a document with an empty \"mergeConfig\" attribute. i.e:    ```{      \"mergeConfig\": {      }  }  ```  Upon completion of this request, the effective configuration will be:   - The configuration set for this repository's SCM type as set at the project level, if present, otherwise - the configuration set for this repository's SCM type as set at the instance level, if present, otherwise - the default configuration for this repository's SCM type   

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiUpdatePullRequestSettings1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiUpdatePullRequestSettings1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestRepositoryPullRequestSettings**](RestRepositoryPullRequestSettings.md)| The updated settings. | 

### Return type

[**RestRepositoryPullRequestSettings**](RestRepositoryPullRequestSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateWebhook1**
> RestWebhook UpdateWebhook1(ctx, projectKey, webhookId, repositorySlug, optional)
Update webhook

Update an existing webhook.   The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **webhookId** | **string**| Id of the existing webhook | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiUpdateWebhook1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiUpdateWebhook1Opts struct
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

# **Watch**
> Watch(ctx, projectKey, commitId, repositorySlug)
Watch commit

Add the authenticated user as a watcher for the specified commit.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository containing the commit to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| The &lt;i&gt;full ID&lt;/i&gt; of the commit within the repository | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Watch2**
> Watch2(ctx, projectKey, repositorySlug, optional)
Watch repository

Add the authenticated user as a watcher for the specified repository.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***RepositoryApiWatch2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a RepositoryApiWatch2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestRepository**](RestRepository.md)| The repository to watch. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

