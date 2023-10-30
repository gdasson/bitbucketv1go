# RestRequiredBuildCondition

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int64** |  | [optional] [default to null]
**BuildParentKeys** | **[]string** | A non-empty list of build parent keys that require green builds for this merge check to pass | [optional] [default to null]
**RefMatcher** | [***RestRequiredBuildConditionRefMatcher**](RestRequiredBuildCondition_refMatcher.md) |  | [optional] [default to null]
**ExemptRefMatcher** | [***RestRequiredBuildConditionRefMatcher**](RestRequiredBuildCondition_refMatcher.md) |  | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

