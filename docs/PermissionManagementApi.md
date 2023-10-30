# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddGroupToUser**](PermissionManagementApi.md#AddGroupToUser) | **Post** /api/latest/admin/users/add-group | Add user to group
[**AddUserToGroup**](PermissionManagementApi.md#AddUserToGroup) | **Post** /api/latest/admin/groups/add-user | Add user to group
[**AddUserToGroups**](PermissionManagementApi.md#AddUserToGroups) | **Post** /api/latest/admin/users/add-groups | Add user to groups
[**AddUsersToGroup**](PermissionManagementApi.md#AddUsersToGroup) | **Post** /api/latest/admin/groups/add-users | Add multiple users to group
[**ClearUserCaptchaChallenge**](PermissionManagementApi.md#ClearUserCaptchaChallenge) | **Delete** /api/latest/admin/users/captcha | Clear CAPTCHA for user
[**CreateGroup**](PermissionManagementApi.md#CreateGroup) | **Post** /api/latest/admin/groups | Create group
[**CreateUser**](PermissionManagementApi.md#CreateUser) | **Post** /api/latest/admin/users | Create user
[**DeleteGroup**](PermissionManagementApi.md#DeleteGroup) | **Delete** /api/latest/admin/groups | Remove group
[**DeleteUser**](PermissionManagementApi.md#DeleteUser) | **Delete** /api/latest/admin/users | Remove user
[**EraseUser**](PermissionManagementApi.md#EraseUser) | **Post** /api/latest/admin/users/erasure | Erase user information
[**FindGroupsForUser**](PermissionManagementApi.md#FindGroupsForUser) | **Get** /api/latest/admin/users/more-members | Get groups for user
[**FindOtherGroupsForUser**](PermissionManagementApi.md#FindOtherGroupsForUser) | **Get** /api/latest/admin/users/more-non-members | Find other groups for user
[**FindUsersInGroup**](PermissionManagementApi.md#FindUsersInGroup) | **Get** /api/latest/admin/groups/more-members | Get group members
[**FindUsersNotInGroup**](PermissionManagementApi.md#FindUsersNotInGroup) | **Get** /api/latest/admin/groups/more-non-members | Get members not in group
[**GetGroups**](PermissionManagementApi.md#GetGroups) | **Get** /api/latest/groups | Get group names
[**GetGroups1**](PermissionManagementApi.md#GetGroups1) | **Get** /api/latest/admin/groups | Get groups
[**GetGroupsWithAnyPermission**](PermissionManagementApi.md#GetGroupsWithAnyPermission) | **Get** /api/latest/admin/permissions/groups | Get groups with a global permission
[**GetGroupsWithAnyPermission2**](PermissionManagementApi.md#GetGroupsWithAnyPermission2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/groups | Get groups with permission to repository
[**GetGroupsWithoutAnyPermission**](PermissionManagementApi.md#GetGroupsWithoutAnyPermission) | **Get** /api/latest/admin/permissions/groups/none | Get groups with no global permission
[**GetGroupsWithoutAnyPermission2**](PermissionManagementApi.md#GetGroupsWithoutAnyPermission2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/groups/none | Get groups without repository permission
[**GetUserDirectories**](PermissionManagementApi.md#GetUserDirectories) | **Get** /api/latest/admin/user-directories | Get directories
[**GetUsers1**](PermissionManagementApi.md#GetUsers1) | **Get** /api/latest/admin/users | Get users
[**GetUsersWithAnyPermission**](PermissionManagementApi.md#GetUsersWithAnyPermission) | **Get** /api/latest/admin/permissions/users | Get users with a global permission
[**GetUsersWithAnyPermission2**](PermissionManagementApi.md#GetUsersWithAnyPermission2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/users | Get users with permission to repository
[**GetUsersWithoutAnyPermission**](PermissionManagementApi.md#GetUsersWithoutAnyPermission) | **Get** /api/latest/admin/permissions/users/none | Get users with no global permission
[**GetUsersWithoutPermission1**](PermissionManagementApi.md#GetUsersWithoutPermission1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/users/none | Get users without repository permission
[**RemoveGroupFromUser**](PermissionManagementApi.md#RemoveGroupFromUser) | **Post** /api/latest/admin/users/remove-group | Remove user from group
[**RemoveUserFromGroup**](PermissionManagementApi.md#RemoveUserFromGroup) | **Post** /api/latest/admin/groups/remove-user | Remove user from group
[**RenameUser**](PermissionManagementApi.md#RenameUser) | **Post** /api/latest/admin/users/rename | Rename user
[**RevokePermissions1**](PermissionManagementApi.md#RevokePermissions1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions | Revoke all repository permissions for users and groups
[**RevokePermissionsForGroup**](PermissionManagementApi.md#RevokePermissionsForGroup) | **Delete** /api/latest/admin/permissions/groups | Revoke all global permissions for group
[**RevokePermissionsForGroup2**](PermissionManagementApi.md#RevokePermissionsForGroup2) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/groups | Revoke group repository permission
[**RevokePermissionsForUser**](PermissionManagementApi.md#RevokePermissionsForUser) | **Delete** /api/latest/admin/permissions/users | Revoke all global permissions for user
[**RevokePermissionsForUser2**](PermissionManagementApi.md#RevokePermissionsForUser2) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/users | Revoke user repository permission
[**SearchPermissions1**](PermissionManagementApi.md#SearchPermissions1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/search | Search repository permissions
[**SetPermissionForGroup**](PermissionManagementApi.md#SetPermissionForGroup) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/groups | Update group repository permission
[**SetPermissionForGroups**](PermissionManagementApi.md#SetPermissionForGroups) | **Put** /api/latest/admin/permissions/groups | Update global permission for group
[**SetPermissionForUser**](PermissionManagementApi.md#SetPermissionForUser) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/permissions/users | Update user repository permission
[**SetPermissionForUsers**](PermissionManagementApi.md#SetPermissionForUsers) | **Put** /api/latest/admin/permissions/users | Update global permission for user
[**UpdateUserDetails**](PermissionManagementApi.md#UpdateUserDetails) | **Put** /api/latest/admin/users | Update user details
[**UpdateUserPassword**](PermissionManagementApi.md#UpdateUserPassword) | **Put** /api/latest/admin/users/credentials | Set password for user
[**ValidateErasable**](PermissionManagementApi.md#ValidateErasable) | **Get** /api/latest/admin/users/erasure | Check user removal

# **AddGroupToUser**
> AddGroupToUser(ctx, optional)
Add user to group

<strong>Deprecated since 2.10</strong>. Use /rest/users/add-groups instead.  Add a user to a group. This is very similar to <code>groups/add-user</code>, but with the <em>context</em> and <em>itemName</em> attributes of the supplied request entity reversed. On the face of it this may appear redundant, but it facilitates a specific UI component in the application.  In the request entity, the <em>context</em> attribute is the user and the <em>itemName</em> is the group.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiAddGroupToUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiAddGroupToUserOpts struct
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
 **optional** | ***PermissionManagementApiAddUserToGroupOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiAddUserToGroupOpts struct
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

# **AddUserToGroups**
> AddUserToGroups(ctx, optional)
Add user to groups

Add a user to one or more groups.    The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiAddUserToGroupsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiAddUserToGroupsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of UserAndGroups**](UserAndGroups.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AddUsersToGroup**
> AddUsersToGroup(ctx, optional)
Add multiple users to group

Add multiple users to a group.   The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiAddUsersToGroupOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiAddUsersToGroupOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of GroupAndUsers**](GroupAndUsers.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ClearUserCaptchaChallenge**
> ClearUserCaptchaChallenge(ctx, name)
Clear CAPTCHA for user

Clears any CAPTCHA challenge that may constrain the user with the supplied username when they authenticate. Additionally any counter or metric that contributed towards the user being issued the CAPTCHA challenge (for instance too many consecutive failed logins) will also be reset.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource, and may not clear the CAPTCHA of a user with greater permissions than themselves.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| The username | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateGroup**
> RestDetailedGroup CreateGroup(ctx, name)
Create group

Create a new group.   The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| Name of the group. | 

### Return type

[**RestDetailedGroup**](RestDetailedGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateUser**
> CreateUser(ctx, emailAddress, displayName, name, optional)
Create user

Creates a new user from the assembled query parameters.  The default group can be used to control initial permissions for new users, such as granting users the ability to login or providing read access to certain projects or repositories. If the user is not added to the default group, they may not be able to login after their account is created until explicit permissions are configured.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **emailAddress** | **string**| The e-mail address for the new user. | 
  **displayName** | **string**| The display name for the new user. | 
  **name** | **string**| The username for the new user. | 
 **optional** | ***PermissionManagementApiCreateUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiCreateUserOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **password** | **optional.String**| The password for the new user. Required if the &lt;code&gt;notify&lt;/code&gt; parameter is not present or is set to &lt;code&gt;false&lt;/false&gt; | 
 **addToDefaultGroup** | **optional.Bool**| Set &lt;code&gt;true&lt;/code&gt; to add the user to the default group, which can be used to grant them a set of initial permissions; otherwise, &lt;code&gt;false&lt;/code&gt; to not add them to a group. | [default to true]
 **notify** | **optional.Bool**| If present and not &lt;code&gt;false&lt;/code&gt; instead of requiring a password, the create user will be notified via email their account has been created and requires a password to be reset. This option can only be used if a mail server has been configured. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteGroup**
> RestDetailedGroup DeleteGroup(ctx, name)
Remove group

Deletes the specified group, removing them from the system. This also removes any permissions that may have been granted to the group.  A user may not delete the last group that is granting them administrative permissions, or a group with greater permissions than themselves.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| The name identifying the group to delete. | 

### Return type

[**RestDetailedGroup**](RestDetailedGroup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteUser**
> RestDetailedUser DeleteUser(ctx, name)
Remove user

Deletes the specified user, removing them from the system. This also removes any permissions that may have been granted to the user.  A user may not delete themselves, and a user with <strong>ADMIN</strong> permissions may not delete a user with <strong>SYS_ADMIN</strong>permissions.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| The username identifying the user to delete. | 

### Return type

[**RestDetailedUser**](RestDetailedUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EraseUser**
> RestErasedUser EraseUser(ctx, name)
Erase user information

Erases personally identifying user data for a deleted user.  References in the application to the original username will be either removed or updated to a new non-identifying username. Refer to the <a href=\"https://confluence.atlassian.com/gdpr/bitbucket-right-to-erasure-949770560.html\">support guide</a> for details about what data is and isn't erased.  User erasure can only be performed on a deleted user. If the user has not been deleted first then this endpoint will return a bad request and no erasure will be performed.  Erasing user data is <strong>irreversible</strong> and may lead to a degraded user experience. This method should not be used as part of a standard user deletion and cleanup process.  Plugins can participate in user erasure by defining a <code>&lt;user-erasure-handler&gt;</code> module. If one or more plugin modules fail, an error summary of the failing modules is returned.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| The username identifying the user to erase. | 

### Return type

[**RestErasedUser**](RestErasedUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindGroupsForUser**
> InlineResponse20017 FindGroupsForUser(ctx, context, optional)
Get groups for user

Retrieves a list of users that are <em>not</em> members of a specified group. <p>The authenticated user must have the <strong>LICENSED_USER</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **context** | **string**| The group which should be used to locate members. | 
 **optional** | ***PermissionManagementApiFindGroupsForUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiFindGroupsForUserOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only users with usernames, display names or email addresses containing the supplied string will be returned. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20017**](inline_response_200_17.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindOtherGroupsForUser**
> InlineResponse20016 FindOtherGroupsForUser(ctx, context, optional)
Find other groups for user

Retrieves a list of groups the specified user is <em>not</em> a member of. <p>The authenticated user must have the <strong>LICENSED_USER</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **context** | **string**| The user which should be used to locate groups. | 
 **optional** | ***PermissionManagementApiFindOtherGroupsForUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiFindOtherGroupsForUserOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only groups with names containing the supplied string will be returned. | 
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

# **FindUsersInGroup**
> InlineResponse20017 FindUsersInGroup(ctx, context, optional)
Get group members

Retrieves a list of users that are members of a specified group. <p>The authenticated user must have the <strong>LICENSED_USER</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **context** | **string**| The group which should be used to locate members. | 
 **optional** | ***PermissionManagementApiFindUsersInGroupOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiFindUsersInGroupOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only users with usernames, display names or email addresses containing the supplied string will be returned. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20017**](inline_response_200_17.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindUsersNotInGroup**
> InlineResponse20017 FindUsersNotInGroup(ctx, context, optional)
Get members not in group

Retrieves a list of users that are <em>not</em> members of a specified group. <p>The authenticated user must have the <strong>LICENSED_USER</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **context** | **string**| The group which should be used to locate members. | 
 **optional** | ***PermissionManagementApiFindUsersNotInGroupOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiFindUsersNotInGroupOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only users with usernames, display names or email addresses containing the supplied string will be returned. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20017**](inline_response_200_17.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetGroups**
> InlineResponse20023 GetGroups(ctx, optional)
Get group names

Retrieve a page of group names.  The authenticated user must have <strong>LICENSED_USER</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetGroupsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetGroupsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**|  | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20023**](inline_response_200_23.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetGroups1**
> InlineResponse20016 GetGroups1(ctx, optional)
Get groups

Retrieve a page of groups.   The authenticated user must have <strong>LICENSED_USER</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetGroups1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetGroups1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**| If specified only group names containing the supplied string will be returned. | 
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

# **GetGroupsWithAnyPermission**
> InlineResponse20018 GetGroupsWithAnyPermission(ctx, optional)
Get groups with a global permission

Retrieve a page of groups that have been granted at least one global permission.   The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetGroupsWithAnyPermissionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetGroupsWithAnyPermissionOpts struct
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

# **GetGroupsWithAnyPermission2**
> InlineResponse20018 GetGroupsWithAnyPermission2(ctx, projectKey, repositorySlug, optional)
Get groups with permission to repository

Retrieve a page of groups that have been granted at least one permission for the specified repository.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PermissionManagementApiGetGroupsWithAnyPermission2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetGroupsWithAnyPermission2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| If specified only group names containing the supplied string will be returned. | 
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

# **GetGroupsWithoutAnyPermission**
> InlineResponse20016 GetGroupsWithoutAnyPermission(ctx, optional)
Get groups with no global permission

Retrieve a page of groups that have no granted global permissions.   The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetGroupsWithoutAnyPermissionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetGroupsWithoutAnyPermissionOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**| If specified only user names containing the supplied string will be returned | 
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

# **GetGroupsWithoutAnyPermission2**
> InlineResponse20016 GetGroupsWithoutAnyPermission2(ctx, projectKey, repositorySlug, optional)
Get groups without repository permission

Retrieve a page of groups that have no granted permissions for the specified repository.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PermissionManagementApiGetGroupsWithoutAnyPermission2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetGroupsWithoutAnyPermission2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| If specified only group names containing the supplied string will be returned. | 
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

# **GetUserDirectories**
> RestUserDirectory GetUserDirectories(ctx, optional)
Get directories

Retrieve a list of active directories.    The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetUserDirectoriesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetUserDirectoriesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **includeInactive** | **optional.String**| Set &lt;code&gt;true&lt;/code&gt; to include inactive directories; otherwise, &lt;code&gt;false&lt;/code&gt; to only return active directories. | 

### Return type

[**RestUserDirectory**](RestUserDirectory.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUsers1**
> InlineResponse20017 GetUsers1(ctx, optional)
Get users

Retrieve a page of users.    The authenticated user must have the <strong>LICENSED_USER</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetUsers1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetUsers1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**| If specified only users with usernames, display name or email addresses containing the supplied string will be returned. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20017**](inline_response_200_17.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUsersWithAnyPermission**
> InlineResponse20018 GetUsersWithAnyPermission(ctx, optional)
Get users with a global permission

Retrieve a page of users that have been granted at least one global permission.   The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetUsersWithAnyPermissionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetUsersWithAnyPermissionOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**| If specified only user names containing the supplied string will be returned | 
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

# **GetUsersWithAnyPermission2**
> InlineResponse20032 GetUsersWithAnyPermission2(ctx, projectKey, repositorySlug, optional)
Get users with permission to repository

Retrieve a page of users that have been granted at least one permission for the specified repository.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PermissionManagementApiGetUsersWithAnyPermission2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetUsersWithAnyPermission2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| If specified only user names containing the supplied string will be returned. | 
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

# **GetUsersWithoutAnyPermission**
> InlineResponse2005 GetUsersWithoutAnyPermission(ctx, optional)
Get users with no global permission

Retrieve a page of users that have no granted global permissions.   The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiGetUsersWithoutAnyPermissionOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetUsersWithoutAnyPermissionOpts struct
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

# **GetUsersWithoutPermission1**
> InlineResponse2005 GetUsersWithoutPermission1(ctx, projectKey, repositorySlug, optional)
Get users without repository permission

Retrieve a page of <i>licensed</i> users that have no granted permissions for the specified repository.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PermissionManagementApiGetUsersWithoutPermission1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiGetUsersWithoutPermission1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| If specified only user names containing the supplied string will be returned. | 
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

# **RemoveGroupFromUser**
> RemoveGroupFromUser(ctx, optional)
Remove user from group

Remove a user from a group. This is very similar to <code>groups/remove-user</code>, but with the <em>context</em> and <em>itemName</em> attributes of the supplied request entity reversed. On the face of it this may appear redundant, but it facilitates a specific UI component in the application.  In the request entity, the <em>context</em> attribute is the user and the <em>itemName</em> is the group.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiRemoveGroupFromUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiRemoveGroupFromUserOpts struct
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

# **RemoveUserFromGroup**
> RemoveUserFromGroup(ctx, optional)
Remove user from group

<strong>Deprecated since 2.10</strong>. Use /rest/users/remove-groups instead.  Remove a user from a group.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.  In the request entity, the <em>context</em> attribute is the group and the <em>itemName</em> is the user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiRemoveUserFromGroupOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiRemoveUserFromGroupOpts struct
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

# **RenameUser**
> RestDetailedUser RenameUser(ctx, optional)
Rename user

Rename a user.   The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiRenameUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiRenameUserOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of UserRename**](UserRename.md)|  | 

### Return type

[**RestDetailedUser**](RestDetailedUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokePermissions1**
> RevokePermissions1(ctx, projectKey, repositorySlug, optional)
Revoke all repository permissions for users and groups

Revoke all permissions for the specified repository for the given groups and users.  The authenticated user must have <strong>PROJECT_ADMIN</strong> permission for the specified repository or a higher global permission to call this resource.  In addition, a user may not revoke a group's permission if their own permission would be revoked as a result, nor may they revoke their own permission unless they have a global permission that already implies that permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PermissionManagementApiRevokePermissions1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiRevokePermissions1Opts struct
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

# **RevokePermissionsForGroup**
> RevokePermissionsForGroup(ctx, name)
Revoke all global permissions for group

Revoke all global permissions for a group.    The authenticated user must have:   - <strong>ADMIN</strong> permission or higher; and - greater or equal permissions than the current permission level of the group (a user may not demote the     permission level of a group with higher permissions than them)   to call this resource. In addition, a user may not revoke a group's permissions if their own permission level would be reduced as a result.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| The name of the group | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokePermissionsForGroup2**
> RevokePermissionsForGroup2(ctx, projectKey, name, repositorySlug)
Revoke group repository permission

Revoke all permissions for the specified repository for a group.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource.  In addition, a user may not revoke a group's permissions if it will reduce their own permission level.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **name** | **string**| The name of the group. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokePermissionsForUser**
> RevokePermissionsForUser(ctx, name)
Revoke all global permissions for user

Revoke all global permissions for a user.   The authenticated user must have:   - <strong>ADMIN</strong> permission or higher; and - greater or equal permissions than the current permission level of the user (a user may not demote the     permission level of a user with higher permissions than them)   to call this resource. In addition, a user may not demote their own permission level.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| The name of the user | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokePermissionsForUser2**
> RevokePermissionsForUser2(ctx, projectKey, name, repositorySlug)
Revoke user repository permission

Revoke all permissions for the specified repository for a user.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource.  In addition, a user may not revoke their own repository permissions if they do not have a higher project or global permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **name** | **string**| The name of the user. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SearchPermissions1**
> SearchPermissions1(ctx, projectKey, repositorySlug, optional)
Search repository permissions

Search direct and implied permissions of users and groups. This endpoint returns a superset of the results returned by the /users and /groups endpoints because it allows filtering by project and global permissions too.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project/global permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***PermissionManagementApiSearchPermissions1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiSearchPermissions1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **permission** | **optional.String**| Permissions to filter by. See the [permissions documentation](https://confluence.atlassian.com/display/BitbucketServer/Using+repository+permissions)for a detailed explanation of what each permission entails. This parameter can be specified multiple times to filter by more than one permission, and can contain repository, project, and global permissions.   | 
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

# **SetPermissionForGroup**
> SetPermissionForGroup(ctx, projectKey, name, permission, repositorySlug)
Update group repository permission

Promote or demote a group's permission level for the specified repository. Available repository permissions are:  - REPO_READ - REPO_WRITE - REPO_ADMIN   See the <a href=\"https://confluence.atlassian.com/display/BitbucketServer/Using+repository+permissions\">Bitbucket Server documentation</a> for a detailed explanation of what each permission entails.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource. In addition, a user may not demote a group's permission level if their own permission level would be reduced as a result.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **name** | [**[]string**](string.md)| The names of the groups. | 
  **permission** | **string**| The permission to grant | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetPermissionForGroups**
> SetPermissionForGroups(ctx, name, permission)
Update global permission for group

Promote or demote a group's global permission level. Available global permissions are:   - LICENSED_USER - PROJECT_CREATE - ADMIN - SYS_ADMIN  See the <a href=\"https://confluence.atlassian.com/display/BitbucketServer/Global+permissions\">Bitbucket Server documentation</a> for a detailed explanation of what each permission entails.   The authenticated user must have:   - <strong>ADMIN</strong> permission or higher; and - the permission they are attempting to grant or higher; and - greater or equal permissions than the current permission level of the group (a user may not demote the     permission level of a group with higher permissions than them)   to call this resource. In addition, a user may not demote a group's permission level if their own permission level would be reduced as a result.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | [**[]string**](string.md)| The names of the groups | 
  **permission** | **string**| The permission to grant | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetPermissionForUser**
> SetPermissionForUser(ctx, projectKey, name, permission, repositorySlug)
Update user repository permission

Promote or demote a user's permission level for the specified repository. Available repository permissions are:  - REPO_READ</li>- REPO_WRITE</li>- REPO_ADMIN</li></ul>See the <a href=\"https://confluence.atlassian.com/display/BitbucketServer/Using+repository+permissions\">Bitbucket Server documentation</a> for a detailed explanation of what each permission entails.  The authenticated user must have <strong>REPO_ADMIN</strong> permission for the specified repository or a higher project or global permission to call this resource. In addition, a user may not reduce their own permission level unless they have a project or global permission that already implies that permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **name** | [**[]string**](string.md)| The names of the users. | 
  **permission** | **string**| The permission to grant | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetPermissionForUsers**
> SetPermissionForUsers(ctx, name, permission)
Update global permission for user

Promote or demote the global permission level of a user. Available global permissions are:   - LICENSED_USER - PROJECT_CREATE - ADMIN - SYS_ADMIN   See the <a href=\"https://confluence.atlassian.com/display/BitbucketServer/Global+permissions\">Bitbucket Server documentation</a> for a detailed explanation of what each permission entails.   The authenticated user must have:   - <strong>ADMIN</strong> permission or higher; and - the permission they are attempting to grant; and - greater or equal permissions than the current permission level of the user (a user may not demote the     permission level of a user with higher permissions than them)   to call this resource. In addition, a user may not demote their own permission level.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | [**[]string**](string.md)| The names of the users | 
  **permission** | **string**| The permission to grant | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateUserDetails**
> RestDetailedUser UpdateUserDetails(ctx, optional)
Update user details

Update a user's details.   The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiUpdateUserDetailsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiUpdateUserDetailsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of UserUpdate**](UserUpdate.md)|  | 

### Return type

[**RestDetailedUser**](RestDetailedUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateUserPassword**
> UpdateUserPassword(ctx, optional)
Set password for user

Update a user's password.   The authenticated user must have the <strong>ADMIN</strong> permission to call this resource, and may not update the password of a user with greater permissions than themselves.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***PermissionManagementApiUpdateUserPasswordOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a PermissionManagementApiUpdateUserPasswordOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of AdminPasswordUpdate**](AdminPasswordUpdate.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ValidateErasable**
> ValidateErasable(ctx, name)
Check user removal

Validate if a user can be erased.  A username is only valid for erasure if it exists as the username of a deleted user. This endpoint will return an appropriate error response if the supplied username is invalid for erasure.  This endpoint does <strong>not</strong> perform the actual user erasure, and will not modify the application in any way.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **name** | **string**| The username of the user to validate erasability for. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

