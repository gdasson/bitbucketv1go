# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Preview**](MarkupApi.md#Preview) | **Post** /api/latest/markup/preview | Preview markdown render

# **Preview**
> RestMarkup Preview(ctx, optional)
Preview markdown render

Preview generated HTML for the given markdown content.  Only authenticated users may call this resource.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***MarkupApiPreviewOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a MarkupApiPreviewOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of string**](string.md)|  | 
 **htmlEscape** | **optional.**| (Optional) true if HTML should be escaped in the input markup, false otherwise. | 
 **urlMode** | **optional.**| (Optional) The mode to use when building URLs. One of: ABSOLUTE, RELATIVE or, CONFIGURED. By default this is RELATIVE. | 
 **includeHeadingId** | **optional.**| (Optional) true if headers should contain an ID based on the heading content. | 
 **hardwrap** | **optional.**| (Optional) Whether the markup implementation should convert newlines to breaks. By default this is false which reflects the standard markdown specification. | 

### Return type

[**RestMarkup**](RestMarkup.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

