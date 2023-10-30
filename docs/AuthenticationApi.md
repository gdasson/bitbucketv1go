# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddForProject**](AuthenticationApi.md#AddForProject) | **Post** /keys/latest/projects/{projectKey}/ssh | Add project SSH key
[**AddForRepository**](AuthenticationApi.md#AddForRepository) | **Post** /keys/latest/projects/{projectKey}/repos/{repositorySlug}/ssh | Add repository SSH key
[**AddSshKey**](AuthenticationApi.md#AddSshKey) | **Post** /ssh/latest/keys | Add SSH key for user
[**CreateAccessToken1**](AuthenticationApi.md#CreateAccessToken1) | **Put** /access-tokens/latest/projects/{projectKey} | Create project HTTP token
[**CreateAccessToken2**](AuthenticationApi.md#CreateAccessToken2) | **Put** /access-tokens/latest/projects/{projectKey}/repos/{repositorySlug} | Create repository HTTP token
[**CreateAccessToken3**](AuthenticationApi.md#CreateAccessToken3) | **Put** /access-tokens/latest/users/{userSlug} | Create personal HTTP token
[**DeleteById**](AuthenticationApi.md#DeleteById) | **Delete** /access-tokens/latest/projects/{projectKey}/{tokenId} | Delete a HTTP token
[**DeleteById1**](AuthenticationApi.md#DeleteById1) | **Delete** /access-tokens/latest/projects/{projectKey}/repos/{repositorySlug}/{tokenId} | Delete a HTTP token
[**DeleteById2**](AuthenticationApi.md#DeleteById2) | **Delete** /access-tokens/latest/users/{userSlug}/{tokenId} | Delete a HTTP token
[**DeleteSshKey**](AuthenticationApi.md#DeleteSshKey) | **Delete** /ssh/latest/keys/{keyId} | Remove SSH key
[**DeleteSshKeys**](AuthenticationApi.md#DeleteSshKeys) | **Delete** /ssh/latest/keys | Delete all user SSH key
[**GetAllAccessTokens**](AuthenticationApi.md#GetAllAccessTokens) | **Get** /access-tokens/latest/projects/{projectKey} | Get project HTTP tokens
[**GetAllAccessTokens1**](AuthenticationApi.md#GetAllAccessTokens1) | **Get** /access-tokens/latest/projects/{projectKey}/repos/{repositorySlug} | Get repository HTTP tokens
[**GetAllAccessTokens2**](AuthenticationApi.md#GetAllAccessTokens2) | **Get** /access-tokens/latest/users/{userSlug} | Get personal HTTP tokens
[**GetById**](AuthenticationApi.md#GetById) | **Get** /access-tokens/latest/projects/{projectKey}/{tokenId} | Get HTTP token by ID
[**GetById1**](AuthenticationApi.md#GetById1) | **Get** /access-tokens/latest/projects/{projectKey}/repos/{repositorySlug}/{tokenId} | Get HTTP token by ID
[**GetById2**](AuthenticationApi.md#GetById2) | **Get** /access-tokens/latest/users/{userSlug}/{tokenId} | Get HTTP token by ID
[**GetForProject**](AuthenticationApi.md#GetForProject) | **Get** /keys/latest/projects/{projectKey}/ssh/{keyId} | Get project SSH key
[**GetForProjects**](AuthenticationApi.md#GetForProjects) | **Get** /keys/latest/ssh/{keyId}/projects | Get project SSH keys
[**GetForRepositories**](AuthenticationApi.md#GetForRepositories) | **Get** /keys/latest/ssh/{keyId}/repos | Get repository SSH key
[**GetForRepository**](AuthenticationApi.md#GetForRepository) | **Get** /keys/latest/projects/{projectKey}/repos/{repositorySlug}/ssh | Get repository SSH keys
[**GetForRepository1**](AuthenticationApi.md#GetForRepository1) | **Get** /keys/latest/projects/{projectKey}/repos/{repositorySlug}/ssh/{keyId} | Get repository SSH key
[**GetSshKey**](AuthenticationApi.md#GetSshKey) | **Get** /ssh/latest/keys/{keyId} | Get SSH key for user by keyId
[**GetSshKeys**](AuthenticationApi.md#GetSshKeys) | **Get** /ssh/latest/keys | Get SSH keys for user
[**GetSshKeysForProject**](AuthenticationApi.md#GetSshKeysForProject) | **Get** /keys/latest/projects/{projectKey}/ssh | Get SSH key
[**RevokeForProject**](AuthenticationApi.md#RevokeForProject) | **Delete** /keys/latest/projects/{projectKey}/ssh/{keyId} | Revoke project SSH key
[**RevokeForRepository**](AuthenticationApi.md#RevokeForRepository) | **Delete** /keys/latest/projects/{projectKey}/repos/{repositorySlug}/ssh/{keyId} | Revoke repository SSH key
[**RevokeMany**](AuthenticationApi.md#RevokeMany) | **Delete** /keys/latest/ssh/{keyId} | Revoke project SSH key
[**SshSettings**](AuthenticationApi.md#SshSettings) | **Get** /ssh/latest/settings | Get SSH settings
[**UpdateAccessToken**](AuthenticationApi.md#UpdateAccessToken) | **Post** /access-tokens/latest/projects/{projectKey}/{tokenId} | Update HTTP token
[**UpdateAccessToken1**](AuthenticationApi.md#UpdateAccessToken1) | **Post** /access-tokens/latest/projects/{projectKey}/repos/{repositorySlug}/{tokenId} | Update HTTP token
[**UpdateAccessToken2**](AuthenticationApi.md#UpdateAccessToken2) | **Post** /access-tokens/latest/users/{userSlug}/{tokenId} | Update HTTP token
[**UpdatePermission**](AuthenticationApi.md#UpdatePermission) | **Put** /keys/latest/projects/{projectKey}/ssh/{keyId}/permission/{permission} | Update project SSH key permission
[**UpdatePermission1**](AuthenticationApi.md#UpdatePermission1) | **Put** /keys/latest/projects/{projectKey}/repos/{repositorySlug}/ssh/{keyId}/permission/{permission} | Update repository SSH key permission

# **AddForProject**
> RestSshAccessKey AddForProject(ctx, projectKey, optional)
Add project SSH key

Register a new SSH key and grants access to the project identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***AuthenticationApiAddForProjectOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiAddForProjectOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestSshAccessKey**](RestSshAccessKey.md)|  | 

### Return type

[**RestSshAccessKey**](RestSshAccessKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AddForRepository**
> RestSshAccessKey AddForRepository(ctx, projectKey, repositorySlug, optional)
Add repository SSH key

Register a new SSH key and grants access to the repository identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **repositorySlug** | **string**| The repository slug | 
 **optional** | ***AuthenticationApiAddForRepositoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiAddForRepositoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestSshAccessKey**](RestSshAccessKey.md)|  | 

### Return type

[**RestSshAccessKey**](RestSshAccessKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **AddSshKey**
> RestSshKey AddSshKey(ctx, optional)
Add SSH key for user

Add a new SSH key to a supplied user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***AuthenticationApiAddSshKeyOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiAddSshKeyOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of LatestKeysBody**](LatestKeysBody.md)|  | 
 **user** | [**optional.Interface of RestSshKey**](.md)| the username of the user to add the SSH key for. If no username is specified, the SSH key will be added for the current authenticated user. | 

### Return type

[**RestSshKey**](RestSshKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateAccessToken1**
> RestRawAccessToken CreateAccessToken1(ctx, projectKey, optional)
Create project HTTP token

Create an access token for the project according to the given request.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***AuthenticationApiCreateAccessToken1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiCreateAccessToken1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestAccessTokenRequest**](RestAccessTokenRequest.md)| The request containing the details of the access token to create. | 

### Return type

[**RestRawAccessToken**](RestRawAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateAccessToken2**
> RestRawAccessToken CreateAccessToken2(ctx, projectKey, repositorySlug, optional)
Create repository HTTP token

Create an access token for the repository according to the given request.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***AuthenticationApiCreateAccessToken2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiCreateAccessToken2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestAccessTokenRequest**](RestAccessTokenRequest.md)| The request containing the details of the access token to create. | 

### Return type

[**RestRawAccessToken**](RestRawAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateAccessToken3**
> RestRawAccessToken CreateAccessToken3(ctx, userSlug, optional)
Create personal HTTP token

Create an access token for the user according to the given request.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug. | 
 **optional** | ***AuthenticationApiCreateAccessToken3Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiCreateAccessToken3Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestAccessTokenRequest**](RestAccessTokenRequest.md)| The request containing the details of the access token to create. | 

### Return type

[**RestRawAccessToken**](RestRawAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteById**
> DeleteById(ctx, projectKey, tokenId)
Delete a HTTP token

Delete the access token identified by the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **tokenId** | **string**| The token id. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteById1**
> DeleteById1(ctx, projectKey, tokenId, repositorySlug)
Delete a HTTP token

Delete the access token identified by the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **tokenId** | **string**| The token id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteById2**
> DeleteById2(ctx, tokenId, userSlug)
Delete a HTTP token

Delete the access token identified by the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **tokenId** | **string**| The token id. | 
  **userSlug** | **string**| The user slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteSshKey**
> DeleteSshKey(ctx, keyId)
Remove SSH key

Delete an SSH key.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **keyId** | **string**| the id of the key to delete. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteSshKeys**
> DeleteSshKeys(ctx, optional)
Delete all user SSH key

Delete all SSH keys for a supplied user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***AuthenticationApiDeleteSshKeysOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiDeleteSshKeysOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userName** | **optional.String**| the username of the user to delete the keys for. If no username is specified, the SSH keys will be deleted for the current authenticated user. | 
 **user** | **optional.String**|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllAccessTokens**
> InlineResponse200 GetAllAccessTokens(ctx, projectKey, optional)
Get project HTTP tokens

Get all access tokens associated with the given project.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***AuthenticationApiGetAllAccessTokensOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiGetAllAccessTokensOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse200**](inline_response_200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllAccessTokens1**
> InlineResponse200 GetAllAccessTokens1(ctx, projectKey, repositorySlug, optional)
Get repository HTTP tokens

Get all access tokens associated with the given repository.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***AuthenticationApiGetAllAccessTokens1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiGetAllAccessTokens1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse200**](inline_response_200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllAccessTokens2**
> InlineResponse200 GetAllAccessTokens2(ctx, userSlug, optional)
Get personal HTTP tokens

Get all access tokens associated with the given user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug. | 
 **optional** | ***AuthenticationApiGetAllAccessTokens2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiGetAllAccessTokens2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse200**](inline_response_200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetById**
> RestAccessToken GetById(ctx, projectKey, tokenId)
Get HTTP token by ID

Get the access token identified by the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **tokenId** | **string**| The token id. | 

### Return type

[**RestAccessToken**](RestAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetById1**
> RestAccessToken GetById1(ctx, projectKey, tokenId, repositorySlug)
Get HTTP token by ID

Get the access token identified by the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **tokenId** | **string**| The token id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestAccessToken**](RestAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetById2**
> RestAccessToken GetById2(ctx, tokenId, userSlug)
Get HTTP token by ID

Get the access token identified by the given ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **tokenId** | **string**| The token id. | 
  **userSlug** | **string**| The user slug. | 

### Return type

[**RestAccessToken**](RestAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetForProject**
> RestSshAccessKey GetForProject(ctx, projectKey, keyId)
Get project SSH key

Retrieves the access key for the SSH key with id <code>keyId</code> on the project identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **keyId** | **string**| The key id | 

### Return type

[**RestSshAccessKey**](RestSshAccessKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetForProjects**
> GetForProjects(ctx, keyId)
Get project SSH keys

Retrieves all project-related access keys for the SSH key with id <code>keyId</code>. If the current user is not an admin any of the projects the key provides access to, none are returned.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **keyId** | **int32**|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetForRepositories**
> GetForRepositories(ctx, keyId, optional)
Get repository SSH key

Retrieves all repository-related access keys for the SSH key with id <code>keyId</code>. If the current user is not an admin of any of the projects the key provides access to, none are returned.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **keyId** | **string**| The key id | 
 **optional** | ***AuthenticationApiGetForRepositoriesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiGetForRepositoriesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **withRestrictions** | **optional.String**| Include the readOnly field. The &#x60;readOnly&#x60; field is contextual for the user making the request. &#x60;readOnly&#x60; returns true if there is a restriction and the user does not have&#x60;PROJECT_ADMIN&#x60; access for the repository the key is associated with. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetForRepository**
> InlineResponse20014 GetForRepository(ctx, projectKey, repositorySlug, optional)
Get repository SSH keys

Retrieves the access keys for the repository identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***AuthenticationApiGetForRepositoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiGetForRepositoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| If specified only SSH access keys with a label prefixed with the supplied string will be returned | 
 **effective** | **optional.String**| Controls whether SSH access keys configured at the project level should be included in the results or not. When set to &lt;code&gt;true&lt;/code&gt; all keys that have &lt;em&gt;access&lt;/em&gt; to the repository (including project level keys) are included in the results. When set to &lt;code&gt;false&lt;/code&gt;, only access keys configured for the specified &lt;code&gt;repository&lt;/code&gt; are considered. Default is &lt;code&gt;false&lt;/code&gt;. | 
 **minimumPermission** | **optional.String**| If specified only SSH access keys with at least the supplied permission will be returned. Default is &lt;code&gt;Permission.REPO_READ&lt;/code&gt;. | 
 **permission** | **optional.String**|  | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20014**](inline_response_200_14.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetForRepository1**
> RestSshAccessKey GetForRepository1(ctx, projectKey, keyId, repositorySlug)
Get repository SSH key

Retrieves the access key for the SSH key with id <code>keyId</code> on the repository identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **keyId** | **string**| The key id | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

[**RestSshAccessKey**](RestSshAccessKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSshKey**
> RestSshKey GetSshKey(ctx, keyId)
Get SSH key for user by keyId

Retrieve an SSH key by keyId

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **keyId** | **string**| the ID of the key to retrieve. | 

### Return type

[**RestSshKey**](RestSshKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSshKeys**
> InlineResponse20015 GetSshKeys(ctx, optional)
Get SSH keys for user

Retrieve a page of SSH keys.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***AuthenticationApiGetSshKeysOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiGetSshKeysOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userName** | **optional.String**| the username of the user to retrieve the keys for. If no username is specified, the SSH keys will be retrieved for the current authenticated user. | 
 **user** | **optional.String**|  | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20015**](inline_response_200_15.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSshKeysForProject**
> InlineResponse20014 GetSshKeysForProject(ctx, projectKey, optional)
Get SSH key

Retrieves the access keys for the project identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
 **optional** | ***AuthenticationApiGetSshKeysForProjectOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiGetSshKeysForProjectOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| If specified only SSH access keys with a label prefixed with the supplied string will be returned. | 
 **permission** | **optional.String**| If specified only SSH access keys with at least the supplied permission will be returned Default is PROJECT_READ. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20014**](inline_response_200_14.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokeForProject**
> RevokeForProject(ctx, projectKey, keyId)
Revoke project SSH key

Remove an existing access key for the project identified in the URL. If the same SSH key is used as an access key for multiple projects or repositories, only the access to the project identified in the URL will be revoked.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **keyId** | **string**| The key id | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokeForRepository**
> RevokeForRepository(ctx, projectKey, keyId, repositorySlug)
Revoke repository SSH key

Remove an existing access key for the repository identified in the URL. If the same SSH key is used as an access key for multiple projects or repositories, only the access to the repository identified in the URL will be revoked.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **keyId** | **string**| The key id | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RevokeMany**
> RevokeMany(ctx, keyId, optional)
Revoke project SSH key

Remove an existing access key for the projects and repositories in the submitted entity. If the same SSH key is used as an access key for multiple projects or repositories not supplied, only the access to the projects or repositories identified will be revoked.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **keyId** | **string**| The identifier of the SSH key | 
 **optional** | ***AuthenticationApiRevokeManyOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiRevokeManyOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of SshKeyIdBody**](SshKeyIdBody.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SshSettings**
> RestSshSettings SshSettings(ctx, )
Get SSH settings

Gets the SSH settings from the upstream.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestSshSettings**](RestSshSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateAccessToken**
> RestAccessToken UpdateAccessToken(ctx, projectKey, tokenId, optional)
Update HTTP token

Modify an access token according to the given request. Any fields not specified will not be altered.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **tokenId** | **string**| The token id. | 
 **optional** | ***AuthenticationApiUpdateAccessTokenOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiUpdateAccessTokenOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestAccessTokenRequest**](RestAccessTokenRequest.md)| The request containing the details of the access token to modify | 

### Return type

[**RestAccessToken**](RestAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateAccessToken1**
> RestAccessToken UpdateAccessToken1(ctx, projectKey, tokenId, repositorySlug, optional)
Update HTTP token

Modify an access token according to the given request. Any fields not specified will not be altered.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **tokenId** | **string**| The token id. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***AuthenticationApiUpdateAccessToken1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiUpdateAccessToken1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | [**optional.Interface of RestAccessTokenRequest**](RestAccessTokenRequest.md)| The request containing the details of the access token to modify | 

### Return type

[**RestAccessToken**](RestAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateAccessToken2**
> RestAccessToken UpdateAccessToken2(ctx, tokenId, userSlug, optional)
Update HTTP token

Modify an access token according to the given request. Any fields not specified will not be altered.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **tokenId** | **string**| The token id. | 
  **userSlug** | **string**| The user slug. | 
 **optional** | ***AuthenticationApiUpdateAccessToken2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a AuthenticationApiUpdateAccessToken2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | [**optional.Interface of RestAccessTokenRequest**](RestAccessTokenRequest.md)| The request containing the details of the access token to modify | 

### Return type

[**RestAccessToken**](RestAccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdatePermission**
> RestSshAccessKey UpdatePermission(ctx, projectKey, keyId, permission)
Update project SSH key permission

Updates the permission granted to the specified SSH key to the project identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **keyId** | **string**| The newly created access key | 
  **permission** | **string**| The new permission to be granted to the SSH key | 

### Return type

[**RestSshAccessKey**](RestSshAccessKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdatePermission1**
> RestSshAccessKey UpdatePermission1(ctx, projectKey, keyId, permission, repositorySlug)
Update repository SSH key permission

Updates the permission granted to the specified SSH key to the repository identified in the URL.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key | 
  **keyId** | **string**| The newly created access key | 
  **permission** | **string**| The new permission to be granted to the SSH key | 
  **repositorySlug** | **string**| The repository slug | 

### Return type

[**RestSshAccessKey**](RestSshAccessKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

