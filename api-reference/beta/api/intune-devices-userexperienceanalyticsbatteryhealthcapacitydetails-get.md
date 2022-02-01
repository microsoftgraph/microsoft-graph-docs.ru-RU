---
title: Get userExperienceAnalyticsBatteryHealthCapacityDetails
description: Ознакомьтесь с свойствами и отношениями объекта userExperienceAnalyticsBatteryHealthCapacityDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9652cef38435ee3ecbe2afe3af80171c04ab43d2
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290450"
---
# <a name="get-userexperienceanalyticsbatteryhealthcapacitydetails"></a>Get userExperienceAnalyticsBatteryHealthCapacityDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ознакомьтесь с свойствами и отношениями [объекта userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsBatteryHealthCapacityDetails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот `200 OK` метод возвращает код отклика и [объект userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthCapacityDetails
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 351

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails",
    "id": "b01fc7df-c7df-b01f-dfc7-1fb0dfc71fb0",
    "activeDevices": 13,
    "batteryCapacityGood": 3,
    "batteryCapacityFair": 3,
    "batteryCapacityPoor": 3,
    "lastRefreshedDateTime": "2017-01-01T00:02:37.7100903-08:00"
  }
}
```




