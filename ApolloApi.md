All URIs are relative to *https://192.168.150.2:8090/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authLogin**](ApolloApi.md#authlogin) | **POST** /auth/login | Login a user using email and password
[**profileShow**](ApolloApi.md#profileshow) | **GET** /user/profile | Show a user profile
[**userList**](ApolloApi.md#userlist) | **GET** /user/list | List users
[**userShow**](ApolloApi.md#usershow) | **GET** /user | Show a user
[**workoutSetExport**](ApolloApi.md#workoutsetexport) | **GET** /workout-set/export | Export a range of workout sets


# **authLogin**
> UserResponse authLogin(email, password, refreshable, apiVersion)

Login a user using email and password

1

### Example
```dart
import 'package:keiser_apollo_sdk/api.dart';

final api = KeiserApolloSdk().getApolloApi();
final String email = email_example; // String | 
final String password = password_example; // String | 
final bool refreshable = true; // bool | 
final String apiVersion = apiVersion_example; // String | 

try {
    final response = api.authLogin(email, password, refreshable, apiVersion);
    print(response);
} catch on DioError (e) {
    print('Exception when calling ApolloApi->authLogin: $e\n');
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **String**|  | 
 **password** | **String**|  | 
 **refreshable** | **bool**|  | [optional] 
 **apiVersion** | **String**|  | [optional] 

### Return type

[**UserResponse**](UserResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **profileShow**
> ProfileResponse profileShow(userId, apiVersion)

Show a user profile

1

### Example
```dart
import 'package:keiser_apollo_sdk/api.dart';
// TODO Configure HTTP basic authorization: bearerAuth
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').username = 'YOUR_USERNAME'
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').password = 'YOUR_PASSWORD';

final api = KeiserApolloSdk().getApolloApi();
final num userId = 8.14; // num | 
final String apiVersion = apiVersion_example; // String | 

try {
    final response = api.profileShow(userId, apiVersion);
    print(response);
} catch on DioError (e) {
    print('Exception when calling ApolloApi->profileShow: $e\n');
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **num**|  | [optional] 
 **apiVersion** | **String**|  | [optional] 

### Return type

[**ProfileResponse**](ProfileResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **userList**
> UserListResponse userList(accountTypes, ascending, limit, name, offset, sort, apiVersion)

List users

1

### Example
```dart
import 'package:keiser_apollo_sdk/api.dart';
// TODO Configure HTTP basic authorization: bearerAuth
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').username = 'YOUR_USERNAME'
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').password = 'YOUR_PASSWORD';

final api = KeiserApolloSdk().getApolloApi();
final List<String> accountTypes = ; // List<String> | 
final bool ascending = true; // bool | 
final num limit = 8.14; // num | 
final String name = name_example; // String | 
final num offset = 8.14; // num | 
final String sort = sort_example; // String | 
final String apiVersion = apiVersion_example; // String | 

try {
    final response = api.userList(accountTypes, ascending, limit, name, offset, sort, apiVersion);
    print(response);
} catch on DioError (e) {
    print('Exception when calling ApolloApi->userList: $e\n');
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountTypes** | [**List&lt;String&gt;**](String.md)|  | [optional] 
 **ascending** | **bool**|  | [optional] [default to true]
 **limit** | **num**|  | [optional] [default to 20]
 **name** | **String**|  | [optional] 
 **offset** | **num**|  | [optional] [default to 0]
 **sort** | **String**|  | [optional] [default to 'id']
 **apiVersion** | **String**|  | [optional] 

### Return type

[**UserListResponse**](UserListResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **userShow**
> UserResponse userShow(userId, apiVersion)

Show a user

1

### Example
```dart
import 'package:keiser_apollo_sdk/api.dart';
// TODO Configure HTTP basic authorization: bearerAuth
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').username = 'YOUR_USERNAME'
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').password = 'YOUR_PASSWORD';

final api = KeiserApolloSdk().getApolloApi();
final num userId = 8.14; // num | 
final String apiVersion = apiVersion_example; // String | 

try {
    final response = api.userShow(userId, apiVersion);
    print(response);
} catch on DioError (e) {
    print('Exception when calling ApolloApi->userShow: $e\n');
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **num**|  | [optional] 
 **apiVersion** | **String**|  | [optional] 

### Return type

[**UserResponse**](UserResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workoutSetExport**
> WorkoutSetExportResponse workoutSetExport(from, to, apiVersion)

Export a range of workout sets

1

### Example
```dart
import 'package:keiser_apollo_sdk/api.dart';
// TODO Configure HTTP basic authorization: bearerAuth
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').username = 'YOUR_USERNAME'
//defaultApiClient.getAuthentication<HttpBasicAuth>('bearerAuth').password = 'YOUR_PASSWORD';

final api = KeiserApolloSdk().getApolloApi();
final DateTime from = 2013-10-20T19:20:30+01:00; // DateTime | 
final DateTime to = 2013-10-20T19:20:30+01:00; // DateTime | 
final String apiVersion = apiVersion_example; // String | 

try {
    final response = api.workoutSetExport(from, to, apiVersion);
    print(response);
} catch on DioError (e) {
    print('Exception when calling ApolloApi->workoutSetExport: $e\n');
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from** | **DateTime**|  | 
 **to** | **DateTime**|  | 
 **apiVersion** | **String**|  | [optional] 

### Return type

[**WorkoutSetExportResponse**](WorkoutSetExportResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
