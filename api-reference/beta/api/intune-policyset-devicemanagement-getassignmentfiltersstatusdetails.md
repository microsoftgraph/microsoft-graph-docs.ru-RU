---
title: действие getAssignmentFiltersStatusDetails
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1fb011c4514705e4416d1eba6fa9fee622276b2b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788747"
---
# <a name="getassignmentfiltersstatusdetails-action"></a>действие getAssignmentFiltersStatusDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/getAssignmentFiltersStatusDetails
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Свойство|Тип|Описание|
|:---|:---|:---|
|managedDeviceId|String|Пока не задокументировано.|
|payloadId|String|Пока не задокументировано.|
|userId|String|Пока не задокументировано.|
|assignmentFilterIds|Коллекция строк|Н/Д|
|top|Int32|Пока не задокументировано.|
|skip|Int32|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения это действие возвращает код ответа и `200 OK` [назначениеFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/getAssignmentFiltersStatusDetails

Content-type: application/json
Content-length: 214

{
  "managedDeviceId": "Managed Device Id value",
  "payloadId": "Payload Id value",
  "userId": "User Id value",
  "assignmentFilterIds": [
    "Assignment Filter Ids value"
  ],
  "top": 3,
  "skip": 4
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

{
  "value": {
    "@odata.type": "microsoft.graph.assignmentFilterStatusDetails",
    "managedDeviceId": "Managed Device Id value",
    "payloadId": "Payload Id value",
    "userId": "User Id value",
    "deviceProperties": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "evalutionSummaries": [
      {
        "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
        "assignmentFilterId": "Assignment Filter Id value",
        "assignmentFilterLastModifiedDateTime": "2017-01-01T00:02:50.0900701-08:00",
        "assignmentFilterDisplayName": "Assignment Filter Display Name value",
        "assignmentFilterPlatform": "androidForWork",
        "evaluationResult": "match",
        "evaluationDateTime": "2016-12-31T23:58:01.2047675-08:00",
        "assignmentFilterType": "include",
        "assignmentFilterTypeAndEvaluationResults": [
          {
            "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
            "assignmentFilterType": "include",
            "evaluationResult": "match"
          }
        ]
      }
    ]
  }
}
```



