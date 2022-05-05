---
title: Обновление zebraFotaDeployment
description: Обновление свойств объекта zebraFotaDeployment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d4b1d42cb140fd1acbc485ffe4f7b8d5d98843d8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213530"
---
# <a name="update-zebrafotadeployment"></a>Обновление zebraFotaDeployment

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/zebraFotaDeployments/{zebraFotaDeploymentId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Созданный системой идентификатор развертывания, предоставленный во время создания развертывания. Возвращается, только если операция выполнена успешно.|
|displayName|Строка|Понятное имя развертывания.|
|description|Строка|Понятное описание развертывания.|
|deploymentSettings|[zebraFotaDeploymentSettings](../resources/intune-androidfotaservice-zebrafotadeploymentsettings.md)|Представляет параметры, необходимые для создания развертывания, такие как тип развертывания, сведения об артефакте, скачивание и установка|
|deploymentAssignments|[Коллекция androidFotaDeploymentAssignment](../resources/intune-androidfotaservice-androidfotadeploymentassignment.md)|Коллекция назначений FOTA для Android|
|deploymentStatus|[zebraFotaDeploymentStatus](../resources/intune-androidfotaservice-zebrafotadeploymentstatus.md)|Представляет состояние развертывания от Zebra. Состояние — это высокоуровневый статус развертывания, а не подробное состояние для каждого устройства.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/zebraFotaDeployments/{zebraFotaDeploymentId}
Content-type: application/json
Content-length: 1892

{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "displayName": "Display Name value",
  "description": "Description value",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "Device Model value",
    "updateType": "latest",
    "timeZoneOffsetInMinutes": 7,
    "firmwareTargetBoardSupportPackageVersion": "Firmware Target Board Support Package Version value",
    "firmwareTargetPatch": "Firmware Target Patch value",
    "firmwareTargetOsVersion": "Firmware Target Os Version value",
    "scheduleMode": "scheduled",
    "scheduleDurationInDays": 6,
    "downloadRuleNetworkType": "wifi",
    "downloadRuleStartDateTime": "2016-12-31T23:59:33.2519835-08:00",
    "installRuleStartDateTime": "2017-01-01T00:02:31.1558076-08:00",
    "installRuleWindowStartTime": "11:57:19.2230000",
    "installRuleWindowEndTime": "11:58:38.5330000",
    "batteryRuleMinimumBatteryLevelPercentage": 8,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "Id value",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "Group Id value"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "createFailed",
    "totalDevices": 12,
    "totalCreated": 12,
    "totalScheduled": 14,
    "totalDownloading": 0,
    "totalAwaitingInstall": 4,
    "totalSucceededInstall": 5,
    "totalCanceled": 13,
    "totalUnknown": 12,
    "totalFailedDownload": 3,
    "totalFailedInstall": 2,
    "completeOrCanceledDateTime": "2016-12-31T23:59:29.651377-08:00",
    "cancelRequested": true,
    "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1941

{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "id": "8bbfa8a0-a8a0-8bbf-a0a8-bf8ba0a8bf8b",
  "displayName": "Display Name value",
  "description": "Description value",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "Device Model value",
    "updateType": "latest",
    "timeZoneOffsetInMinutes": 7,
    "firmwareTargetBoardSupportPackageVersion": "Firmware Target Board Support Package Version value",
    "firmwareTargetPatch": "Firmware Target Patch value",
    "firmwareTargetOsVersion": "Firmware Target Os Version value",
    "scheduleMode": "scheduled",
    "scheduleDurationInDays": 6,
    "downloadRuleNetworkType": "wifi",
    "downloadRuleStartDateTime": "2016-12-31T23:59:33.2519835-08:00",
    "installRuleStartDateTime": "2017-01-01T00:02:31.1558076-08:00",
    "installRuleWindowStartTime": "11:57:19.2230000",
    "installRuleWindowEndTime": "11:58:38.5330000",
    "batteryRuleMinimumBatteryLevelPercentage": 8,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "Id value",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "Group Id value"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "createFailed",
    "totalDevices": 12,
    "totalCreated": 12,
    "totalScheduled": 14,
    "totalDownloading": 0,
    "totalAwaitingInstall": 4,
    "totalSucceededInstall": 5,
    "totalCanceled": 13,
    "totalUnknown": 12,
    "totalFailedDownload": 3,
    "totalFailedInstall": 2,
    "completeOrCanceledDateTime": "2016-12-31T23:59:29.651377-08:00",
    "cancelRequested": true,
    "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
  }
}
```




