# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddKey**](SecurityApi.md#AddKey) | **Post** /gpg/latest/keys | Create a GPG key
[**BulkAddExemptRepositories**](SecurityApi.md#BulkAddExemptRepositories) | **Post** /api/latest/secret-scanning/exempt | Bulk exempt repos from secret scanning
[**CreateAllowlistRule**](SecurityApi.md#CreateAllowlistRule) | **Post** /api/latest/projects/{projectKey}/secret-scanning/allowlist | Create project secret scanning allowlist rule
[**CreateAllowlistRule1**](SecurityApi.md#CreateAllowlistRule1) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/allowlist | Create repository secret scanning allowlist rule
[**CreateRule**](SecurityApi.md#CreateRule) | **Post** /api/latest/projects/{projectKey}/secret-scanning/rules | Create project secret scanning rule
[**CreateRule1**](SecurityApi.md#CreateRule1) | **Post** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/rules | Create repository secret scanning rule
[**CreateRule2**](SecurityApi.md#CreateRule2) | **Post** /api/latest/secret-scanning/rules | Create global secret scanning rule
[**DeleteAllowlistRule**](SecurityApi.md#DeleteAllowlistRule) | **Delete** /api/latest/projects/{projectKey}/secret-scanning/allowlist/{id} | Delete a project secret scanning allowlist rule
[**DeleteAllowlistRule1**](SecurityApi.md#DeleteAllowlistRule1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/allowlist/{id} | Delete a repository secret scanning allowlist rule
[**DeleteForUser**](SecurityApi.md#DeleteForUser) | **Delete** /gpg/latest/keys | Delete all GPG keys for user
[**DeleteKey**](SecurityApi.md#DeleteKey) | **Delete** /gpg/latest/keys/{fingerprintOrId} | Delete a GPG key
[**DeleteRule**](SecurityApi.md#DeleteRule) | **Delete** /api/latest/projects/{projectKey}/secret-scanning/rules/{id} | Delete a project secret scanning rule
[**DeleteRule1**](SecurityApi.md#DeleteRule1) | **Delete** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/rules/{id} | Delete a repository secret scanning rule
[**DeleteRule2**](SecurityApi.md#DeleteRule2) | **Delete** /api/latest/secret-scanning/rules/{id} | Delete a global secret scanning rule
[**EditAllowlistRule**](SecurityApi.md#EditAllowlistRule) | **Put** /api/latest/projects/{projectKey}/secret-scanning/allowlist/{id} | Edit an existing project secret scanning allowlist rule
[**EditAllowlistRule1**](SecurityApi.md#EditAllowlistRule1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/allowlist/{id} | Edit an existing repository secret scanning allowlist rule
[**EditRule**](SecurityApi.md#EditRule) | **Put** /api/latest/projects/{projectKey}/secret-scanning/rules/{id} | Edit an existing project secret scanning rule
[**EditRule1**](SecurityApi.md#EditRule1) | **Put** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/rules/{id} | Edit an existing repository secret scanning rule
[**EditRule2**](SecurityApi.md#EditRule2) | **Put** /api/latest/secret-scanning/rules/{id} | Edit a global secret scanning rule.
[**FindExemptReposByScope**](SecurityApi.md#FindExemptReposByScope) | **Get** /api/latest/secret-scanning/exempt | Find all repos exempt from secret scan
[**GetAllowlistRule**](SecurityApi.md#GetAllowlistRule) | **Get** /api/latest/projects/{projectKey}/secret-scanning/allowlist/{id} | Get a project secret scanning allowlist rule
[**GetAllowlistRule1**](SecurityApi.md#GetAllowlistRule1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/allowlist/{id} | Get a repository secret scanning allowlist rule
[**GetKeysForUser**](SecurityApi.md#GetKeysForUser) | **Get** /gpg/latest/keys | Get all GPG keys
[**GetRule**](SecurityApi.md#GetRule) | **Get** /api/latest/projects/{projectKey}/secret-scanning/rules/{id} | Get a project secret scanning rule
[**GetRule1**](SecurityApi.md#GetRule1) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/rules/{id} | Get a repository secret scanning rule
[**GetRule2**](SecurityApi.md#GetRule2) | **Get** /api/latest/secret-scanning/rules/{id} | Get a global secret scanning rule
[**Search1**](SecurityApi.md#Search1) | **Get** /api/latest/projects/{projectKey}/secret-scanning/rules | Find project secret scanning rules
[**Search2**](SecurityApi.md#Search2) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/allowlist | Find repository secret scanning allowlist rules
[**Search3**](SecurityApi.md#Search3) | **Get** /api/latest/projects/{projectKey}/repos/{repositorySlug}/secret-scanning/rules | Find repository secret scanning rules
[**Search4**](SecurityApi.md#Search4) | **Get** /api/latest/secret-scanning/rules | Find global secret scanning rules
[**SearchAllowlistRule**](SecurityApi.md#SearchAllowlistRule) | **Get** /api/latest/projects/{projectKey}/secret-scanning/allowlist | Find project secret scanning allowlist rules

# **AddKey**
> RestGpgKey AddKey(ctx, optional)
Create a GPG key

Add a GPG key to the authenticated user's account. Optionally, users with ADMIN and higher permissions may choose to specify the <code>user</code> parameter to add a GPG key for another user.  Only authenticated users may call this endpoint.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SecurityApiAddKeyOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiAddKeyOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestGpgKey**](RestGpgKey.md)| The request body. | 
 **user** | **optional.**| The name of the user to add a key for (optional; requires ADMIN permission or higher). | 

### Return type

[**RestGpgKey**](RestGpgKey.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **BulkAddExemptRepositories**
> BulkAddExemptRepositories(ctx, optional)
Bulk exempt repos from secret scanning

Bulk exempt a  list of repositories from being scanned for secrets. User must be have global **ADMIN** permissions.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SecurityApiBulkAddExemptRepositoriesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiBulkAddExemptRepositoriesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of []RestRepositorySelector**](RestRepositorySelector.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateAllowlistRule**
> RestSecretScanningAllowlistRule CreateAllowlistRule(ctx, body, projectKey)
Create project secret scanning allowlist rule

Create a new project level secret scanning allowlist rule. Project allowlist rules are used when scanning all non exempt repositories in the provided project.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningAllowlistRuleSetRequest**](RestSecretScanningAllowlistRuleSetRequest.md)| Allowlist rule to create, either the line regular expression or the path regular expression must be present | 
  **projectKey** | **string**| The project key. | 

### Return type

[**RestSecretScanningAllowlistRule**](RestSecretScanningAllowlistRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateAllowlistRule1**
> RestSecretScanningAllowlistRule CreateAllowlistRule1(ctx, body, projectKey, repositorySlug)
Create repository secret scanning allowlist rule

Create a new repository secret scanning allowlist rule. Repository allowlist rules are used when scanning the given repository.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningAllowlistRuleSetRequest**](RestSecretScanningAllowlistRuleSetRequest.md)| Allowlist rule to create, either the line regular expression or the path regular expression must be present | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestSecretScanningAllowlistRule**](RestSecretScanningAllowlistRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRule**
> RestSecretScanningRule CreateRule(ctx, body, projectKey)
Create project secret scanning rule

Create a new project level secret scanning rule. Project rules are used when scanning all non exempt repositories in the provided project.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningRuleSetRequest**](RestSecretScanningRuleSetRequest.md)| Rule to create, either the line regular expression or the path regular expression must be present | 
  **projectKey** | **string**| The project key. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRule1**
> RestSecretScanningRule CreateRule1(ctx, body, projectKey, repositorySlug)
Create repository secret scanning rule

Create a new repository secret scanning rule. Repository rules are used when scanning the given repository.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningRuleSetRequest**](RestSecretScanningRuleSetRequest.md)| Rule to create, either the line regular expression or the path regular expression must be present | 
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateRule2**
> RestSecretScanningRule CreateRule2(ctx, body)
Create global secret scanning rule

Create a new global secret scanning rule. Global rules are used when scanning all non exempt repositories.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningRuleSetRequest**](RestSecretScanningRuleSetRequest.md)| Rule to create, either the line regular expression or the path regular expression must be present | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAllowlistRule**
> DeleteAllowlistRule(ctx, projectKey, id)
Delete a project secret scanning allowlist rule

Delete a project secret scanning allowlist rule with the provided ID.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The allowlist rule id. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAllowlistRule1**
> DeleteAllowlistRule1(ctx, projectKey, id, repositorySlug)
Delete a repository secret scanning allowlist rule

Delete a repository secret scanning allowlist rule with the provided ID.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The allowlist rule id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteForUser**
> DeleteForUser(ctx, optional)
Delete all GPG keys for user

Delete all GPG keys for a supplied user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SecurityApiDeleteForUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiDeleteForUserOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | **optional.String**| The username of the user to delete the keys for. If no username is specified, the GPG keys will be deleted for the currently authenticated user. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteKey**
> DeleteKey(ctx, fingerprintOrId)
Delete a GPG key

Delete the GPG key with the specified ID or Key Fingerprint.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **fingerprintOrId** | **string**| The GPG fingerprint or ID. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRule**
> DeleteRule(ctx, projectKey, id)
Delete a project secret scanning rule

Delete a project secret scanning rule with the provided ID.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The rule id. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRule1**
> DeleteRule1(ctx, projectKey, id, repositorySlug)
Delete a repository secret scanning rule

Delete a repository secret scanning rule with the provided ID.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The rule id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteRule2**
> DeleteRule2(ctx, id)
Delete a global secret scanning rule

Delete a global secret scanning rule with the provided ID

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **id** | **string**| The rule id. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EditAllowlistRule**
> RestSecretScanningAllowlistRule EditAllowlistRule(ctx, body, projectKey, id)
Edit an existing project secret scanning allowlist rule

Edit a project secret scanning allowlist rule.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningAllowlistRuleSetRequest**](RestSecretScanningAllowlistRuleSetRequest.md)|  | 
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The allowlist rule id. | 

### Return type

[**RestSecretScanningAllowlistRule**](RestSecretScanningAllowlistRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EditAllowlistRule1**
> RestSecretScanningAllowlistRule EditAllowlistRule1(ctx, body, projectKey, id, repositorySlug)
Edit an existing repository secret scanning allowlist rule

Edit a repository secret scanning allowlist rule.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningAllowlistRuleSetRequest**](RestSecretScanningAllowlistRuleSetRequest.md)|  | 
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The allowlist rule id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestSecretScanningAllowlistRule**](RestSecretScanningAllowlistRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EditRule**
> RestSecretScanningRule EditRule(ctx, body, projectKey, id)
Edit an existing project secret scanning rule

Edit a project secret scanning rule.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningRuleSetRequest**](RestSecretScanningRuleSetRequest.md)|  | 
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The rule id. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EditRule1**
> RestSecretScanningRule EditRule1(ctx, body, projectKey, id, repositorySlug)
Edit an existing repository secret scanning rule

Edit a repository secret scanning rule.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningRuleSetRequest**](RestSecretScanningRuleSetRequest.md)|  | 
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The rule id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **EditRule2**
> RestSecretScanningRule EditRule2(ctx, body, id)
Edit a global secret scanning rule.

Edit an existing global secret scanning rule

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **body** | [**RestSecretScanningRuleSetRequest**](RestSecretScanningRuleSetRequest.md)|  | 
  **id** | **string**| The rule id. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **FindExemptReposByScope**
> InlineResponse20029 FindExemptReposByScope(ctx, optional)
Find all repos exempt from secret scan

Find all repositories exempt from secret scanning

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SecurityApiFindExemptReposByScopeOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiFindExemptReposByScopeOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order** | **optional.String**| Order by project name followed by repository name either ascending or descending, defaults to ascending. | 
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

# **GetAllowlistRule**
> RestSecretScanningAllowlistRule GetAllowlistRule(ctx, projectKey, id)
Get a project secret scanning allowlist rule

Get a project secret scanning allowlist rule by ID.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The allowlist rule id. | 

### Return type

[**RestSecretScanningAllowlistRule**](RestSecretScanningAllowlistRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllowlistRule1**
> RestSecretScanningAllowlistRule GetAllowlistRule1(ctx, projectKey, id, repositorySlug)
Get a repository secret scanning allowlist rule

Get a repository secret scanning allowlist rule by ID.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The allowlist rule id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestSecretScanningAllowlistRule**](RestSecretScanningAllowlistRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetKeysForUser**
> InlineResponse2007 GetKeysForUser(ctx, optional)
Get all GPG keys

Find all the keys for the currently authenticated user. Optionally, users with ADMIN and higher permissions may choose to specify the <code>user</code> parameter to retrieve GPG keys for another user.  Only authenticated users may call this endpoint.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SecurityApiGetKeysForUserOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiGetKeysForUserOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | **optional.String**| The name of the user to get keys for (optional; requires ADMIN permission or higher). | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse2007**](inline_response_200_7.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRule**
> RestSecretScanningRule GetRule(ctx, projectKey, id)
Get a project secret scanning rule

Get a project secret scanning rule by ID.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The rule id. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRule1**
> RestSecretScanningRule GetRule1(ctx, projectKey, id, repositorySlug)
Get a repository secret scanning rule

Get a repository secret scanning rule by ID.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **id** | **string**| The rule id. | 
  **repositorySlug** | **string**| The repository slug. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRule2**
> RestSecretScanningRule GetRule2(ctx, id)
Get a global secret scanning rule

Get a global secret scanning rule by ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **id** | **string**| The rule id. | 

### Return type

[**RestSecretScanningRule**](RestSecretScanningRule.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Search1**
> InlineResponse20043 Search1(ctx, projectKey, optional)
Find project secret scanning rules

Find project secret scanning rules by filtering.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***SecurityApiSearch1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiSearch1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| Filter names by the provided text | 
 **order** | **optional.String**| Order by | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20043**](inline_response_200_43.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Search2**
> InlineResponse20042 Search2(ctx, projectKey, repositorySlug, optional)
Find repository secret scanning allowlist rules

Find repository secret scanning allowlist rules by filtering.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***SecurityApiSearch2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiSearch2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| Filter names by the provided text | 
 **order** | **optional.String**| Order by | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20042**](inline_response_200_42.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Search3**
> InlineResponse20043 Search3(ctx, projectKey, repositorySlug, optional)
Find repository secret scanning rules

Find repository secret scanning rules by filtering.  Repository **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
  **repositorySlug** | **string**| The repository slug. | 
 **optional** | ***SecurityApiSearch3Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiSearch3Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **filter** | **optional.String**| Filter names by the provided text | 
 **order** | **optional.String**| Order by | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20043**](inline_response_200_43.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Search4**
> InlineResponse20043 Search4(ctx, optional)
Find global secret scanning rules

Find global secret scanning rules by filtering.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SecurityApiSearch4Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiSearch4Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**| Filter by rule name | 
 **order** | **optional.String**| Order by | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20043**](inline_response_200_43.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SearchAllowlistRule**
> InlineResponse20042 SearchAllowlistRule(ctx, projectKey, optional)
Find project secret scanning allowlist rules

Find project secret scanning allowlist rules by filtering.  Project **Admin** is required

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **projectKey** | **string**| The project key. | 
 **optional** | ***SecurityApiSearchAllowlistRuleOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SecurityApiSearchAllowlistRuleOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **filter** | **optional.String**| Filter names by the provided text | 
 **order** | **optional.String**| Order by | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20042**](inline_response_200_42.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

