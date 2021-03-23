# DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAlarm**](DefaultApi.md#createAlarm) | **POST** /alarms | 
[**listAlarms**](DefaultApi.md#listAlarms) | **GET** /alarms | 


<a name="createAlarm"></a>
# **createAlarm**
> Alarm createAlarm(NewAlarm)



    a new alarm

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **NewAlarm** | [**NewAlarm**](../Models/NewAlarm.md)| alarm to schedule | [optional]

### Return type

[**Alarm**](../Models/Alarm.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="listAlarms"></a>
# **listAlarms**
> List listAlarms()



    list alarms

### Parameters
This endpoint does not need any parameter.

### Return type

[**List**](../Models/Alarm.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

