# RestSecretScanningRule

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Human readable name for the rule | [optional] [default to null]
**Id** | **int64** | The ID of the rule | [optional] [default to null]
**LineRegex** | **string** | If present, regular expression for matching a secret on a code line | [optional] [default to null]
**PathRegex** | **string** | If present, regular expression matching file names | [optional] [default to null]
**Scope** | [***RestSecretScanningRuleScope**](RestSecretScanningRule_scope.md) |  | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

