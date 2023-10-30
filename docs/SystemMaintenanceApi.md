# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelExportJob**](SystemMaintenanceApi.md#CancelExportJob) | **Post** /api/latest/migration/exports/{jobId}/cancel | Cancel export job
[**CancelImportJob**](SystemMaintenanceApi.md#CancelImportJob) | **Post** /api/latest/migration/imports/{jobId}/cancel | Cancel import job
[**CancelMeshMigrationJob**](SystemMaintenanceApi.md#CancelMeshMigrationJob) | **Post** /api/latest/migration/mesh/{jobId}/cancel | Cancel Mesh migration job
[**ClearDefaultBranch**](SystemMaintenanceApi.md#ClearDefaultBranch) | **Delete** /api/latest/admin/default-branch | Clear default branch
[**ClearSenderAddress**](SystemMaintenanceApi.md#ClearSenderAddress) | **Delete** /api/latest/admin/mail-server/sender-address | Update mail configuration
[**Connectivity**](SystemMaintenanceApi.md#Connectivity) | **Get** /api/latest/admin/git/mesh/diagnostics/connectivity | Generate Mesh connectivity report
[**CreateHookScript**](SystemMaintenanceApi.md#CreateHookScript) | **Post** /api/latest/hook-scripts | Create a new hook script
[**Delete2**](SystemMaintenanceApi.md#Delete2) | **Delete** /api/latest/admin/git/mesh/nodes/{id} | Delete Mesh node
[**Delete6**](SystemMaintenanceApi.md#Delete6) | **Delete** /api/latest/admin/rate-limit/settings/users/{userSlug} | Delete user specific rate limit settings
[**DeleteAvatar**](SystemMaintenanceApi.md#DeleteAvatar) | **Delete** /api/latest/users/{userSlug}/avatar.png | Delete user avatar
[**DeleteBanner**](SystemMaintenanceApi.md#DeleteBanner) | **Delete** /api/latest/admin/banner | Delete announcement banner
[**DeleteHookScript**](SystemMaintenanceApi.md#DeleteHookScript) | **Delete** /api/latest/hook-scripts/{scriptId} | Delete a hook script.
[**DeleteMailConfig**](SystemMaintenanceApi.md#DeleteMailConfig) | **Delete** /api/latest/admin/mail-server | Delete mail configuration
[**DismissRetentionConfigReviewNotification**](SystemMaintenanceApi.md#DismissRetentionConfigReviewNotification) | **Delete** /audit/latest/notification-settings/retention-config-review | Dismiss retention config notification
[**Get2**](SystemMaintenanceApi.md#Get2) | **Get** /api/latest/admin/license | Get license details
[**Get4**](SystemMaintenanceApi.md#Get4) | **Get** /api/latest/admin/rate-limit/settings/users/{userSlug} | Get user specific rate limit settings
[**GetActiveMeshMigrationSummary**](SystemMaintenanceApi.md#GetActiveMeshMigrationSummary) | **Get** /api/latest/migration/mesh/summary | Get summary for Mesh migration job
[**GetAllMeshMigrationSummaries**](SystemMaintenanceApi.md#GetAllMeshMigrationSummaries) | **Get** /api/latest/migration/mesh/summaries | Get all Mesh migration job summaries
[**GetAllRateLimitSettings**](SystemMaintenanceApi.md#GetAllRateLimitSettings) | **Get** /api/latest/admin/rate-limit/settings/users | Get rate limit settings for user
[**GetAllRegisteredMeshNodes**](SystemMaintenanceApi.md#GetAllRegisteredMeshNodes) | **Get** /api/latest/admin/git/mesh/nodes | Get all registered Mesh nodes
[**GetApplicationProperties**](SystemMaintenanceApi.md#GetApplicationProperties) | **Get** /api/latest/application-properties | Get application properties
[**GetBanner**](SystemMaintenanceApi.md#GetBanner) | **Get** /api/latest/admin/banner | Get announcement banner
[**GetControlPlanePublicKey**](SystemMaintenanceApi.md#GetControlPlanePublicKey) | **Get** /api/latest/admin/git/mesh/config/control-plane.pem | Get the control plane PEM
[**GetDefaultBranch**](SystemMaintenanceApi.md#GetDefaultBranch) | **Get** /api/latest/admin/default-branch | Get the default branch
[**GetExportJob**](SystemMaintenanceApi.md#GetExportJob) | **Get** /api/latest/migration/exports/{jobId} | Get export job details
[**GetExportJobMessages**](SystemMaintenanceApi.md#GetExportJobMessages) | **Get** /api/latest/migration/exports/{jobId}/messages | Get job messages
[**GetGlobalSettings**](SystemMaintenanceApi.md#GetGlobalSettings) | **Get** /admin | Get global SSH key settings
[**GetHistory**](SystemMaintenanceApi.md#GetHistory) | **Get** /api/latest/admin/rate-limit/history | Get rate limit history
[**GetHookScript**](SystemMaintenanceApi.md#GetHookScript) | **Get** /api/latest/hook-scripts/{scriptId} | Get a hook script
[**GetImportJob**](SystemMaintenanceApi.md#GetImportJob) | **Get** /api/latest/migration/imports/{jobId} | Get import job status
[**GetImportJobMessages**](SystemMaintenanceApi.md#GetImportJobMessages) | **Get** /api/latest/migration/imports/{jobId}/messages | Get import job messages
[**GetInformation**](SystemMaintenanceApi.md#GetInformation) | **Get** /api/latest/admin/cluster | Get cluster node information
[**GetLabel**](SystemMaintenanceApi.md#GetLabel) | **Get** /api/latest/labels/{labelName} | Get label
[**GetLabelables**](SystemMaintenanceApi.md#GetLabelables) | **Get** /api/latest/labels/{labelName}/labeled | Get labelables for label
[**GetLabels**](SystemMaintenanceApi.md#GetLabels) | **Get** /api/latest/labels | Get all labels
[**GetLevel**](SystemMaintenanceApi.md#GetLevel) | **Get** /api/latest/logs/logger/{loggerName} | Get current log level
[**GetMailConfig**](SystemMaintenanceApi.md#GetMailConfig) | **Get** /api/latest/admin/mail-server | Get mail configuration
[**GetMeshMigrationJob**](SystemMaintenanceApi.md#GetMeshMigrationJob) | **Get** /api/latest/migration/mesh/{jobId} | Get Mesh migration job details
[**GetMeshMigrationJobMessages**](SystemMaintenanceApi.md#GetMeshMigrationJobMessages) | **Get** /api/latest/migration/mesh/{jobId}/messages | Get Mesh migration job messages
[**GetMeshMigrationJobSummary**](SystemMaintenanceApi.md#GetMeshMigrationJobSummary) | **Get** /api/latest/migration/mesh/{jobId}/summary | Get Mesh migration job summary
[**GetRegisteredMeshNodeById**](SystemMaintenanceApi.md#GetRegisteredMeshNodeById) | **Get** /api/latest/admin/git/mesh/nodes/{id} | Get Mesh node
[**GetRepositoryArchivePolicy**](SystemMaintenanceApi.md#GetRepositoryArchivePolicy) | **Get** /policies/latest/admin/repos/archive | Get repository archive policy
[**GetRepositoryDeletePolicy**](SystemMaintenanceApi.md#GetRepositoryDeletePolicy) | **Get** /policies/latest/admin/repos/delete | Get repository delete policy
[**GetRootLevel**](SystemMaintenanceApi.md#GetRootLevel) | **Get** /api/latest/logs/rootLogger | Get root log level
[**GetSenderAddress**](SystemMaintenanceApi.md#GetSenderAddress) | **Get** /api/latest/admin/mail-server/sender-address | Get server mail address
[**GetSettings2**](SystemMaintenanceApi.md#GetSettings2) | **Get** /api/latest/admin/rate-limit/settings | Get rate limit settings
[**GetSupportZip**](SystemMaintenanceApi.md#GetSupportZip) | **Get** /api/latest/admin/git/mesh/support-zips/{id} | Get support zip for node
[**GetSupportZips**](SystemMaintenanceApi.md#GetSupportZips) | **Get** /api/latest/admin/git/mesh/support-zips | Get support zips for all Mesh nodes
[**GetSupportedKeyTypes**](SystemMaintenanceApi.md#GetSupportedKeyTypes) | **Get** /admin/supported-key-types | Get supported SSH key algorithms and lengths
[**GetUser**](SystemMaintenanceApi.md#GetUser) | **Get** /api/latest/users/{userSlug} | Get user
[**GetUserSettings**](SystemMaintenanceApi.md#GetUserSettings) | **Get** /api/latest/users/{userSlug}/settings | Get user settings
[**GetUsers2**](SystemMaintenanceApi.md#GetUsers2) | **Get** /api/latest/users | Get all users
[**PreviewExport**](SystemMaintenanceApi.md#PreviewExport) | **Post** /api/latest/migration/exports/preview | Preview export
[**PreviewMeshMigration**](SystemMaintenanceApi.md#PreviewMeshMigration) | **Post** /api/latest/migration/mesh/preview | Preview Mesh migration
[**Read**](SystemMaintenanceApi.md#Read) | **Get** /api/latest/hook-scripts/{scriptId}/content | Get hook script content
[**RegisterNewMeshNode**](SystemMaintenanceApi.md#RegisterNewMeshNode) | **Post** /api/latest/admin/git/mesh/nodes | Register new Mesh node
[**SearchMeshMigrationRepos**](SystemMaintenanceApi.md#SearchMeshMigrationRepos) | **Get** /api/latest/migration/mesh/repos | Find repositories by Mesh migration state
[**Set**](SystemMaintenanceApi.md#Set) | **Post** /api/latest/admin/rate-limit/settings/users | Set rate limit settings for users
[**Set1**](SystemMaintenanceApi.md#Set1) | **Put** /api/latest/admin/rate-limit/settings/users/{userSlug} | Set rate limit settings for user
[**SetBanner**](SystemMaintenanceApi.md#SetBanner) | **Put** /api/latest/admin/banner | Update/Set announcement banner
[**SetDefaultBranch**](SystemMaintenanceApi.md#SetDefaultBranch) | **Put** /api/latest/admin/default-branch | Update/Set default branch
[**SetLevel**](SystemMaintenanceApi.md#SetLevel) | **Put** /api/latest/logs/logger/{loggerName}/{levelName} | Set log level
[**SetMailConfig**](SystemMaintenanceApi.md#SetMailConfig) | **Put** /api/latest/admin/mail-server | Update mail configuration
[**SetRepositoryArchivePolicy**](SystemMaintenanceApi.md#SetRepositoryArchivePolicy) | **Put** /policies/latest/admin/repos/archive | Update repository archive policy
[**SetRepositoryDeletePolicy**](SystemMaintenanceApi.md#SetRepositoryDeletePolicy) | **Put** /policies/latest/admin/repos/delete | Update the repository delete policy
[**SetRootLevel**](SystemMaintenanceApi.md#SetRootLevel) | **Put** /api/latest/logs/rootLogger/{levelName} | Set root log level
[**SetSenderAddress**](SystemMaintenanceApi.md#SetSenderAddress) | **Put** /api/latest/admin/mail-server/sender-address | Update server mail address
[**SetSettings2**](SystemMaintenanceApi.md#SetSettings2) | **Put** /api/latest/admin/rate-limit/settings | Set rate limit
[**StartExport**](SystemMaintenanceApi.md#StartExport) | **Post** /api/latest/migration/exports | Start export job
[**StartImport**](SystemMaintenanceApi.md#StartImport) | **Post** /api/latest/migration/imports | Start import job
[**StartMeshMigration**](SystemMaintenanceApi.md#StartMeshMigration) | **Post** /api/latest/migration/mesh | Start Mesh migration job
[**UpdateGlobalSettings**](SystemMaintenanceApi.md#UpdateGlobalSettings) | **Put** /admin | Update global SSH key settings
[**UpdateHookScript**](SystemMaintenanceApi.md#UpdateHookScript) | **Put** /api/latest/hook-scripts/{scriptId} | Update a hook script
[**UpdateLicense**](SystemMaintenanceApi.md#UpdateLicense) | **Post** /api/latest/admin/license | Update license
[**UpdateMeshNode**](SystemMaintenanceApi.md#UpdateMeshNode) | **Put** /api/latest/admin/git/mesh/nodes/{id} | Update Mesh node
[**UpdateSettings**](SystemMaintenanceApi.md#UpdateSettings) | **Post** /api/latest/users/{userSlug}/settings | Update user settings
[**UpdateUserDetails1**](SystemMaintenanceApi.md#UpdateUserDetails1) | **Put** /api/latest/users | Update user details
[**UpdateUserPassword1**](SystemMaintenanceApi.md#UpdateUserPassword1) | **Put** /api/latest/users/credentials | Set password
[**UploadAvatar1**](SystemMaintenanceApi.md#UploadAvatar1) | **Post** /api/latest/users/{userSlug}/avatar.png | Update user avatar

# **CancelExportJob**
> CancelExportJob(ctx, jobId)
Cancel export job

Requests the cancellation of an export job.  The request to cancel a job will be processed successfully if the job is actually still running. If it has already finished (successfully or with errors) or if it has already been canceled before, then an error will be returned.  There might be a small delay between accepting the request and actually cancelling the job. In most cases, the delay will be close to instantaneously. In the unlikely case of communication issues across a cluster, it can however take a few seconds to cancel a job.  A client should always actively query the job status to confirm that a job has been successfully canceled.  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| the ID of the job to cancel | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CancelImportJob**
> CancelImportJob(ctx, jobId)
Cancel import job

Requests the cancellation of an import job.  The request to cancel a job will be processed successfully if the job is actually still running. If it has already finished (successfully or with errors) or if it has already been canceled before, then an error will be returned.  Note that import jobs are not canceled as instantaneously as export jobs. Rather, once the request has been accepted, there are a number of checkpoints at which the job will actually apply it and stop. This is to keep the system in a reasonably consistent state:  - After the current fork hierarchy has been imported and verified. - Before the next repository is imported. - Before the next pull request is imported.  A client should always actively query the job status to confirm that a job has been successfully canceled.  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| the ID of the job to cancel | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CancelMeshMigrationJob**
> CancelMeshMigrationJob(ctx, jobId)
Cancel Mesh migration job

Requests the cancellation of a migration job.   The request to cancel a job will be processed successfully if the job is actually still running. If it has already finished (successfully or with errors) or if it has already been canceled before, then an error will be returned.   There might be a small delay between accepting the request and actually cancelling the job. In most cases, the delay will be close to instantaneously. In the unlikely case of communication issues across a cluster, it can however take a few seconds to cancel a job.  A client should always actively query the job status to confirm that a job has been successfully canceled.  The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| The ID of the job to cancel | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ClearDefaultBranch**
> ClearDefaultBranch(ctx, )
Clear default branch

Clears the global default branch, which is used when creating new repositories if an explicit default branch is not specified, if one has been configured.  The authenticated user must have <strong>ADMIN</strong> permission to call this resource.

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

# **ClearSenderAddress**
> ClearSenderAddress(ctx, )
Update mail configuration

Clears the server email address.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

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

# **Connectivity**
> RestMeshConnectivityReport Connectivity(ctx, )
Generate Mesh connectivity report

Generates a connectivity report between the Bitbucket node(s) and the Mesh node(s).  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestMeshConnectivityReport**](RestMeshConnectivityReport.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **CreateHookScript**
> RestHookScript CreateHookScript(ctx, optional)
Create a new hook script

Create a new hook script.  This endpoint requires **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiCreateHookScriptOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiCreateHookScriptOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content** | **optional.**|  | 
 **description** | **optional.**|  | 
 **name** | **optional.**|  | 
 **type_** | **optional.**|  | 

### Return type

[**RestHookScript**](RestHookScript.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete2**
> Delete2(ctx, id, optional)
Delete Mesh node

Delete a Mesh node  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **id** | **int64**|  | 
 **optional** | ***SystemMaintenanceApiDelete2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiDelete2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **force** | **optional.Bool**|  | [default to false]

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json;charset=UTF-8

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Delete6**
> Delete6(ctx, userSlug)
Delete user specific rate limit settings

Deletes the user-specific rate limit settings for the given user.  The authenticated user must have <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteAvatar**
> RestNamedLink DeleteAvatar(ctx, userSlug)
Delete user avatar

Delete the avatar associated to a user.   Users are always allowed to delete their own avatar. To delete someone else's avatar the authenticated user must have global <strong>ADMIN</strong> permission, or global <strong>SYS_ADMIN</strong> permission to update a <strong>SYS_ADMIN</strong> user's avatar.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug | 

### Return type

[**RestNamedLink**](RestNamedLink.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteBanner**
> DeleteBanner(ctx, )
Delete announcement banner

Deletes a banner, if one is present in the database.

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

# **DeleteHookScript**
> DeleteHookScript(ctx, scriptId)
Delete a hook script.

Deletes a registered hook script.  This endpoint requires **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **scriptId** | **string**| The ID of the hook script to delete | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteMailConfig**
> DeleteMailConfig(ctx, )
Delete mail configuration

Deletes the current mail configuration.  The authenticated user must have the <strong>SYS_ADMIN</strong> permission to call this resource.

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

# **DismissRetentionConfigReviewNotification**
> DismissRetentionConfigReviewNotification(ctx, )
Dismiss retention config notification

Dismisses the retention config review notification displayed by the audit plugin for the user that's currently logged in.

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

# **Get2**
> RestBitbucketLicense Get2(ctx, )
Get license details

Retrieves details about the current license, as well as the current status of the system with regards to the installed license. The status includes the current number of users applied toward the license limit, as well as any status messages about the license (warnings about expiry or user counts exceeding license limits).   The authenticated user must have <b>ADMIN</b> permission. Unauthenticated users, and non-administrators, are not permitted to access license details.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestBitbucketLicense**](RestBitbucketLicense.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Get4**
> RestUserRateLimitSettings Get4(ctx, userSlug)
Get user specific rate limit settings

Retrieves the user-specific rate limit settings for the given user.  To call this resource, the user must be authenticated and either have <strong>ADMIN</strong> permission or be the same user as the one whose settings are requested. A user with <strong>ADMIN</strong> permission cannot get the settings of a user with <strong>SYS_ADMIN</strong> permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug. | 

### Return type

[**RestUserRateLimitSettings**](RestUserRateLimitSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetActiveMeshMigrationSummary**
> RestMeshMigrationSummary GetActiveMeshMigrationSummary(ctx, )
Get summary for Mesh migration job

Gets the summary, including the queue status and progress, of the currently active Mesh migration job.  The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestMeshMigrationSummary**](RestMeshMigrationSummary.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllMeshMigrationSummaries**
> InlineResponse20028 GetAllMeshMigrationSummaries(ctx, optional)
Get all Mesh migration job summaries

Retrieve a page of Mesh migration job summaries. Jobs are ordered by when they were started, newest first.   The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiGetAllMeshMigrationSummariesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetAllMeshMigrationSummariesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20028**](inline_response_200_28.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllRateLimitSettings**
> InlineResponse20020 GetAllRateLimitSettings(ctx, optional)
Get rate limit settings for user

Retrieves the user-specific rate limit settings for the given user.  The authenticated user must have <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiGetAllRateLimitSettingsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetAllRateLimitSettingsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**| Optional filter | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20020**](inline_response_200_20.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetAllRegisteredMeshNodes**
> RestMeshNode GetAllRegisteredMeshNodes(ctx, )
Get all registered Mesh nodes

Get all the registered Mesh nodes.  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestMeshNode**](RestMeshNode.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetApplicationProperties**
> RestApplicationProperties GetApplicationProperties(ctx, )
Get application properties

Retrieve version information and other application properties.  No authentication is required to call this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestApplicationProperties**](RestApplicationProperties.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetBanner**
> RestAnnouncementBanner GetBanner(ctx, )
Get announcement banner

Gets the announcement banner, if one exists and is available to the user

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestAnnouncementBanner**](RestAnnouncementBanner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetControlPlanePublicKey**
> GetControlPlanePublicKey(ctx, )
Get the control plane PEM

Obtain the control plane PEM.  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters
This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetDefaultBranch**
> GetDefaultBranch(ctx, )
Get the default branch

Retrieves the configured global default branch, which is used when creating new repositories if an explicit default branch is not specified.  The user must be authenticated to call this resource.

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

# **GetExportJob**
> RestJob GetExportJob(ctx, jobId)
Get export job details

Gets the details, including the current status and progress, of the export job identified by the given ID.  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| the ID of the job | 

### Return type

[**RestJob**](RestJob.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetExportJobMessages**
> InlineResponse20026 GetExportJobMessages(ctx, jobId, optional)
Get job messages

Gets the messages generated by the job.  Without any filter, all messages will be returned, but the response can optionally be filtered for the following severities. The severity parameter can be repeated to include multiple severities in one response.  - INFO - WARN - ERROR  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| The ID of the job | 
 **optional** | ***SystemMaintenanceApiGetExportJobMessagesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetExportJobMessagesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **severity** | **optional.String**| The severity to include in the results | 
 **subject** | **optional.String**| The subject | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20026**](inline_response_200_26.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetGlobalSettings**
> RestSshKeySettings GetGlobalSettings(ctx, )
Get global SSH key settings

Gets the global settings that enforce the maximum expiry of SSH keys and restrictions on SSH key types.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestSshKeySettings**](RestSshKeySettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetHistory**
> InlineResponse20019 GetHistory(ctx, optional)
Get rate limit history

Retrieves the recent rate limit history for the instance.  The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiGetHistoryOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetHistoryOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order** | **optional.String**| An optional sort category to arrange the results in descending order | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20019**](inline_response_200_19.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetHookScript**
> RestHookScript GetHookScript(ctx, scriptId)
Get a hook script

Retrieves a hook script by ID.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **scriptId** | **string**| The ID of the hook script to retrieve | 

### Return type

[**RestHookScript**](RestHookScript.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetImportJob**
> RestJob GetImportJob(ctx, jobId)
Get import job status

Gets the details, including the current status and progress, of the import job identified by the given ID.  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| The ID of the job | 

### Return type

[**RestJob**](RestJob.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetImportJobMessages**
> InlineResponse20026 GetImportJobMessages(ctx, jobId, optional)
Get import job messages

Gets the messages generated by the job.  Without any filter, all messages will be returned, but the response can optionally be filtered for the following severities. The severity parameter can be repeated to include multiple severities in one response.  - INFO - WARN - ERROR  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| The ID of the job | 
 **optional** | ***SystemMaintenanceApiGetImportJobMessagesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetImportJobMessagesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **severity** | **optional.String**| The severity to include in the results | 
 **subject** | **optional.String**| The subject | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20026**](inline_response_200_26.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetInformation**
> RestClusterInformation GetInformation(ctx, )
Get cluster node information

Gets information about the nodes that currently make up the stash cluster.  The authenticated user must have the <strong>SYS_ADMIN</strong> permission to call this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestClusterInformation**](RestClusterInformation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetLabel**
> RestLabel GetLabel(ctx, labelName)
Get label

Returns a label.  The user needs to be authenticated to use this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **labelName** | **string**| the label name | 

### Return type

[**RestLabel**](RestLabel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetLabelables**
> InlineResponse20025 GetLabelables(ctx, labelName, optional)
Get labelables for label

Returns a page of labelables for a given label.  Only labelables that the authenticated user has view access to will be returned.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **labelName** | **string**| The page of labelables. | 
 **optional** | ***SystemMaintenanceApiGetLabelablesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetLabelablesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **type_** | **optional.String**|  the type of labelables to be returned. Supported values: REPOSITORY | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20025**](inline_response_200_25.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetLabels**
> InlineResponse20024 GetLabels(ctx, optional)
Get all labels

Returns a paged response of all the labels in the system.  The user needs to be authenticated to use this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiGetLabelsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetLabelsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **prefix** | **optional.String**| (optional) prefix to filter the labels on. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20024**](inline_response_200_24.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetLevel**
> RestLogLevel GetLevel(ctx, loggerName)
Get current log level

Retrieve the current log level for a given logger.  The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **loggerName** | **string**| The name of the logger. | 

### Return type

[**RestLogLevel**](RestLogLevel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetMailConfig**
> RestMailConfiguration GetMailConfig(ctx, )
Get mail configuration

Retrieves the current mail configuration.   The authenticated user must have the <strong>SYS_ADMIN</strong> permission to call this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestMailConfiguration**](RestMailConfiguration.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetMeshMigrationJob**
> GetMeshMigrationJob(ctx, jobId)
Get Mesh migration job details

Gets the details, including the current status and progress, of the job identified by the given ID.  The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| The ID of the job | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetMeshMigrationJobMessages**
> InlineResponse20026 GetMeshMigrationJobMessages(ctx, jobId, optional)
Get Mesh migration job messages

Gets the messages generated by the job.   Without any filter, all messages will be returned, but the response can optionally be filtered for the following severities. The severity parameter can be repeated to include multiple severities in one response.        - INFO      - WARN      - ERROR   The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| The ID of the job | 
 **optional** | ***SystemMaintenanceApiGetMeshMigrationJobMessagesOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetMeshMigrationJobMessagesOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **severity** | **optional.String**| The severity to include in the results | 
 **subject** | **optional.String**| The subject | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20026**](inline_response_200_26.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetMeshMigrationJobSummary**
> RestMeshMigrationSummary GetMeshMigrationJobSummary(ctx, jobId)
Get Mesh migration job summary

Gets the summary, including the queue status and progress, of a Mesh migration job.   The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **jobId** | **string**| The ID of the job | 

### Return type

[**RestMeshMigrationSummary**](RestMeshMigrationSummary.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRegisteredMeshNodeById**
> RestMeshNode GetRegisteredMeshNodeById(ctx, id)
Get Mesh node

Get the registered Mesh node that matches the supplied ID.  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **id** | **string**| The ID of the Mesh node. | 

### Return type

[**RestMeshNode**](RestMeshNode.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositoryArchivePolicy**
> RestRepositoryPolicy GetRepositoryArchivePolicy(ctx, )
Get repository archive policy

Retrieves the repository archive policy for the instance.  The user must be authenticated to access this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestRepositoryPolicy**](RestRepositoryPolicy.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRepositoryDeletePolicy**
> RestRepositoryPolicy GetRepositoryDeletePolicy(ctx, )
Get repository delete policy

Retrieves the repository delete policy for the instance.  The user must be authenticated to access this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestRepositoryPolicy**](RestRepositoryPolicy.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetRootLevel**
> RestLogLevel GetRootLevel(ctx, )
Get root log level

 Retrieve the current log level for the root logger.  The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestLogLevel**](RestLogLevel.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSenderAddress**
> GetSenderAddress(ctx, )
Get server mail address

Retrieves the server email address

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

# **GetSettings2**
> RestRateLimitSettings GetSettings2(ctx, )
Get rate limit settings

Retrieves the rate limit settings for the instance.  The user must be authenticated to call this resource.

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**RestRateLimitSettings**](RestRateLimitSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSupportZip**
> GetSupportZip(ctx, id)
Get support zip for node

Get the support zip for the Mesh node that matches the specified ID.  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **id** | **string**| The ID of the Mesh node. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSupportZips**
> GetSupportZips(ctx, )
Get support zips for all Mesh nodes

Get the support zips for all the Mesh nodes.  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters
This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSupportedKeyTypes**
> GetSupportedKeyTypes(ctx, )
Get supported SSH key algorithms and lengths

Retrieves a list of all supported SSH key algorithms and lengths.

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

# **GetUser**
> RestApplicationUser GetUser(ctx, userSlug)
Get user

Retrieve the user matching the supplied <strong>userSlug</strong>.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug | 

### Return type

[**RestApplicationUser**](RestApplicationUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUserSettings**
> ExampleSettingsMap GetUserSettings(ctx, userSlug)
Get user settings

Retrieve a map of user setting key values for a specific user identified by the user slug.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug. | 

### Return type

[**ExampleSettingsMap**](ExampleSettingsMap.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetUsers2**
> RestApplicationUser GetUsers2(ctx, optional)
Get all users

Retrieve a page of users, optionally run through provided filters.   Only authenticated users may call this resource. ### Permission Filters   The following three sub-sections list parameters supported for permission filters (where <code>[root]</code> is the root permission filter name, e.g. <code>permission</code>, <code>permission.1</code> etc.) depending on the permission resource. The system determines which filter to apply (Global, Project or Repository permission) based on the `[root]` permission value. E.g. <code>ADMIN</code> is a global permission, <code>PROJECT_ADMIN</code> is a project permission and <code>REPO_ADMIN</code> is a repository permission. Note that the parameters for a given resource will be looked up in the order as they are listed below, that is e.g. for a project resource, if both <code>projectId</code> and <code>projectKey</code> are provided, the system will use <code>projectId</code> for the lookup. <h4>Global permissions</h4>   The permission value under <code>[root]</code> is the only required and recognized parameter, as global permissions do not apply to a specific resource.   Example valid filter: <code>permission=ADMIN</code>. <h4>Project permissions</h4>   - <code>[root]</code>- specifies the project permission - <code>[root].projectId</code> - specifies the project ID to lookup the project by - <code>[root].projectKey</code> - specifies the project key to lookup the project by   Example valid filter: <code>permission.1=PROJECT_ADMIN&amp;permission.1.projectKey=TEST_PROJECT</code>. #### Repository permissions   - <code>[root]</code>- specifies the repository permission - <code>[root].projectId</code> - specifies the repository ID to lookup the repository by - <code>[root].projectKey</code> and <code>[root].repositorySlug</code>- specifies the project key and     repository slug to lookup the repository by; both values <i>need to</i> be provided for this look up to be     triggered   Example valid filter: <code>permission.2=REPO_ADMIN&amp;permission.2.projectKey=TEST_PROJECT&amp;permission.2.repositorySlug=test_repo</code>.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiGetUsers2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiGetUsers2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **optional.String**| Return only users, whose username, name or email address &lt;i&gt;contain&lt;/i&gt; the &lt;code&gt; filter&lt;/code&gt; value | 
 **permissionN** | **optional.String**| The \&quot;root\&quot; of a single permission filter, similar to the &lt;code&gt;permission&lt;/code&gt; parameter, where \&quot;N\&quot; is a natural number starting from 1. This allows clients to specify multiple permission filters, by providing consecutive filters as &lt;code&gt;permission.1&lt;/code&gt;, &lt;code&gt;permission.2&lt;/code&gt; etc. Note that the filters numbering has to start with 1 and be continuous for all filters to be processed. The total allowed number of permission filters is 50 and all filters exceeding that limit will be dropped. See the section \&quot;Permission Filters\&quot; above for more details on how the permission filters are processed. | 
 **permission** | **optional.String**| The \&quot;root\&quot; of a permission filter, whose value must be a valid global, project, or repository permission. Additional filter parameters referring to this filter that specify the resource (project or repository) to apply the filter to must be prefixed with &lt;code&gt;permission.&lt;/code&gt;. See the section \&quot;Permission Filters\&quot; above for more details. | 
 **group** | **optional.String**| return only users who are members of the given group | 

### Return type

[**RestApplicationUser**](RestApplicationUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PreviewExport**
> RestScopesExample PreviewExport(ctx, optional)
Preview export

Enumerates the projects and repositories that would be exported for a given export request.  All affected repositories will be enumerated explicitly, and while projects are listed as individual items in responses from this endpoint, their presence does not imply that all their repositories are included.  While this endpoint can be used to verify that all selectors in the request apply as intended, it should be noted that a subsequent, actual export might contain a different set of repositories, as they might have been added or deleted in the meantime.  Note that the overall response from this endpoint can become very large when a lot of repositories end up in the selection. This is why the server is streaming the response while it is being generated (as opposed to creating it in memory and then sending it all at once) and it can be consumed in a streaming way, too.  Also, due to the potential size of the response, projects and repositories are listed with fewer details than in other REST responses.  For a more detailed description of selectors, see the endpoint documentation for starting an export.  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiPreviewExportOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiPreviewExportOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestExportRequest**](RestExportRequest.md)| the export request | 

### Return type

[**RestScopesExample**](RestScopesExample.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **PreviewMeshMigration**
> ExamplePreviewMigration PreviewMeshMigration(ctx, optional)
Preview Mesh migration

Enumerates the projects and repositories that would be migrated for a given request.  All affected repositories will be enumerated explicitly, and while projects are listed as individual items in responses from this endpoint, their presence does not imply that all their repositories are included.  While this endpoint can be used to verify that all selectors in the request apply as intended, it should be noted that a subsequent, actual export might contain a different set of repositories, as they might have been added or deleted in the meantime.  Note that the overall response from this endpoint can become very large when a lot of repositories end up in the selection. This is why the server is streaming the response while it is being generated (as opposed to creating it in memory and then sending it all at once) and it can be consumed in a streaming way, too.  Also, due to the potential size of the response, projects and repositories are listed with fewer details than in other REST responses.  The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiPreviewMeshMigrationOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiPreviewMeshMigrationOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestMeshMigrationRequest**](RestMeshMigrationRequest.md)| The export request | 

### Return type

[**ExamplePreviewMigration**](ExamplePreviewMigration.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Read**
> Read(ctx, scriptId)
Get hook script content

Retrieves the hook script content.  This endpoint requires **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **scriptId** | **string**| The ID of the hook script | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **RegisterNewMeshNode**
> RestMeshNode RegisterNewMeshNode(ctx, optional)
Register new Mesh node

Register a new Mesh node.  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiRegisterNewMeshNodeOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiRegisterNewMeshNodeOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestMeshNode**](RestMeshNode.md)| The request specifying the new Mesh node. | 

### Return type

[**RestMeshNode**](RestMeshNode.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SearchMeshMigrationRepos**
> InlineResponse20027 SearchMeshMigrationRepos(ctx, optional)
Find repositories by Mesh migration state

Searches for repositories in the system matching the specified criteria and enriches their MeshMigrationQueueState migration state if a migration is currently in progress.   The currently active migration can optionally be specified by passing a migrationId, if known. If this isn't passed, an attempt is made to locate the active migration and its ID is used.   If a migration is currently active, only repositories that are a part of the migration are filtered and returned. Otherwise, all repositories in the systems are filtered and returned.   Filtering by state is ignored when no migration is currently in progress. In such a case, results are not enriched with their MeshMigrationQueueState migration state.   The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSearchMeshMigrationReposOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSearchMeshMigrationReposOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **migrationId** | **optional.String**| (optional) The currently active migration job. If not passed, this is looked up internally. | 
 **projectKey** | **optional.String**| (optional) The project key. Can be specified more than once to filter by more than one project. | 
 **name** | **optional.String**| (optional) The repository name | 
 **state** | **optional.String**| (optional) If a migration is active, the MeshMigrationQueueState state to filter results by. Can be specified more than once to filter by more than one state. | 
 **remote** | **optional.String**| (optional) Whether the repository has been fully migrated to Mesh. If not present, all repositories are considered regardless of where they&#x27;re located. | 
 **start** | **optional.Float64**| Start number for the page (inclusive). If not passed, first page is assumed. | 
 **limit** | **optional.Float64**| Number of items to return. If not passed, a page size of 25 is used. | 

### Return type

[**InlineResponse20027**](inline_response_200_27.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Set**
> RestUserRateLimitSettings Set(ctx, optional)
Set rate limit settings for users

Sets the given rate limit settings for the given users.  The authenticated user must have <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestBulkUserRateLimitSettingsUpdateRequest**](RestBulkUserRateLimitSettingsUpdateRequest.md)|  | 

### Return type

[**RestUserRateLimitSettings**](RestUserRateLimitSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **Set1**
> RestUserRateLimitSettings Set1(ctx, userSlug, optional)
Set rate limit settings for user

Sets the given rate limit settings for the given user.  The authenticated user must have <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug. | 
 **optional** | ***SystemMaintenanceApiSet1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSet1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestUserRateLimitSettingsUpdateRequest**](RestUserRateLimitSettingsUpdateRequest.md)|  | 

### Return type

[**RestUserRateLimitSettings**](RestUserRateLimitSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetBanner**
> SetBanner(ctx, optional)
Update/Set announcement banner

Sets the announcement banner with the provided JSON. Only users authenticated as Admins may call this resource

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetBannerOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetBannerOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of AdminBannerBody**](AdminBannerBody.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetDefaultBranch**
> SetDefaultBranch(ctx, optional)
Update/Set default branch

Configures the global default branch, which is used when creating new repositories if an explicit default branch is not specified.  The authenticated user must have <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetDefaultBranchOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetDefaultBranchOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of AdminDefaultbranchBody**](AdminDefaultbranchBody.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetLevel**
> SetLevel(ctx, levelName, loggerName)
Set log level

Set the current log level for a given logger.  The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **levelName** | **string**| The level to set the logger to. Either TRACE, DEBUG, INFO, WARN or ERROR | 
  **loggerName** | **string**| The name of the logger. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetMailConfig**
> RestMailConfiguration SetMailConfig(ctx, optional)
Update mail configuration

Updates the mail configuration.   The authenticated user must have the <strong>SYS_ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetMailConfigOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetMailConfigOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of AdminMailserverBody**](AdminMailserverBody.md)|  | 

### Return type

[**RestMailConfiguration**](RestMailConfiguration.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetRepositoryArchivePolicy**
> RestRepositoryPolicy SetRepositoryArchivePolicy(ctx, optional)
Update repository archive policy

Sets the repository archive policy for the instance.  The authenticated user must have <b>SYS_ADMIN</b> permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetRepositoryArchivePolicyOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetRepositoryArchivePolicyOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestRepositoryPolicy**](RestRepositoryPolicy.md)| The request containing the details of the policy. | 

### Return type

[**RestRepositoryPolicy**](RestRepositoryPolicy.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetRepositoryDeletePolicy**
> RestRepositoryPolicy SetRepositoryDeletePolicy(ctx, optional)
Update the repository delete policy

Sets the repository delete policy for the instance.  The authenticated user must have <b>SYS_ADMIN</b> permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetRepositoryDeletePolicyOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetRepositoryDeletePolicyOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestRepositoryPolicy**](RestRepositoryPolicy.md)| The request containing the details of the policy. | 

### Return type

[**RestRepositoryPolicy**](RestRepositoryPolicy.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetRootLevel**
> SetRootLevel(ctx, levelName)
Set root log level

Set the current log level for the root logger.  The authenticated user must have <strong>ADMIN</strong> permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **levelName** | **string**| the level to set the logger to. Either TRACE, DEBUG, INFO, WARN or ERROR | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetSenderAddress**
> SetSenderAddress(ctx, optional)
Update server mail address

Updates the server email address   The authenticated user must have the <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetSenderAddressOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetSenderAddressOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of string**](string.md)|  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SetSettings2**
> RestRateLimitSettings SetSettings2(ctx, optional)
Set rate limit

Sets the rate limit settings for the instance.  The authenticated user must have <strong>ADMIN</strong> permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiSetSettings2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiSetSettings2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestRateLimitSettings**](RestRateLimitSettings.md)| Sets the rate limit settings for the instance.

The authenticated user must have &lt;strong&gt;ADMIN&lt;/strong&gt; permission to call this resource. | 

### Return type

[**RestRateLimitSettings**](RestRateLimitSettings.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StartExport**
> RestJob StartExport(ctx, optional)
Start export job

Starts a background job that exports the selected repositories.  Only 2 concurrent exports are supported _per cluster node_. If a request ends up on a node that is already running that many export jobs, the request will be rejected and an error returned.  The response includes a description of the job that has been started, and its ID can be used to query these details again, including the current progress, warnings and errors that occurred while processing the job, and to interrupt and cancel the execution of this job.  The request to start an export is similar to the one for previewing an export. Additionally, it accepts an optional parameter, `exportLocation`, which can be used to specify a _relative_ path within `data/migration/export` in the shared home directory. No locations outside of that directory will be accepted for exports.  There are essentially three ways to select repositories for export. Regardless of which you use, a few general rules apply:  - You can supply a list of selectors. The selection will be additive. - Repositories that are selected more than once due to overlapping selectors will be de-duplicated and effectively exported only once. - For every selected repository, its full fork hierarchy will be considered selected, even if parts of that hierarchy would otherwise not be matched by the provided selectors. For example, when you explicitly select a single repository only, but that repository is a fork, then its origin will be exported (and eventually imported), too.  Now, a single repository can be selected like this:  ```    {       \"projectKey\": \"PRJ\",       \"slug\": \"my-repo\" }  ```  Second, all repositories in a specific project can be selected like this:  ```    {       \"projectKey\": \"PRJ\",       \"slug\": *\" }  ```  And third, all projects and repositories in the system would be selected like this:  ```    {       \"projectKey\": \"*\",       \"slug\": *\" }  ```  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiStartExportOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiStartExportOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestExportRequest**](RestExportRequest.md)| The request | 

### Return type

[**RestJob**](RestJob.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StartImport**
> RestJob StartImport(ctx, optional)
Start import job

Starts a background job that imports the specified archive.  Only 1 import at a time is supported _per cluster_. If another request is made while an import is already running, the request will be rejected and an error returned.  The path in the request must point to a valid archive file. The file must be located within the `data/migration/import` directory in the shared home directory.  The authenticated user must have **ADMIN** permission or higher to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiStartImportOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiStartImportOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestImportRequest**](RestImportRequest.md)| The request | 

### Return type

[**RestJob**](RestJob.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **StartMeshMigration**
> RestJob StartMeshMigration(ctx, optional)
Start Mesh migration job

Starts a background job that migrates selected projects/repositories to Mesh.   Only 1 job is supported _per cluster_.  The response includes a description of the job that has been started, and its ID can be used to query these details again, including the current progress, and to interrupt and cancel the execution of this job.   The request to start a migration is similar to the one for previewing a migration.   There are essentially three ways to select repositories for migration. Regardless of which you use, a few general rules apply:       - You can supply a list of repository IDs and project IDs. The selection will be additive. All repositories     in the system are migrated if both lists are empty.     - Repositories that are selected more than once due to overlapping IDs will be de-duplicated and     effectively migrated only once.     - For every selected repository, its full fork hierarchy will be considered selected, even if parts of that     hierarchy would otherwise not be matched by the provided IDs. For example, when you explicitly     select a single repository only, but that repository is a fork, then its origin will be migrated too.   Now, a single repository can be selected like this:   ```       {      \"repositoryIds\": [1]      } ```  Multiple repositories can be selected like this:    ```       {      \"repositoryIds\": [1, 2]      } ```  Second, all repositories in a specific project can be selected like this:    ```       {      \"projectIds\": [1]      } ```  And third, all projects and repositories in the system would be selected like this:    ```       {      \"projectIds\": [],      \"repositoryIds\": []      } ```  The authenticated user must have **SYS_ADMIN** permission to call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiStartMeshMigrationOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiStartMeshMigrationOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of MigrationMeshBody**](MigrationMeshBody.md)|  | 

### Return type

[**RestJob**](RestJob.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateGlobalSettings**
> UpdateGlobalSettings(ctx, optional)
Update global SSH key settings

Updates the global settings that enforces the maximum expiry of SSH keys and restrictions on SSH key types.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiUpdateGlobalSettingsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUpdateGlobalSettingsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestSshKeySettings**](RestSshKeySettings.md)| A request containing expiry length to be set for SSH keys and a list of SSH key type restrictions. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateHookScript**
> RestHookScript UpdateHookScript(ctx, scriptId, optional)
Update a hook script

Updates a hook script.  This endpoint requires **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **scriptId** | **string**| The ID of the hook script | 
 **optional** | ***SystemMaintenanceApiUpdateHookScriptOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUpdateHookScriptOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of ExamplePutMultipartFormData**](ExamplePutMultipartFormData.md)| The multipart form data containing the hook script | 

### Return type

[**RestHookScript**](RestHookScript.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateLicense**
> RestBitbucketLicense UpdateLicense(ctx, optional)
Update license

Decodes the provided encoded license and sets it as the active license. If no license was provided, a 400 is returned. If the license cannot be decoded, or cannot be applied, a 409 is returned. Some possible reasons a license may not be applied include:   - It is for a different product - It is already expired   Otherwise, if the license is updated successfully, details for the new license are returned with a 200 response.  <b>Warning</b>: It is possible to downgrade the license during update, applying a license with a lower number of permitted users. If the number of currently-licensed users exceeds the limits of the new license, pushing will be disabled until the licensed user count is brought into compliance with the new license.  The authenticated user must have <b>SYS_ADMIN</b> permission. <b>ADMIN</b> users may <i>view</i> the current license details, but they may not <i>update</i> the license.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiUpdateLicenseOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUpdateLicenseOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of RestBitbucketLicense**](RestBitbucketLicense.md)| a JSON payload containing the encoded license to apply | 

### Return type

[**RestBitbucketLicense**](RestBitbucketLicense.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateMeshNode**
> RestMeshNode UpdateMeshNode(ctx, id, optional)
Update Mesh node

Update a Mesh node.  The authenticated user must have **SYS_ADMIN** permission.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **id** | **string**| The ID of the Mesh node to update. | 
 **optional** | ***SystemMaintenanceApiUpdateMeshNodeOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUpdateMeshNodeOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of RestMeshNode**](RestMeshNode.md)| The request specifying the updated Mesh node. | 

### Return type

[**RestMeshNode**](RestMeshNode.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateSettings**
> UpdateSettings(ctx, userSlug, optional)
Update user settings

Update the entries of a map of user setting key/values for a specific user identified by the user slug.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug. | 
 **optional** | ***SystemMaintenanceApiUpdateSettingsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUpdateSettingsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of ExampleSettingsMap**](ExampleSettingsMap.md)| A map with the UserSettings entries which must be updated. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateUserDetails1**
> RestApplicationUser UpdateUserDetails1(ctx, optional)
Update user details

Update the currently authenticated user's details. The update will always be applied to the currently authenticated user.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiUpdateUserDetails1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUpdateUserDetails1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of UserUpdate**](UserUpdate.md)| The user update details | 

### Return type

[**RestApplicationUser**](RestApplicationUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateUserPassword1**
> UpdateUserPassword1(ctx, optional)
Set password

Update the currently authenticated user's password.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SystemMaintenanceApiUpdateUserPassword1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUpdateUserPassword1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of UserPasswordUpdate**](UserPasswordUpdate.md)| The password update details | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UploadAvatar1**
> UploadAvatar1(ctx, userSlug, optional)
Update user avatar

Update the avatar for the user with the supplied <strong>slug</strong>.   This resource accepts POST multipart form data, containing a single image in a form-field named 'avatar'.   There are configurable server limits on both the dimensions (1024x1024 pixels by default) and uploaded file size (1MB by default). Several different image formats are supported, but <strong>PNG</strong> and <strong>JPEG</strong> are preferred due to the file size limit.   This resource has Cross-Site Request Forgery (XSRF) protection. To allow the request to pass the XSRF check the caller needs to send an <code>X-Atlassian-Token</code> HTTP header with the value <code>no-check</code>.   An example <a href=\"http://curl.haxx.se/\">curl</a> request to upload an image name 'avatar.png' would be: ``` curl -X POST -u username:password -H \"X-Atlassian-Token: no-check\" http://example.com/rest/api/latest/users/jdoe/avatar.png -F avatar=@avatar.png ```   Users are always allowed to update their own avatar. To update someone else's avatar the authenticated user must have global <strong>ADMIN</strong> permission, or global <strong>SYS_ADMIN</strong> permission to update a <strong>SYS_ADMIN</strong> user's avatar.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **userSlug** | **string**| The user slug | 
 **optional** | ***SystemMaintenanceApiUploadAvatar1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SystemMaintenanceApiUploadAvatar1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **avatar** | **optional.Interface of *os.File****optional.**|  | 
 **xAtlassianToken** | **optional.**| This resource has Cross-Site Request Forgery (XSRF) protection. To allow the request to pass the XSRF check the caller needs to send an &lt;code&gt;X-Atlassian-Token&lt;/code&gt; HTTP header with the value &lt;code&gt;no-check&lt;/code&gt;. | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

