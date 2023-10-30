# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Accept**](MirroringUpstreamApi.md#Accept) | **Post** /mirroring/latest/requests/{mirroringRequestId}/accept | Accept a mirroring request
[**AnalyticsSettings**](MirroringUpstreamApi.md#AnalyticsSettings) | **Get** /mirroring/latest/analyticsSettings | Get analytics settings from upstream
[**Authenticate**](MirroringUpstreamApi.md#Authenticate) | **Post** /mirroring/latest/authenticate | Authenticate on behalf of a user
[**DeleteMirroringRequest**](MirroringUpstreamApi.md#DeleteMirroringRequest) | **Delete** /mirroring/latest/requests/{mirroringRequestId} | Delete a mirroring request
[**DeletePreferredMirrorId**](MirroringUpstreamApi.md#DeletePreferredMirrorId) | **Delete** /mirroring/latest/account/settings/preferred-mirror | Remove preferred mirror
[**GetAllContentHashes**](MirroringUpstreamApi.md#GetAllContentHashes) | **Get** /mirroring/latest/repos | Get content hashes for repositories
[**GetAllReposForProject**](MirroringUpstreamApi.md#GetAllReposForProject) | **Get** /mirroring/latest/projects/{projectId}/repos | Get hashes for repositories in project
[**GetContentHashById**](MirroringUpstreamApi.md#GetContentHashById) | **Get** /mirroring/latest/repos/{repoId} | Get content hash for a repository
[**GetMirror**](MirroringUpstreamApi.md#GetMirror) | **Get** /mirroring/latest/mirrorServers/{mirrorId} | Get mirror by ID
[**GetMirroringRequest**](MirroringUpstreamApi.md#GetMirroringRequest) | **Get** /mirroring/latest/requests/{mirroringRequestId} | Get a mirroring request
[**GetPanelHtml**](MirroringUpstreamApi.md#GetPanelHtml) | **Get** /mirroring/latest/mirrorServers/{mirrorId}/webPanels/config | Get HTML for remote-connect web-panel on mirror
[**GetPreferredMirrorId**](MirroringUpstreamApi.md#GetPreferredMirrorId) | **Get** /mirroring/latest/account/settings/preferred-mirror | Get preferred mirror
[**GetProjectById**](MirroringUpstreamApi.md#GetProjectById) | **Get** /mirroring/latest/projects/{projectId} | Get project
[**GetRepositoryMirrors**](MirroringUpstreamApi.md#GetRepositoryMirrors) | **Get** /mirroring/latest/repos/{repoId}/mirrors | Get mirrors for repository
[**ListMirrors**](MirroringUpstreamApi.md#ListMirrors) | **Get** /mirroring/latest/mirrorServers | Get all mirrors
[**ListRequests**](MirroringUpstreamApi.md#ListRequests) | **Get** /mirroring/latest/requests | Get mirroring requests
[**PublishEvent**](MirroringUpstreamApi.md#PublishEvent) | **Post** /mirroring/latest/mirrorServers/{mirrorId}/events | Publish RepositoryMirrorEvent
[**Register**](MirroringUpstreamApi.md#Register) | **Post** /mirroring/latest/requests | Create a mirroring request
[**Reject**](MirroringUpstreamApi.md#Reject) | **Post** /mirroring/latest/requests/{mirroringRequestId}/reject | Reject a mirroring request
[**Remove**](MirroringUpstreamApi.md#Remove) | **Delete** /mirroring/latest/mirrorServers/{mirrorId} | Delete mirror by ID
[**SetPreferredMirrorId**](MirroringUpstreamApi.md#SetPreferredMirrorId) | **Post** /mirroring/latest/account/settings/preferred-mirror | Set preferred mirror
[**Upgrade**](MirroringUpstreamApi.md#Upgrade) | **Put** /mirroring/latest/mirrorServers/{mirrorId} | Upgrade add-on for a mirror

# **Accept**
> RestMirrorServer Accept(ctx, mirroringRequestId)
Accept a mirroring request

Accepts a mirroring request

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirroringRequestId** | **string**| the ID of the request to accept | 

### Return type

[**RestMirrorServer**](RestMirrorServer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AnalyticsSettings**
> RestAnalyticsSettings AnalyticsSettings(ctx, )
Get analytics settings from upstream

Gets the analytics settings from the mirroring upstream

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestAnalyticsSettings**](RestAnalyticsSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Authenticate**
> RestApplicationUserWithPermissions Authenticate(ctx, optional)
Authenticate on behalf of a user

Authenticates on behalf of a user. Used by mirrors to check the credentials supplied to them by users. If successful a user and their effective permissions are returned as follows -  * For SSH credentials - all the effective user permissions are returned. * For all other credentials - the highest global permission is returned along with highest repository permission if repository ID is also provided in the request.  Currently only username/password, bearer token and SSH credentials are supported.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MirroringUpstreamApiAuthenticateOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiAuthenticateOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestAuthenticationRequest**](RestAuthenticationRequest.md)|  | 

### Return type

[**RestApplicationUserWithPermissions**](RestApplicationUserWithPermissions.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteMirroringRequest**
> DeleteMirroringRequest(ctx, mirroringRequestId)
Delete a mirroring request

Deletes a mirroring request

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirroringRequestId** | **string**| the ID of the mirroring request to delete | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeletePreferredMirrorId**
> DeletePreferredMirrorId(ctx, )
Remove preferred mirror

Removes the current user's preferred mirror

### Required Parameters
This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllContentHashes**
> EnrichedRepository GetAllContentHashes(ctx, optional)
Get content hashes for repositories

Returns a page of repositories enriched with a content hash and default branch

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MirroringUpstreamApiGetAllContentHashesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiGetAllContentHashesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **includeDefaultBranch** | **optional.String**| includes defaultBranchId for each repository in the response, if &lt;code&gt;true&lt;/code&gt;. Default value is &lt;code&gt;false&lt;/code&gt;. | [default to false]

### Return type

[**EnrichedRepository**](EnrichedRepository.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllReposForProject**
> InlineResponse20011 GetAllReposForProject(ctx, projectId, optional)
Get hashes for repositories in project

Returns a page of repositories for a given project, enriched with a content hash

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectId** | **string**| the id of the requested project | 
 **optional** | ***MirroringUpstreamApiGetAllReposForProjectOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiGetAllReposForProjectOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **includeDefaultBranch** | **optional.String**| includes defaultBranchId in the response, if &lt;code&gt;true&lt;/code&gt;. Default value is &lt;code&gt;false&lt;/code&gt; | [default to false]
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20011**](inline_response_200_11.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetContentHashById**
> EnrichedRepository GetContentHashById(ctx, repoId, optional)
Get content hash for a repository

Returns a repository enriched with a content hash and default branch

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **repoId** | **string**| the ID of the requested repository | 
 **optional** | ***MirroringUpstreamApiGetContentHashByIdOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiGetContentHashByIdOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **includeDefaultBranch** | **optional.Bool**|  | [default to false]

### Return type

[**EnrichedRepository**](EnrichedRepository.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetMirror**
> RestMirrorServer GetMirror(ctx, mirrorId)
Get mirror by ID

Returns the mirror specified by a mirror ID

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirrorId** | **string**| the mirror ID | 

### Return type

[**RestMirrorServer**](RestMirrorServer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetMirroringRequest**
> RestMirroringRequest GetMirroringRequest(ctx, mirroringRequestId)
Get a mirroring request

Retrieves a mirroring request

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirroringRequestId** | **string**| the ID of the mirroring request to retrieve | 

### Return type

[**RestMirroringRequest**](RestMirroringRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPanelHtml**
> GetPanelHtml(ctx, mirrorId)
Get HTML for remote-connect web-panel on mirror

Gets the rendered HTML that is needed to get the remote connect web-panel on the mirror.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirrorId** | **string**|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/html

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPreferredMirrorId**
> RestMirrorServer GetPreferredMirrorId(ctx, )
Get preferred mirror

Retrieves the current user's preferred mirror server

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestMirrorServer**](RestMirrorServer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetProjectById**
> RestProject GetProjectById(ctx, projectId)
Get project

Returns the requested project using its primary key ID.<br> Since 6.7

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectId** | **string**| the ID of the requested project | 

### Return type

[**RestProject**](RestProject.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositoryMirrors**
> RestMirroredRepositoryDescriptor GetRepositoryMirrors(ctx, repoId)
Get mirrors for repository

Returns a page of mirrors for a repository. This resource will return <strong>all mirrors</strong> along with authorized links to the mirror's repository REST resource. To determine if a repository is available on the mirror, the returned URL needs to be called.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **repoId** | **string**| the ID of the requested repository | 

### Return type

[**RestMirroredRepositoryDescriptor**](RestMirroredRepositoryDescriptor.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListMirrors**
> InlineResponse20010 ListMirrors(ctx, optional)
Get all mirrors

Returns a list of mirrors

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MirroringUpstreamApiListMirrorsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiListMirrorsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20010**](inline_response_200_10.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ListRequests**
> InlineResponse20012 ListRequests(ctx, optional)
Get mirroring requests

Retrieves a mirroring request

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MirroringUpstreamApiListRequestsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiListRequestsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **state** | **optional.String**| (optional) the request state to filter on | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20012**](inline_response_200_12.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PublishEvent**
> PublishEvent(ctx, mirrorId, optional)
Publish RepositoryMirrorEvent

Publishes a RepositoryMirrorEvent on the event queue.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirrorId** | **string**| the server id of the mirror that raised this event | 
 **optional** | ***MirroringUpstreamApiPublishEventOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiPublishEventOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestRepositoryMirrorEvent**](RestRepositoryMirrorEvent.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Register**
> RestMirroringRequest Register(ctx, optional)
Create a mirroring request

Creates a new mirroring request

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MirroringUpstreamApiRegisterOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiRegisterOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestMirroringRequest**](RestMirroringRequest.md)|  | 

### Return type

[**RestMirroringRequest**](RestMirroringRequest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Reject**
> RestMirrorServer Reject(ctx, mirroringRequestId)
Reject a mirroring request

Rejects a mirroring request

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirroringRequestId** | **string**| the ID of the request to reject | 

### Return type

[**RestMirrorServer**](RestMirrorServer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Remove**
> Remove(ctx, mirrorId)
Delete mirror by ID

Removes a mirror, disabling all access and notifications for the mirror server in question

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirrorId** | **string**| the ID of the mirror to remove | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetPreferredMirrorId**
> SetPreferredMirrorId(ctx, optional)
Set preferred mirror

Sets the mirror specified by a mirror ID as the current user's preferred mirror

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MirroringUpstreamApiSetPreferredMirrorIdOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiSetPreferredMirrorIdOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of string**](string.md)| the mirror ID | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Upgrade**
> RestMirrorServer Upgrade(ctx, mirrorId, optional)
Upgrade add-on for a mirror

Upgrades the add-on for the mirror server in question This endpoint can only be called by the mirror instance or system administrators<br>Since 5.8

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **mirrorId** | **string**| the ID of the mirror to upgrade | 
 **optional** | ***MirroringUpstreamApiUpgradeOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MirroringUpstreamApiUpgradeOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestMirrorUpgradeRequest**](RestMirrorUpgradeRequest.md)|  | 

### Return type

[**RestMirrorServer**](RestMirrorServer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

