# ExampleMultipartFormData

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Branch** | **string** | The branch on which the &lt;code&gt;path&lt;/code&gt; should be modified or created. | [optional] [default to null]
**Content** | **string** | The full content of the file at &lt;code&gt;path&lt;/code&gt;. | [optional] [default to null]
**Message** | **string** | The message associated with this change, to be used as the commit message. Or null if the default message should be used. | [optional] [default to null]
**SourceBranch** | **string** | The starting point for &lt;code&gt;branch&lt;/code&gt;. If provided and different from &lt;code&gt;branch&lt;/code&gt;, &lt;code&gt;branch&lt;/code&gt; will be created as a new branch, branching off from &lt;code&gt;sourceBranch&lt;/code&gt;. | [optional] [default to null]
**SourceCommitId** | **string** | The commit ID of the file before it was edited, used to identify if content has changed. Or null if this is a new file | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

