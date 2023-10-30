# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApplySuggestion**](PullRequestsApi.md#ApplySuggestion) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId}/apply-suggestion | Apply pull request suggestion
[**Approve**](PullRequestsApi.md#Approve) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/approve | Approve pull request
[**AssignParticipantRole**](PullRequestsApi.md#AssignParticipantRole) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants | Assign pull request participant role
[**CanMerge**](PullRequestsApi.md#CanMerge) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/merge | Test if pull request can be merged
[**CanRebase**](PullRequestsApi.md#CanRebase) | **Get** /git/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/rebase | Check PR rebase precondition
[**Create**](PullRequestsApi.md#Create) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests | Create pull request
[**Create1**](PullRequestsApi.md#Create1) | **Post** /api/latest/projects/{projectKey}/settings/reviewer-groups | Create reviewer group
[**Create2**](PullRequestsApi.md#Create2) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/reviewer-groups | Create reviewer group
[**CreateComment1**](PullRequestsApi.md#CreateComment1) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments | Add new blocker comment
[**CreateComment2**](PullRequestsApi.md#CreateComment2) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments | Add pull request comment
[**CreatePullRequestCondition**](PullRequestsApi.md#CreatePullRequestCondition) | **Post** /default-reviewers/latest/projects/{projectKey}/condition | Create default reviewer
[**CreatePullRequestCondition1**](PullRequestsApi.md#CreatePullRequestCondition1) | **Post** /default-reviewers/latest/projects/{projectKey}/repos/{repositorySlug}/condition | Create default reviewers condition
[**Decline**](PullRequestsApi.md#Decline) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/decline | Decline pull request
[**Delete3**](PullRequestsApi.md#Delete3) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId} | Delete pull request
[**Delete4**](PullRequestsApi.md#Delete4) | **Delete** /api/latest/projects/{projectKey}/settings/reviewer-groups/{id} | Delete reviewer group
[**Delete5**](PullRequestsApi.md#Delete5) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/reviewer-groups/{id} | Delete reviewer group
[**DeleteComment1**](PullRequestsApi.md#DeleteComment1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments/{commentId} | Delete pull request comment
[**DeleteComment2**](PullRequestsApi.md#DeleteComment2) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} | Delete a pull request comment
[**DeletePullRequestCondition**](PullRequestsApi.md#DeletePullRequestCondition) | **Delete** /default-reviewers/latest/projects/{projectKey}/condition/{id} | Remove default reviewer
[**DeletePullRequestCondition1**](PullRequestsApi.md#DeletePullRequestCondition1) | **Delete** /default-reviewers/latest/projects/{projectKey}/repos/{repositorySlug}/condition/{id} | Delete a default reviewer condition
[**DiscardReview**](PullRequestsApi.md#DiscardReview) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/review | Discard pull request review
[**FinishReview**](PullRequestsApi.md#FinishReview) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/review | Complete pull request review
[**Get3**](PullRequestsApi.md#Get3) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId} | Get pull request
[**GetActivities**](PullRequestsApi.md#GetActivities) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/activities | Get pull request activity
[**GetComment1**](PullRequestsApi.md#GetComment1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments/{commentId} | Get pull request comment
[**GetComment2**](PullRequestsApi.md#GetComment2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} | Get a pull request comment
[**GetComments1**](PullRequestsApi.md#GetComments1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments | Search pull request comments
[**GetComments2**](PullRequestsApi.md#GetComments2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments | Get pull request comments for path
[**GetCommitMessageSuggestion**](PullRequestsApi.md#GetCommitMessageSuggestion) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/commit-message-suggestion | Get commit message suggestion
[**GetCommits1**](PullRequestsApi.md#GetCommits1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/commits | Get pull request commits
[**GetMergeConfig**](PullRequestsApi.md#GetMergeConfig) | **Get** /api/latest/admin/pull-requests/{scmId} | Get merge strategies
[**GetPage**](PullRequestsApi.md#GetPage) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests | Get pull requests for repository
[**GetPullRequestConditions**](PullRequestsApi.md#GetPullRequestConditions) | **Get** /default-reviewers/latest/projects/{projectKey}/conditions | Get default reviewers
[**GetPullRequestConditions1**](PullRequestsApi.md#GetPullRequestConditions1) | **Get** /default-reviewers/latest/projects/{projectKey}/repos/{repositorySlug}/conditions | Get configured default reviewers
[**GetPullRequests**](PullRequestsApi.md#GetPullRequests) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/commits/{commitId}/pull-requests | Get repository pull requests containing commit
[**GetReview**](PullRequestsApi.md#GetReview) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/review | Get pull request comment thread
[**GetReviewerGroup**](PullRequestsApi.md#GetReviewerGroup) | **Get** /api/latest/projects/{projectKey}/settings/reviewer-groups/{id} | Get reviewer group
[**GetReviewerGroup1**](PullRequestsApi.md#GetReviewerGroup1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/reviewer-groups/{id} | Get reviewer group
[**GetReviewerGroups**](PullRequestsApi.md#GetReviewerGroups) | **Get** /api/latest/projects/{projectKey}/settings/reviewer-groups | Get all reviewer groups
[**GetReviewerGroups1**](PullRequestsApi.md#GetReviewerGroups1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/reviewer-groups | Get all reviewer groups
[**GetReviewers**](PullRequestsApi.md#GetReviewers) | **Get** /default-reviewers/latest/projects/{projectKey}/repos/{repositorySlug}/reviewers | Get required reviewers for PR creation
[**GetUsers**](PullRequestsApi.md#GetUsers) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/reviewer-groups/{id}/users | Get reviewer group users
[**ListParticipants**](PullRequestsApi.md#ListParticipants) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants | Get pull request participants
[**Merge**](PullRequestsApi.md#Merge) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/merge | Merge pull request
[**React1**](PullRequestsApi.md#React1) | **Put** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId}/reactions/{emoticon} | React to a PR comment
[**Rebase**](PullRequestsApi.md#Rebase) | **Post** /git/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/rebase | Rebase pull request
[**Reopen**](PullRequestsApi.md#Reopen) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/reopen | Re-open pull request
[**Search**](PullRequestsApi.md#Search) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/participants | Search pull request participants
[**SetMergeConfig**](PullRequestsApi.md#SetMergeConfig) | **Post** /api/latest/admin/pull-requests/{scmId} | Update merge strategies
[**StreamChanges1**](PullRequestsApi.md#StreamChanges1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/changes | Gets pull request changes
[**StreamDiff2**](PullRequestsApi.md#StreamDiff2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/diff/{path} | Stream a diff within a pull request
[**StreamPatch1**](PullRequestsApi.md#StreamPatch1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}.patch | Stream pull request as patch
[**StreamRawDiff2**](PullRequestsApi.md#StreamRawDiff2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}.diff | Stream raw pull request diff
[**UnReact1**](PullRequestsApi.md#UnReact1) | **Delete** /comment-likes/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId}/reactions/{emoticon} | Remove a reaction from a PR comment
[**UnassignParticipantRole**](PullRequestsApi.md#UnassignParticipantRole) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants/{userSlug} | Unassign pull request participant
[**UnassignParticipantRole1**](PullRequestsApi.md#UnassignParticipantRole1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants | Unassign pull request participant
[**Unwatch1**](PullRequestsApi.md#Unwatch1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/watch | Stop watching pull request
[**Update**](PullRequestsApi.md#Update) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId} | Update pull request metadata
[**Update1**](PullRequestsApi.md#Update1) | **Put** /api/latest/projects/{projectKey}/settings/reviewer-groups/{id} | Update reviewer group attributes
[**Update2**](PullRequestsApi.md#Update2) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/settings/reviewer-groups/{id} | Update reviewer group attributes
[**UpdateComment1**](PullRequestsApi.md#UpdateComment1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/blocker-comments/{commentId} | Update pull request comment
[**UpdateComment2**](PullRequestsApi.md#UpdateComment2) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/comments/{commentId} | Update pull request comment
[**UpdatePullRequestCondition**](PullRequestsApi.md#UpdatePullRequestCondition) | **Put** /default-reviewers/latest/projects/{projectKey}/condition/{id} | Update the default reviewer
[**UpdatePullRequestCondition1**](PullRequestsApi.md#UpdatePullRequestCondition1) | **Put** /default-reviewers/latest/projects/{projectKey}/repos/{repositorySlug}/condition/{id} | Update a default reviewer condition
[**UpdateStatus**](PullRequestsApi.md#UpdateStatus) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/participants/{userSlug} | Change pull request status
[**Watch1**](PullRequestsApi.md#Watch1) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/watch | Watch pull request
[**WithdrawApproval**](PullRequestsApi.md#WithdrawApproval) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/pull-requests/{pullRequestId}/approve | Unapprove pull request

# **ApplySuggestion**
> ApplySuggestion(ctx, projectKey, commentId, pullRequestId, repositorySlug, optional)
Apply pull request suggestion

Apply a suggestion contained within a comment.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The ID of the comment to retrieve. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiApplySuggestionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiApplySuggestionOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **body** | [**optional.Interface of RestApplySuggestionRequest**](RestApplySuggestionRequest.md)| A request containing other parameters required to apply a suggestion - The given versions/hashes must match the server&#x27;s version/hashes or the suggestion application will fail (in order to avoid applying the suggestion to the wrong place | 

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

# **AssignParticipantRole**
> RestPullRequestParticipant AssignParticipantRole(ctx, body, projectKey, pullRequestId, repositorySlug)
Assign pull request participant role

Assigns a participant to an explicit role in pull request. Currently only the REVIEWER role may be assigned.   If the user is not yet a participant in the pull request, they are made one and assigned the supplied role.   If the user is already a participant in the pull request, their previous role is replaced with the supplied role unless they are already assigned the AUTHOR role which cannot be changed and will result in a Bad Request (400) response code.   The authenticated user must have <strong>REPO_WRITE</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestPullRequestAssignParticipantRoleRequest**](RestPullRequestAssignParticipantRoleRequest.md)| The participant to be added to the pull request, includes the user and their role | 
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestPullRequestParticipant**](RestPullRequestParticipant.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CanMerge**
> RestPullRequestMergeability CanMerge(ctx, projectKey, pullRequestId, repositorySlug)
Test if pull request can be merged

Test whether a pull request can be merged.   A pull request may not be merged if:   - there are conflicts that need to be manually resolved before merging; and/or - one or more merge checks have vetoed the merge.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestPullRequestMergeability**](RestPullRequestMergeability.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CanRebase**
> RestPullRequestRebaseability CanRebase(ctx, projectKey, pullRequestId, repositorySlug)
Check PR rebase precondition

Checks preconditions to determine whether the pull request can be rebased.  Some of the preconditions are:  - The pull request is between Git repositories - The pull request is currently open - The pull request's {@link PullRequest#getFromRef \"from\" ref} is a <i>branch</i>    - In other words, the qualified ID for the \"from\" ref must start with <code>refs/heads/</code>    - Tags, and other non-standard refs, cannot be rebased - The current user has an e-mail address    - Pull requests cannot be rebased anonymously    - `git rebase` records the current user as the committer for the rebased commits, which        requires a name and e-mail address - The current user has <i>write</i> access to the {@link PullRequest#getFromRef \"from\" ref}'s repository    - Note that in order to <i>view</i> a pull request a user is only required to have <i>read</i>      access to the {@link PullRequest#getToRef toRef}'s repository, so just because a user can <i>see</i>      a pull request does not mean they can request a rebase   This list is not exhaustive, and the exact set of preconditions applied can be extended by third-party add-ons.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestPullRequestRebaseability**](RestPullRequestRebaseability.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Create**
> RestPullRequest Create(ctx, projectKey, repositorySlug, optional)
Create pull request

Create a new pull request from a source branch or tag to a target branch. The source and target may be in the same repository, or different ones. (Note that different repositories must belong to the same <code>Repository#getHierarchyId()</code> hierarchy.)   The <code>fromRef</code> may be a branch or a tag. The <code>toRef</code> is required to be a branch. Tags are not allowed as targets because tags are intended to be immutable and should not be changed after they are created.   The authenticated user must have <strong>REPO_READ</strong> permission for the <code>fromRef</code> and <code>toRef</code> repositories to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiCreateOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiCreateOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestPullRequest**](RestPullRequest.md)| The pull request data | 

### Return type

[**RestPullRequest**](RestPullRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Create1**
> RestReviewerGroup Create1(ctx, projectKey, optional)
Create reviewer group

Create a reviewer group.  The authenticated user must have <b>PROJECT_ADMIN</b> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***PullRequestsApiCreate1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiCreate1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestReviewerGroup**](RestReviewerGroup.md)| The reviewer group to be create | 

### Return type

[**RestReviewerGroup**](RestReviewerGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Create2**
> RestReviewerGroup Create2(ctx, projectKey, repositorySlug, optional)
Create reviewer group

Create a reviewer group.  The authenticated user must have <b>REPO_ADMIN</b> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiCreate2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiCreate2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestReviewerGroup**](RestReviewerGroup.md)| The request containing the details of the reviewer group. | 

### Return type

[**RestReviewerGroup**](RestReviewerGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateComment1**
> RestComment CreateComment1(ctx, projectKey, pullRequestId, repositorySlug, optional)
Add new blocker comment

Add a new blocker comment.   Comments can be added in a few places by setting different attributes:   General pull request blocker comment:  ```  {       \"text\": \"A task on a pull request.\"  } ```  Blocker reply to a comment:   ```  {      \"text\": \"This reply is a task.\",       \"parent\": {           \"id\": 1       }  }  ```  General blocker file comment:  ```  {      \"text\": \"A blocker comment on a file.\",       \"anchor\": {           \"diffType\": \"RANGE\",           \"fromHash\": \"6df3858eeb9a53a911cd17e66a9174d44ffb02cd\",           \"path\": \"path/to/file\",           \"srcPath\": \"path/to/file\",           \"toHash\": \"04c7c5c931b9418ca7b66f51fe934d0bd9b2ba4b\"       }   }  ```  Blocker file line comment:   ```  {       \"text\": \"A task on a particular line within a file.\",       \"anchor\": {           \"diffType\": \"COMMIT\",           \"line\": 1,           \"lineType\": \"CONTEXT\",           \"fileType\": \"FROM\",           \"fromHash\": \"6df3858eeb9a53a911cd17e66a9174d44ffb02cd\",           \"path\": \"path/to/file\",           \"srcPath\": \"path/to/file\",           \"toHash\": \"04c7c5c931b9418ca7b66f51fe934d0bd9b2ba4b\"       }   }  ```  For file and line comments, 'path' refers to the path of the file to which the comment should be applied and 'srcPath' refers to the path the that file used to have (only required for copies and moves). Also, fromHash and toHash refer to the sinceId / untilId (respectively) used to produce the diff on which the comment was added. Finally diffType refers to the type of diff the comment was added on. For backwards compatibility purposes if no diffType is provided and no fromHash/toHash pair is provided the diffType will be resolved to 'EFFECTIVE'. In any other cases the diffType is REQUIRED.   For line comments, 'line' refers to the line in the diff that the comment should apply to. 'lineType' refers to the type of diff hunk, which can be:   - 'ADDED' - for an added line; - 'REMOVED' - for a removed line; or - 'CONTEXT' - for a line that was unmodified but is in the vicinity of the diff.    'fileType' refers to the file of the diff to which the anchor should be attached - which is of relevance when displaying the diff in a side-by-side way. Currently the supported values are:   - 'FROM' - the source file of the diff  - 'TO' - the destination file of the diff   If the current user is not a participant the user is added as a watcher of the pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiCreateComment1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiCreateComment1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestComment**](RestComment.md)| The comment to add. | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateComment2**
> RestComment CreateComment2(ctx, projectKey, pullRequestId, repositorySlug, optional)
Add pull request comment

Add a new comment.   Comments can be added in a few places by setting different attributes: </p>General pull request comment:   <pre> {     \"text\": \"An insightful general comment on a pull request.\"   }   </pre> Reply to a comment:  <pre> {     \"text\": \"A measured reply.\",     \"parent\": {        \"id\": 1      }   }   </pre> General file comment:  <pre> {     \"text\": \"An insightful general comment on a file.\",     \"anchor\": {        \"diffType\": \"RANGE\",        \"fromHash\": \"6df3858eeb9a53a911cd17e66a9174d44ffb02cd\",        \"path\": \"path/to/file\",        \"srcPath\": \"path/to/file\",        \"toHash\": \"04c7c5c931b9418ca7b66f51fe934d0bd9b2ba4b\"     }   }   </pre> File line comment:  <pre> {     \"text\": \"A pithy comment on a particular line within a file.\",     \"anchor\": {        \"diffType\": \"COMMIT\",        \"line\": 1,        \"lineType\": \"CONTEXT\",        \"fileType\": \"FROM\",        \"fromHash\": \"6df3858eeb9a53a911cd17e66a9174d44ffb02cd\",        \"path\": \"path/to/file\",        \"srcPath\": \"path/to/file\",        \"toHash\": \"04c7c5c931b9418ca7b66f51fe934d0bd9b2ba4b\"      }   }   </pre>    Add a new task.   Tasks are just comments with the attribute 'severity' set to 'BLOCKER':   General pull request task:  <pre> {     \"text\": \"A task on a pull request.\",     \"severity\": \"BLOCKER\"   }   </pre>    Add a pending comment.    Pending comments are just comments with the attribute 'state' set to 'PENDING':   Pending comment: <pre> {     \"text\": \"This is a pending comment\",     \"state\": \"PENDING\"   }   </pre>   For file and line comments, 'path' refers to the path of the file to which the comment should be applied and 'srcPath' refers to the path the that file used to have (only required for copies and moves). Also, fromHash and toHash refer to the sinceId / untilId (respectively) used to produce the diff on which the comment was added. Finally diffType refers to the type of diff the comment was added on. For backwards compatibility purposes if no diffType is provided and no fromHash/toHash pair is provided the diffType will be resolved to 'EFFECTIVE'. In any other cases the diffType is REQUIRED.   For line comments, 'line' refers to the line in the diff that the comment should apply to. 'lineType' refers to the type of diff hunk, which can be:   - 'ADDED' - for an added line; - 'REMOVED' - for a removed line; or - 'CONTEXT' - for a line that was unmodified but is in the vicinity of the diff. </ul>'fileType' refers to the file of the diff to which the anchor should be attached - which is of relevance when displaying the diff in a side-by-side way. Currently the supported values are:   - 'FROM' - the source file of the diff - 'TO' - the destination file of the diff </ul>If the current user is not a participant the user is added as a watcher of the pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiCreateComment2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiCreateComment2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestComment**](RestComment.md)| The comment to add | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreatePullRequestCondition**
> RestPullRequestCondition CreatePullRequestCondition(ctx, projectKey, optional)
Create default reviewer

Create a default reviewer pull request condition for the given project.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***PullRequestsApiCreatePullRequestConditionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiCreatePullRequestConditionOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestDefaultReviewersRequest**](RestDefaultReviewersRequest.md)| The details needed to create a default reviewer pull request condition. | 

### Return type

[**RestPullRequestCondition**](RestPullRequestCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreatePullRequestCondition1**
> RestPullRequestCondition CreatePullRequestCondition1(ctx, projectKey, repositorySlug, optional)
Create default reviewers condition

Create a default reviewer pull request condition for the given repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiCreatePullRequestCondition1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiCreatePullRequestCondition1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestDefaultReviewersRequest**](RestDefaultReviewersRequest.md)| The details needed to create a default reviewer pull request condition. | 

### Return type

[**RestPullRequestCondition**](RestPullRequestCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Decline**
> RestPullRequest Decline(ctx, projectKey, pullRequestId, repositorySlug, optional)
Decline pull request

Decline a pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pullrequest ID provided by the path | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiDeclineOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiDeclineOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestPullRequestDeclineRequest**](RestPullRequestDeclineRequest.md)| The body holder | 
 **version** | **optional.**| The current version of the pull request. If the server&#x27;s version isn&#x27;t the same as the specified version the operation will fail. To determine the current version of the pull request it should be fetched from the server prior to this operation. Look for the &#x27;version&#x27; attribute in the returned JSON structure. | 

### Return type

[**RestPullRequest**](RestPullRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete3**
> Delete3(ctx, projectKey, pullRequestId, repositorySlug, optional)
Delete pull request

Deletes a pull request.   To call this resource, users must be authenticated and have permission to view the pull request. Additionally, they must:   - be the pull request author, if the system is configured to allow authors to delete their own   pull requests (this is the default) OR  - have repository administrator permission for the repository the pull request is targeting   A body containing the version of the pull request must be provided with this request.   `{ \"version\": 1 }`

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiDelete3Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiDelete3Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestPullRequestDeleteRequest**](RestPullRequestDeleteRequest.md)| A body containing the version of the pull request | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete4**
> Delete4(ctx, projectKey, id)
Delete reviewer group

Deletes a reviewer group.  The authenticated user must have <b>PROJECT_ADMIN</b> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the reviewer group to be deleted | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete5**
> Delete5(ctx, projectKey, id, repositorySlug)
Delete reviewer group

Deletes a reviewer group.  The authenticated user must have <b>REPO_ADMIN</b> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the reviewer group to be deleted | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteComment1**
> DeleteComment1(ctx, projectKey, commentId, pullRequestId, repositorySlug, optional)
Delete pull request comment

Delete a pull request comment. Anyone can delete their own comment. Only users with <strong>REPO_ADMIN</strong> and above may delete comments created by other users.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The ID of the comment to retrieve. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiDeleteComment1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiDeleteComment1Opts struct
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

# **DeleteComment2**
> DeleteComment2(ctx, projectKey, commentId, pullRequestId, repositorySlug, optional)
Delete a pull request comment

Delete a pull request comment. Anyone can delete their own comment. Only users with <strong>REPO_ADMIN</strong> and above may delete comments created by other users.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The ID of the comment to retrieve. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiDeleteComment2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiDeleteComment2Opts struct
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

# **DeletePullRequestCondition**
> DeletePullRequestCondition(ctx, projectKey, id)
Remove default reviewer

Delete the default reviewer pull request condition associated with the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the pull request condition. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeletePullRequestCondition1**
> DeletePullRequestCondition1(ctx, projectKey, id, repositorySlug)
Delete a default reviewer condition

Delete the default reviewer pull request condition associated with the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **int32**|  | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DiscardReview**
> DiscardReview(ctx, projectKey, pullRequestId, repositorySlug)
Discard pull request review

Discard a pull request review for the authenticated user.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository to call this resource.

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

# **FinishReview**
> FinishReview(ctx, projectKey, pullRequestId, repositorySlug, optional)
Complete pull request review

Complete a review on a pull request.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiFinishReviewOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiFinishReviewOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestPullRequestFinishReviewRequest**](RestPullRequestFinishReviewRequest.md)| The REST request which contains comment text and participant status | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Get3**
> RestPullRequest Get3(ctx, projectKey, pullRequestId, repositorySlug)
Get pull request

Retrieve a pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestPullRequest**](RestPullRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetActivities**
> InlineResponse20039 GetActivities(ctx, projectKey, pullRequestId, repositorySlug, optional)
Get pull request activity

Retrieve a page of activity associated with a pull request.   Activity items include comments, approvals, rescopes (i.e. adding and removing of commits), merges and more.   Different types of activity items may be introduced in newer versions of Stash or by user installed plugins, so clients should be flexible enough to handle unexpected entity shapes in the returned page.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetActivitiesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetActivitiesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **fromType** | **optional.String**| (required if &lt;strong&gt;fromId&lt;/strong&gt; is present) the type of the activity item specified by &lt;strong&gt;fromId&lt;/strong&gt; (either &lt;strong&gt;COMMENT&lt;/strong&gt; or &lt;strong&gt;ACTIVITY&lt;/strong&gt;) | 
 **fromId** | **optional.String**| (optional) the ID of the activity item to use as the first item in the returned page | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20039**](inline_response_200_39.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetComment1**
> RestComment GetComment1(ctx, projectKey, commentId, pullRequestId, repositorySlug)
Get pull request comment

Retrieves a pull request comment.  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The ID of the comment to retrieve | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetComment2**
> RestComment GetComment2(ctx, projectKey, commentId, pullRequestId, repositorySlug)
Get a pull request comment

Retrieves a pull request comment.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The ID of the comment to retrieve. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetComments1**
> InlineResponse20036 GetComments1(ctx, projectKey, pullRequestId, repositorySlug, optional)
Search pull request comments

Gets comments matching the given set of field values for the specified pull request. (Note this does <b>not</b> perform any kind of searching for comments by their text).   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetComments1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetComments1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **count** | **optional.String**| If true only the count of the comments by state will be returned (and not the body of the comments). | 
 **state** | [**optional.Interface of []string**](string.md)|  | 
 **states** | **optional.String**| (optional). If supplied, only comments with a state in the given list will be returned. The state can be OPEN or RESOLVED. | 
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

# **GetComments2**
> InlineResponse20036 GetComments2(ctx, path, projectKey, pullRequestId, repositorySlug, optional)
Get pull request comments for path

Gets comments for the specified pull request and path.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The path to stream comments for a given path | 
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetComments2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetComments2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **fromHash** | **optional.String**| The from commit hash to stream comments for a RANGE or COMMIT arbitrary change scope | 
 **anchorState** | **optional.String**| ACTIVE to stream the active comments; ORPHANED to stream the orphaned comments; ALL to stream both the active and the orphaned comments; | 
 **diffType** | [**optional.Interface of []string**](string.md)|  | 
 **toHash** | **optional.String**| The to commit hash to stream comments for a RANGE or COMMIT arbitrary change scope | 
 **state** | [**optional.Interface of []string**](string.md)|  | 
 **diffTypes** | **optional.String**| EFFECTIVE to stream the comments related to the effective diff of the pull request; RANGE to stream comments related to a commit range between two arbitrary commits (requires &#x27;fromHash&#x27; and &#x27;toHash&#x27;); COMMIT to stream comments related to a commit between two arbitrary commits (requires &#x27;fromHash&#x27; and &#x27;toHash&#x27;) | 
 **states** | **optional.String**| (optional). If supplied, only comments with a state in the given list will be returned. The state can be OPEN or RESOLVED. | 
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

# **GetCommitMessageSuggestion**
> RestCommitMessageSuggestion GetCommitMessageSuggestion(ctx, projectKey, pullRequestId, repositorySlug)
Get commit message suggestion

Retrieve a suggested commit message for the given Pull Request.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request to generate the suggestion for | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestCommitMessageSuggestion**](RestCommitMessageSuggestion.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetCommits1**
> InlineResponse20035 GetCommits1(ctx, projectKey, pullRequestId, repositorySlug, optional)
Get pull request commits

Retrieve commits for the specified pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| ID of the pullrequest, part of the path | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetCommits1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetCommits1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **avatarScheme** | **optional.String**| The desired scheme for the avatar URL. If the parameter is not present URLs will use the same scheme as this request | 
 **withCounts** | **optional.String**| If set to true, the service will add \&quot;authorCount\&quot; and \&quot;totalCount\&quot; at the end of the page. \&quot;authorCount\&quot; is the number of different authors and \&quot;totalCount\&quot; is the total number of commits. | 
 **avatarSize** | **optional.String**| If present the service adds avatar URLs for commit authors. Should be an integer specifying the desired size in pixels. If the parameter is not present, avatar URLs will not be setCOMMIT to stream comments related to a commit between two arbitrary commits (requires &#x27;fromHash&#x27; and &#x27;toHash&#x27;) | 
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

# **GetMergeConfig**
> RestPullRequestMergeConfig GetMergeConfig(ctx, scmId)
Get merge strategies

Retrieve the merge strategies available for this instance.   The user must be authenticated to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **scmId** | **string**| the id of the scm to get strategies for | 

### Return type

[**RestPullRequestMergeConfig**](RestPullRequestMergeConfig.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPage**
> InlineResponse20022 GetPage(ctx, projectKey, repositorySlug, optional)
Get pull requests for repository

Retrieve a page of pull requests to or from the specified repository.   The authenticated user must have <strong>REPO_READ</strong> permission for the specified repository to call this resource.  Optionally clients can specify PR participant filters. Each filter has a mandatory username.N parameter, and the optional role.N and approved.N parameters.   - username.N - the \"root\" of a single participant filter, where \"N\" is a natural number   starting from 1. This allows clients to specify multiple participant filters, by providing consecutive   filters as username.1, username.2 etc. Note that the filters numbering has to start   with 1 and be continuous for all filters to be processed. The total allowed number of participant   filters is 10 and all filters exceeding that limit will be dropped. - role.N(optional) the role associated with username.N.   This must be one of AUTHOR, REVIEWER, or PARTICIPANT - approved.N (optional) the approved status associated with username.N.   That is whether username.N has approved the PR. Either true, or false 

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetPageOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetPageOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **withAttributes** | **optional.String**| (optional) defaults to true, whether to return additional pull request attributes | 
 **at** | **optional.String**| (optional) a &lt;i&gt;fully-qualified&lt;/i&gt; branch ID to find pull requests to or from, such as refs/heads/master | 
 **withProperties** | **optional.String**| (optional) defaults to true, whether to return additional pull request properties | 
 **filterText** | **optional.String**| (optional) If specified, only pull requests where the title or description contains the supplied string will be returned. | 
 **state** | **optional.String**| (optional, defaults to &lt;strong&gt;OPEN&lt;/strong&gt;). Supply &lt;strong&gt;ALL&lt;/strong&gt; to return pull request in any state. If a state is supplied only pull requests in the specified state will be returned. Either &lt;strong&gt;OPEN&lt;/strong&gt;, &lt;strong&gt;DECLINED&lt;/strong&gt; or &lt;strong&gt;MERGED&lt;/strong&gt;. | 
 **order** | **optional.String**| (optional, defaults to &lt;strong&gt;NEWEST&lt;/strong&gt;) the order to return pull requests in, either &lt;strong&gt;OLDEST&lt;/strong&gt; (as in: \&quot;oldest first\&quot;) or &lt;strong&gt;NEWEST&lt;/strong&gt;. | 
 **direction** | **optional.String**| (optional, defaults to &lt;strong&gt;INCOMING&lt;/strong&gt;) the direction relative to the specified repository. Either &lt;strong&gt;INCOMING&lt;/strong&gt; or &lt;strong&gt;OUTGOING&lt;/strong&gt;. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20022**](inline_response_200_22.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPullRequestConditions**
> []RestPullRequestCondition GetPullRequestConditions(ctx, projectKey)
Get default reviewers

Return a page of default reviewer pull request conditions that have been configured for this project.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 

### Return type

[**[]RestPullRequestCondition**](RestPullRequestCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPullRequestConditions1**
> []RestPullRequestCondition GetPullRequestConditions1(ctx, projectKey, repositorySlug)
Get configured default reviewers

Return a page of default reviewer pull request conditions that have been configured for this repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**[]RestPullRequestCondition**](RestPullRequestCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPullRequests**
> InlineResponse20022 GetPullRequests(ctx, projectKey, commitId, repositorySlug, optional)
Get repository pull requests containing commit

Retrieve a page of pull requests in the current repository that contain the given commit.  The user must be authenticated and have access to the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **commitId** | **string**| the commit ID | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***PullRequestsApiGetPullRequestsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetPullRequestsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20022**](inline_response_200_22.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetReview**
> InlineResponse20036 GetReview(ctx, projectKey, pullRequestId, repositorySlug, optional)
Get pull request comment thread

Get the <code>CommentThread</code> threads which have <code>Comment</code> comments that have a <code>CommentState#PENDING</code> pending state and are part of the pull request review for the authenticated user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetReviewOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetReviewOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



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

# **GetReviewerGroup**
> RestReviewerGroup GetReviewerGroup(ctx, projectKey, id)
Get reviewer group

Retrieve a reviewer group.  The authenticated user must have <b>PROJECT_READ</b> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the reviewer group to be retrieved | 

### Return type

[**RestReviewerGroup**](RestReviewerGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetReviewerGroup1**
> RestReviewerGroup GetReviewerGroup1(ctx, projectKey, id, repositorySlug)
Get reviewer group

Retrieve a reviewer group.  The authenticated user must have <b>REPO_READ</b> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the reviewer group to be retrieved | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestReviewerGroup**](RestReviewerGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetReviewerGroups**
> InlineResponse20045 GetReviewerGroups(ctx, projectKey, optional)
Get all reviewer groups

Retrieve a page of reviewer groups of a given scope.  The authenticated user must have <b>PROJECT_READ</b> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***PullRequestsApiGetReviewerGroupsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetReviewerGroupsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20045**](inline_response_200_45.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetReviewerGroups1**
> InlineResponse20045 GetReviewerGroups1(ctx, projectKey, repositorySlug, optional)
Get all reviewer groups

Retrieve a page of reviewer groups of a given scope.  The authenticated user must have <b>REPO_READ</b> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetReviewerGroups1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetReviewerGroups1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20045**](inline_response_200_45.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetReviewers**
> []RestPullRequestCondition GetReviewers(ctx, projectKey, repositorySlug, optional)
Get required reviewers for PR creation

Return a set of users who are required reviewers for pull requests created from the given source repository and ref to the given target ref in this repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiGetReviewersOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiGetReviewersOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **targetRepoId** | **optional.String**| The ID of the repository in which the target ref exists | 
 **sourceRepoId** | **optional.String**| The ID of the repository in which the source ref exists | 
 **sourceRefId** | **optional.String**| The ID of the source ref | 
 **targetRefId** | **optional.String**| The ID of the target ref | 

### Return type

[**[]RestPullRequestCondition**](RestPullRequestCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUsers**
> []RestApplicationUser GetUsers(ctx, projectKey, id, repositorySlug)
Get reviewer group users

Retrieve a list of the users of a reviewer group.  This does not return all the users of the group, only the users who have <b>REPO_READ</b> permission for the specified repository.  The authenticated user must have <b>REPO_READ</b> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the reviewer group to be retrieved | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**[]RestApplicationUser**](RestApplicationUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json;charset=UTF-8

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListParticipants**
> InlineResponse20040 ListParticipants(ctx, projectKey, pullRequestId, repositorySlug, optional)
Get pull request participants

Retrieves a page of the participants for a given pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiListParticipantsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiListParticipantsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20040**](inline_response_200_40.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Merge**
> RestPullRequest Merge(ctx, projectKey, pullRequestId, repositorySlug, optional)
Merge pull request

Merge the specified pull request.  The authenticated user must have <strong>REPO_WRITE</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiMergeOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiMergeOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestPullRequestMergeRequest**](RestPullRequestMergeRequest.md)| The body holder | 
 **version** | **optional.**| The current version of the pull request. If the server&#x27;s version isn&#x27;t the same as the specified version the operation will fail. To determine the current version of the pull request it should be fetched from the server prior to this operation. Look for the &#x27;version&#x27; attribute in the returned JSON structure. | 

### Return type

[**RestPullRequest**](RestPullRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **React1**
> RestUserReaction React1(ctx, projectKey, commentId, pullRequestId, emoticon, repositorySlug)
React to a PR comment

Add an emoticon reaction to a pull request comment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The comment id. | 
  **pullRequestId** | **string**| The pull request id. | 
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

# **Rebase**
> RestPullRequestRebaseResult Rebase(ctx, projectKey, pullRequestId, repositorySlug, optional)
Rebase pull request

Rebases the specified pull request, rewriting the incoming commits to start from the tip commit of the pull request's target branch. <i>This operation alters the pull request's source branch and cannot be undone.</i>  The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets <i>and</i> <strong>REPO_WRITE</strong> permission for the pull request's source repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiRebaseOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiRebaseOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestPullRequestRebaseRequest**](RestPullRequestRebaseRequest.md)| The pull request rebase request. | 

### Return type

[**RestPullRequestRebaseResult**](RestPullRequestRebaseResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Reopen**
> RestPullRequest Reopen(ctx, projectKey, pullRequestId, repositorySlug, optional)
Re-open pull request

Re-open a declined pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiReopenOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiReopenOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestPullRequestReopenRequest**](RestPullRequestReopenRequest.md)| The body holder | 
 **version** | **optional.**| The current version of the pull request. If the server&#x27;s version isn&#x27;t the same as the specified version the operation will fail. To determine the current version of the pull request it should be fetched from the server prior to this operation. Look for the &#x27;version&#x27; attribute in the returned JSON structure. | 

### Return type

[**RestPullRequest**](RestPullRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Search**
> InlineResponse2005 Search(ctx, projectKey, repositorySlug, optional)
Search pull request participants

Retrieve a page of participant users for all the pull requests to or from the specified repository.   Optionally clients can specify following filters.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiSearchOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiSearchOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| (optional) Return only users, whose username, name or email address &lt;i&gt;contain&lt;/i&gt; the filter value | 
 **role** | **optional.String**| (optional) The role associated with the pull request participant. This must be one of AUTHOR, REVIEWER, or PARTICIPANT | 
 **direction** | **optional.String**| (optional), Defaults to &lt;strong&gt;INCOMING&lt;/strong&gt;) the direction relative to the specified repository. Either &lt;strong&gt;INCOMING&lt;/strong&gt; or &lt;strong&gt;OUTGOING&lt;/strong&gt;. | 
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

# **SetMergeConfig**
> RestPullRequestMergeConfig SetMergeConfig(ctx, scmId, optional)
Update merge strategies

Update the pull request merge strategies for the context repository.   The authenticated user must have <strong>ADMIN</strong> permission to call this resource.   Only the strategies provided will be enabled, only one may be set to default   The commit message template will not be updated if not provided, and will be deleted if the `commitMessageTemplate` attribute is empty, i.e: `commitMessageTemplate: {}`.  An explicitly set pull request merge strategy configuration can be deleted by POSTing a document with an empty `mergeConfig` attribute. i.e: ``` {      \"mergeConfig\": {}  }  ```  Upon completion of this request, the effective configuration will be the default configuration.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **scmId** | **string**| the id of the scm to get strategies for | 
 **optional** | ***PullRequestsApiSetMergeConfigOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiSetMergeConfigOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestPullRequestSettings**](RestPullRequestSettings.md)| the settings | 

### Return type

[**RestPullRequestMergeConfig**](RestPullRequestMergeConfig.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamChanges1**
> RestChange StreamChanges1(ctx, projectKey, pullRequestId, repositorySlug, optional)
Gets pull request changes

Gets changes for the specified PullRequest.  If the changeScope query parameter is set to 'UNREVIEWED', the application will attempt to stream unreviewed changes based on the lastReviewedCommit of the current user, which are the changes between the lastReviewedCommit and the latest commit of the source branch. The current user is considered to <i>not</i> have any unreviewed changes for the pull request when the lastReviewedCommit is either null (everything is unreviewed, so all changes are streamed), equal to the latest commit of the source branch (everything is reviewed), or no longer on the source branch (the source branch has been rebased). In these cases, the application will fall back to streaming all changes (the default), which is the effective diff for the pull request. The type of changes streamed can be determined by the changeScope parameter included in the properties map of the response.   Note: This resource is currently <i>not paged</i>. The server will return at most one page. The server will truncate the number of changes to either the request's page limit or an internal maximum, whichever is smaller. The start parameter of the page request is also ignored.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiStreamChanges1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiStreamChanges1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **sinceId** | **optional.String**| The since commit hash to stream changes for a RANGE arbitrary change scope | 
 **changeScope** | **optional.String**| UNREVIEWED to stream the unreviewed changes for the current user (if they exist); RANGE to stream changes between two arbitrary commits (requires &#x27;sinceId&#x27; and &#x27;untilId&#x27;); otherwise ALL to stream all changes (the default) | 
 **untilId** | **optional.String**| The until commit hash to stream changes for a RANGE arbitrary change scope | 
 **withComments** | **optional.String**| true to apply comment counts in the changes (the default); otherwise, false to stream changes without comment counts | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**RestChange**](RestChange.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamDiff2**
> InlineResponse20037 StreamDiff2(ctx, path, projectKey, pullRequestId, repositorySlug, optional)
Stream a diff within a pull request

Streams a diff within a pull request.   If the specified file has been copied, moved or renamed, the <code>srcPath</code> must also be specified to produce the correct diff.   To stream a raw text representation of the diff, this endpoint can be called with the request header 'Accept: text/plain'.   Note: This RESTful endpoint is currently <i>not paged</i>. The server will internally apply a hard cap to the streamed lines, and it is not possible to request subsequent pages if that cap is exceeded.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **path** | **string**| The path to the file which should be diffed (optional) | 
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiStreamDiff2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiStreamDiff2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **avatarScheme** | **optional.String**| The security scheme for avatar URLs. If the scheme is not present then it is inherited from the request. It can be set to \&quot;https\&quot; to force the use of secure URLs. Not applicable if streaming raw diff | 
 **contextLines** | **optional.String**| The number of context lines to include around added/removed lines in the diff | 
 **sinceId** | **optional.String**| The since commit hash to stream a diff between two arbitrary hashes | 
 **srcPath** | **optional.String**| The previous path to the file, if the file has been copied, moved or renamed | 
 **diffType** | **optional.String**| The type of diff being requested. When withComments is true this works as a hint to the system to attach the correct set of comments to the diff. Not applicable if streaming raw diff | 
 **untilId** | **optional.String**| The until commit hash to stream a diff between two arbitrary hashes | 
 **whitespace** | **optional.String**| Optional whitespace flag which can be set to &lt;code&gt;ignore-all&lt;/code&gt; | 
 **withComments** | **optional.String**| &lt;code&gt;true&lt;/code&gt; to embed comments in the diff (the default); otherwise, &lt;code&gt;false&lt;/code&gt; to stream the diff without comments. Not applicable if streaming raw diff | 
 **avatarSize** | **optional.String**| If present the service adds avatar URLs for comment authors where the provided value specifies the desired avatar size in pixels. Not applicable if streaming raw diff | 
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

# **StreamPatch1**
> StreamPatch1(ctx, projectKey, pullRequestId, repositorySlug)
Stream pull request as patch

Streams a patch representing a pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StreamRawDiff2**
> StreamRawDiff2(ctx, projectKey, pullRequestId, repositorySlug, optional)
Stream raw pull request diff

Streams the raw diff for a pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiStreamRawDiff2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiStreamRawDiff2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **contextLines** | **optional.String**| The number of context lines to include around added/removed lines in the diff | 
 **whitespace** | **optional.String**| optional whitespace flag which can be set to &lt;code&gt;ignore-all&lt;/code&gt; | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, text/html

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UnReact1**
> UnReact1(ctx, projectKey, commentId, pullRequestId, emoticon, repositorySlug)
Remove a reaction from a PR comment

Remove an emoticon reaction from a pull request comment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The comment id. | 
  **pullRequestId** | **string**| The pull request id. | 
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

# **UnassignParticipantRole**
> UnassignParticipantRole(ctx, projectKey, userSlug, pullRequestId, repositorySlug)
Unassign pull request participant

Unassigns a participant from the REVIEWER role they may have been given in a pull request.   If the participant has no explicit role this method has no effect.   Afterwards, the user will still remain a participant in the pull request but their role will be reduced to PARTICIPANT. This is because once made a participant of a pull request, a user will forever remain a participant. Only their role may be altered.   The authenticated user must have <strong>REPO_WRITE</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **userSlug** | **string**| The slug for the user being unassigned | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

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
 **optional** | ***PullRequestsApiUnassignParticipantRole1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUnassignParticipantRole1Opts struct
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

# **Unwatch1**
> Unwatch1(ctx, projectKey, pullRequestId, repositorySlug)
Stop watching pull request

Remove the authenticated user as a watcher for the specified pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

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

# **Update**
> RestPullRequest Update(ctx, projectKey, pullRequestId, repositorySlug, optional)
Update pull request metadata

Update the title, description, reviewers or destination branch of an existing pull request.   **Note:** the <em>reviewers</em> list may be updated using this resource. However the <em>author</em> and <em>participants</em> list may not.   The authenticated user must either:   - be the author of the pull request and have the <strong>REPO_READ</strong> permission for the repository that this pull request targets; or - have the <strong>REPO_WRITE</strong> permission for the repository that this pull request targets   to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiUpdateOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUpdateOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestPullRequest**](RestPullRequest.md)| The updated pull request | 

### Return type

[**RestPullRequest**](RestPullRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Update1**
> RestReviewerGroup Update1(ctx, projectKey, id, optional)
Update reviewer group attributes

Update the attributes of a reviewer group.  The authenticated user must have <b>PROJECT_READ</b> permission for the specified project to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the reviewer group to be updated | 
 **optional** | ***PullRequestsApiUpdate1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUpdate1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestReviewerGroup**](RestReviewerGroup.md)| The request containing the attributes of the reviewer group to be updated. Only the attributes to be updated need to be present in this object. | 

### Return type

[**RestReviewerGroup**](RestReviewerGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Update2**
> RestReviewerGroup Update2(ctx, projectKey, id, repositorySlug, optional)
Update reviewer group attributes

Update the attributes of a reviewer group.  The authenticated user must have <b>REPO_ADMIN</b> permission for the specified repository to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the reviewer group to be updated | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiUpdate2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUpdate2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestReviewerGroup**](RestReviewerGroup.md)| The request containing the attributes of the reviewer group to be updated. Only the attributes to be updated need to be present in this object. | 

### Return type

[**RestReviewerGroup**](RestReviewerGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateComment1**
> RestComment UpdateComment1(ctx, projectKey, commentId, pullRequestId, repositorySlug, optional)
Update pull request comment

Update a comment, with the following restrictions:   - only the author of the comment may update the <i>text</i> of the comment - only the author of the comment, the author of the pull request or repository admins and above may update   the other fields of a comment   Convert a comment to a task or vice versa.   Comments can be converted to tasks by setting the 'severity' attribute to 'BLOCKER':  ```  {  \"severity\": \"BLOCKER\"  }  ```  Tasks can be converted to comments by setting the 'severity' attribute to 'NORMAL': ```  {  \"severity\": \"NORMAL\"  }  ```  Resolve a blocker comment.   Blocker comments can be resolved by setting the 'state' attribute to 'RESOLVED': ```  {  \"state\": \"RESOLVED\"  }  ```  <strong>Note:</strong> the supplied JSON object must contain a <code>version</code> that must match the server's version of the comment or the update will fail. To determine the current version of the comment, the comment should be fetched from the server prior to the update. Look for the 'version' attribute in the returned JSON structure.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The ID of the comment to retrieve. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiUpdateComment1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUpdateComment1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **body** | [**optional.Interface of RestComment**](RestComment.md)| The comment to add. | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateComment2**
> RestComment UpdateComment2(ctx, projectKey, commentId, pullRequestId, repositorySlug, optional)
Update pull request comment

Update a comment, with the following restrictions:   - only the author of the comment may update the <i>text</i> of the comment - only the author of the comment, the author of the pull request or repository admins and above may update the other fields of a comment </ul>   Convert a comment to a task or vice versa.   Comments can be converted to tasks by setting the 'severity' attribute to 'BLOCKER':   <pre> {   \"severity\": \"BLOCKER\"   }   </pre>  Tasks can be converted to comments by setting the 'severity' attribute to 'NORMAL':  <pre> {   \"severity\": \"NORMAL\"   }   </pre>  Resolve a task.   Tasks can be resolved by setting the 'state' attribute to 'RESOLVED':  <pre> {   \"state\": \"RESOLVED\"   }   </pre>  <strong>Note:</strong> the supplied JSON object must contain a <code>version</code> that must match the server's version of the comment or the update will fail. To determine the current version of the comment, the comment should be fetched from the server prior to the update. Look for the 'version' attribute in the returned JSON structure.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **commentId** | **string**| The ID of the comment to retrieve. | 
  **pullRequestId** | **string**| The pull request ID. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiUpdateComment2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUpdateComment2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **body** | [**optional.Interface of RestComment**](RestComment.md)| The updated comment | 

### Return type

[**RestComment**](RestComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdatePullRequestCondition**
> RestPullRequestCondition UpdatePullRequestCondition(ctx, projectKey, id, optional)
Update the default reviewer

Update the default reviewer pull request condition for the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the pull request condition. | 
 **optional** | ***PullRequestsApiUpdatePullRequestConditionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUpdatePullRequestConditionOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestDefaultReviewersRequest**](RestDefaultReviewersRequest.md)| The new details for the default reviewer pull request condition. | 

### Return type

[**RestPullRequestCondition**](RestPullRequestCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdatePullRequestCondition1**
> RestPullRequestCondition UpdatePullRequestCondition1(ctx, projectKey, id, repositorySlug, optional)
Update a default reviewer condition

Update the default reviewer pull request condition for the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The ID of the pull request condition | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PullRequestsApiUpdatePullRequestCondition1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PullRequestsApiUpdatePullRequestCondition1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of ConditionIdBody**](ConditionIdBody.md)|  | 

### Return type

[**RestPullRequestCondition**](RestPullRequestCondition.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateStatus**
> RestPullRequestParticipant UpdateStatus(ctx, body, projectKey, userSlug, pullRequestId, repositorySlug)
Change pull request status

Change the current user's status for a pull request. Implicitly adds the user as a participant if they are not already. If the current user is the author, this method will fail.   The possible values for {@code status} are <strong>UNAPPROVED</strong>, <strong>NEEDS_WORK</strong> (which is referred to as \"Requested changes\" in the frontend from 8.10 onward), or <strong>APPROVED</strong>.   If the new {@code status} is <strong>NEEDS_WORK</strong> or <strong>APPROVED</strong> then the {@code lastReviewedCommit} for the participant will be updated to the latest commit of the source branch of the pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestPullRequestAssignStatusRequest**](RestPullRequestAssignStatusRequest.md)| The participant representing the status to set, includes the status of the participant | 
  **projectKey** | **string**| The project key. | 
  **userSlug** | **string**| The slug for the user changing their status | 
  **pullRequestId** | **string**| The ID of the pull request within the repository | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestPullRequestParticipant**](RestPullRequestParticipant.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Watch1**
> Watch1(ctx, projectKey, pullRequestId, repositorySlug)
Watch pull request

Add the authenticated user as a watcher for the specified pull request.   The authenticated user must have <strong>REPO_READ</strong> permission for the repository that this pull request targets to call this resource.

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

