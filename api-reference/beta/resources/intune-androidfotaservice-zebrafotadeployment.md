---
title: Тип ресурса zebraFotaDeployment
description: Сущность развертывания Zebra FOTA, которая описывает параметры, группы устройств развертывания, необходимые для создания развертывания FOTA, и состояние развертывания.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d3ba6ffd223320be5bfbe1b259768534a47941c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213570"
---
# <a name="zebrafotadeployment-resource-type"></a>Тип ресурса zebraFotaDeployment

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность развертывания Zebra FOTA, которая описывает параметры, группы устройств развертывания, необходимые для создания развертывания FOTA, и состояние развертывания.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-list.md)|[Коллекция zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Список свойств и связей объектов [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[Получение zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-get.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Чтение свойств и связей объекта [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[Создание zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-create.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Создайте объект [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[Удаление zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-delete.md)|Нет|Удаляет [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md).|
|[Обновление zebraFotaDeployment](../api/intune-androidfotaservice-zebrafotadeployment-update.md)|[zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md)|Обновление свойств объекта [zebraFotaDeployment](../resources/intune-androidfotaservice-zebrafotadeployment.md) .|
|[Действие отмены](../api/intune-androidfotaservice-zebrafotadeployment-cancel.md)|Boolean|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Созданный системой идентификатор развертывания, предоставленный во время создания развертывания. Возвращается, только если операция выполнена успешно.|
|displayName|Строка|Понятное имя развертывания.|
|description|Строка|Понятное описание развертывания.|
|deploymentSettings|[zebraFotaDeploymentSettings](../resources/intune-androidfotaservice-zebrafotadeploymentsettings.md)|Представляет параметры, необходимые для создания развертывания, такие как тип развертывания, сведения об артефакте, скачивание и установка|
|deploymentAssignments|[Коллекция androidFotaDeploymentAssignment](../resources/intune-androidfotaservice-androidfotadeploymentassignment.md)|Коллекция назначений FOTA для Android|
|deploymentStatus|[zebraFotaDeploymentStatus](../resources/intune-androidfotaservice-zebrafotadeploymentstatus.md)|Представляет состояние развертывания от Zebra. Состояние — это высокоуровневый статус развертывания, а не подробное состояние для каждого устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaDeployment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeployment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "deploymentSettings": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings",
    "deviceModel": "String",
    "updateType": "String",
    "timeZoneOffsetInMinutes": 1024,
    "firmwareTargetBoardSupportPackageVersion": "String",
    "firmwareTargetPatch": "String",
    "firmwareTargetOsVersion": "String",
    "scheduleMode": "String",
    "scheduleDurationInDays": 1024,
    "downloadRuleNetworkType": "String",
    "downloadRuleStartDateTime": "String (timestamp)",
    "installRuleStartDateTime": "String (timestamp)",
    "installRuleWindowStartTime": "String (time of day)",
    "installRuleWindowEndTime": "String (time of day)",
    "batteryRuleMinimumBatteryLevelPercentage": 1024,
    "batteryRuleRequireCharger": true
  },
  "deploymentAssignments": [
    {
      "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment",
      "id": "String",
      "target": {
        "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
        "groupId": "String"
      }
    }
  ],
  "deploymentStatus": {
    "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus",
    "state": "String",
    "totalDevices": 1024,
    "totalCreated": 1024,
    "totalScheduled": 1024,
    "totalDownloading": 1024,
    "totalAwaitingInstall": 1024,
    "totalSucceededInstall": 1024,
    "totalCanceled": 1024,
    "totalUnknown": 1024,
    "totalFailedDownload": 1024,
    "totalFailedInstall": 1024,
    "completeOrCanceledDateTime": "String (timestamp)",
    "cancelRequested": true,
    "lastUpdatedDateTime": "String (timestamp)"
  }
}
```




