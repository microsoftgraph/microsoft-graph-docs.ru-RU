---
title: summarizeDeviceRemoteConnection
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cbb5b3a722fed0c8ab798b8c1274158b115cf94
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342050"
---
# <a name="summarizedeviceremoteconnection-function"></a>summarizeDeviceRemoteConnection

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.
В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.

|Свойство|Тип|Описание|
|:---|:---|:---|
|summarizeBy|[userExperienceAnalyticsSummarizedBy](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успеха эта функция возвращает код отклика и `200 OK` [коллекцию userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection(summarizeBy='parameterValue')
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
      "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "virtualNetwork": "Virtual Network value",
      "manufacturer": "Manufacturer value",
      "deviceCount": 11,
      "cloudPcRoundTripTime": 6.666666666666667,
      "cloudPcSignInTime": 5.666666666666667,
      "remoteSignInTime": 5.333333333333333,
      "coreBootTime": 4.0,
      "coreSignInTime": 4.666666666666667,
      "cloudPcFailurePercentage": 8.0,
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




