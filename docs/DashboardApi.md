# {{classname}}

All URIs are relative to *http://{baseurl}/rest*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetPullRequestSuggestions**](DashboardApi.md#GetPullRequestSuggestions) | **Get** /api/latest/dashboard/pull-request-suggestions | Get pull request suggestions
[**GetPullRequests1**](DashboardApi.md#GetPullRequests1) | **Get** /api/latest/dashboard/pull-requests | Get pull requests for a user

# **GetPullRequestSuggestions**
> InlineResponse20021 GetPullRequestSuggestions(ctx, optional)
Get pull request suggestions

Retrieves a page of suggestions for pull requests that the currently authenticated user may wish to raise. Such suggestions are based on ref changes occurring and so contain the ref change that prompted the suggestion plus the time the change event occurred. Changes will be returned in descending order based on the time the change that prompted the suggestion occurred.   Note that although the response is a page object, the interface does not support paging, however a limit can be applied to the size of the returned page.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***DashboardApiGetPullRequestSuggestionsOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DashboardApiGetPullRequestSuggestionsOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **changesSince** | **optional.String**| restrict pull request suggestions to be based on events that occurred since some timein the past. This is expressed in seconds since \&quot;now\&quot;. So to return suggestionsbased only on activity within the past 48 hours, pass a value of 172800. | 
 **limit** | **optional.String**| restricts the result set to return at most this many suggestions. | 

### Return type

[**InlineResponse20021**](inline_response_200_21.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetPullRequests1**
> InlineResponse20022 GetPullRequests1(ctx, optional)
Get pull requests for a user

Retrieve a page of pull requests where a user is involved as either a reviewer, author or a participant. The request may be filtered by pull request state, role or participant status.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***DashboardApiGetPullRequests1Opts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a DashboardApiGetPullRequests1Opts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **closedSince** | **optional.String**| (optional, defaults to returning pull requests regardless of closed since date). Permits returning only pull requests with a closed timestamp set more recently that (now - closedSince). Units are in seconds. So for example if closed since 86400 is set only pull requests closed in the previous 24 hours will be returned. | 
 **role** | **optional.String**| (optional, defaults to returning pull requests for any role). If a role is supplied only pull requests where the authenticated user is a participant in the given role will be returned. Either &lt;strong&gt;REVIEWER&lt;/strong&gt;, &lt;strong&gt;AUTHOR&lt;/strong&gt; or &lt;strong&gt;PARTICIPANT&lt;/strong&gt;. | 
 **participantStatus** | **optional.String**| (optional, defaults to returning pull requests with any participant status). A comma separated list of participant status. That is, one or more of &lt;strong&gt;UNAPPROVED&lt;/strong&gt;, &lt;strong&gt;NEEDS_WORK&lt;/strong&gt;, or &lt;strong&gt;APPROVED&lt;/strong&gt;. | 
 **state** | **optional.String**| (optional, defaults to returning pull requests in any state). If a state is supplied only pull requests in the specified state will be returned. Either &lt;strong&gt;OPEN&lt;/strong&gt;, &lt;strong&gt;DECLINED&lt;/strong&gt; or &lt;strong&gt;MERGED&lt;/strong&gt;. Omit this parameter to return pull request in any state. | 
 **user** | **optional.String**| The name of the involved user, defaults to the current user. | 
 **order** | **optional.String**| (optional, defaults to &lt;strong&gt;NEWEST&lt;/strong&gt;) the order to return pull requests in, either &lt;strong&gt;OLDEST&lt;/strong&gt; (as in: \&quot;oldest first\&quot;), &lt;strong&gt;NEWEST&lt;/strong&gt;, &lt;strong&gt;PARTICIPANT_STATUS&lt;/strong&gt;, or &lt;strong&gt;CLOSED_DATE&lt;/strong&gt;. Where &lt;strong&gt;CLOSED_DATE&lt;/strong&gt; is specified and the result set includes pull requests that are not in the closed state, these pull requests will appear first in the result set, followed by most recently closed pull requests. | 
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

