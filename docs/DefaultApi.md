# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetPullRequestCount**](DefaultApi.md#GetPullRequestCount) | **Get** /api/latest/inbox/pull-requests/count | Get total number of pull requests in inbox
[**GetPullRequests2**](DefaultApi.md#GetPullRequests2) | **Get** /api/latest/inbox/pull-requests | Get pull requests in inbox

# **GetPullRequestCount**
> GetPullRequestCount(ctx, )
Get total number of pull requests in inbox

Returns the total number of pull requests in the user's inbox

### Required Parameters
This endpoint does not need any parameter.

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json;charset=UTF-8

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPullRequests2**
> GetPullRequests2(ctx, optional)
Get pull requests in inbox

Returns a page of pull requests in the user's inbox.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***DefaultApiGetPullRequests2Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DefaultApiGetPullRequests2Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **role** | **optional.String**|  | [default to reviewer]
 **limit** | **optional.Int32**|  | [default to 25]
 **start** | **optional.Int32**|  | [default to 0]

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json;charset=UTF-8

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

