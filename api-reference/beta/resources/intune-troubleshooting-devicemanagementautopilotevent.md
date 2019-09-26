---
title: Тип ресурса Девицеманажементаутопилотевент
description: Представляет событие процесса автопилота.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0ceaf629e9955fedb80910c7363caabfecfa290d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201187"
---
# <a name="devicemanagementautopilotevent-resource-type"></a>Тип ресурса Девицеманажементаутопилотевент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет событие процесса автопилота.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементаутопилотевентс](../api/intune-troubleshooting-devicemanagementautopilotevent-list.md)|Коллекция [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Список свойств и связей объектов [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|
|[Получение Девицеманажементаутопилотевент](../api/intune-troubleshooting-devicemanagementautopilotevent-get.md)|[девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Чтение свойств и связей объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|
|[Создание Девицеманажементаутопилотевент](../api/intune-troubleshooting-devicemanagementautopilotevent-create.md)|[девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Создание нового объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|
|[Удаление Девицеманажементаутопилотевент](../api/intune-troubleshooting-devicemanagementautopilotevent-delete.md)|Нет|Удаляет объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md).|
|[Обновление Девицеманажементаутопилотевент](../api/intune-troubleshooting-devicemanagementautopilotevent-update.md)|[девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Обновление свойств объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|UUID объекта.|
|eventDateTime|DateTimeOffset|Время возникновения события.|
|девицерегистереддатетиме|DateTimeOffset|Дата регистрации устройства.|
|енроллментстартдатетиме|DateTimeOffset|Дата начала регистрации устройства.|
|enrollmentType|[виндовсаутопилотенроллменттипе](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|Тип регистрации. Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|девицесериалнумбер|String.|Серийный номер устройства.|
|managedDeviceName|String|Управляемое имя устройства.|
|userPrincipalName|String|Имя участника пользователя, используемое для регистрации устройства.|
|виндовсаутопилотдеплойментпрофиледисплайнаме|String.|Имя профиля для автопилота.|
|енроллментстате|[енроллментстате](../resources/intune-shared-enrollmentstate.md)|Не удалось зарегистрировать состояние регистрации, например "зарегистрировано". Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String.|Имя профиля страницы состояния регистрации|
|деплойментстате|[виндовсаутопилотдеплойментстате](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|osVersion|String.|Версия операционной системы устройства.|
|деплойментдуратион|Duration (Длительность)|Длительность развертывания с автопилотной версией, включая регистрацию.|
|деплойменттоталдуратион|Duration (Длительность)|Общее время развертывания с экрана регистрации на рабочем столе.|
|девицепрепаратиондуратион|Duration (Длительность)|Время, затраченное на регистрацию устройств.|
|девицесетупдуратион|Duration (Длительность)|Время, затраченное на устройство ESP.|
|аккаунтсетупдуратион|Duration (Длительность)|Время, затраченное на ESP пользователем.|
|деплойментстартдатетиме|DateTimeOffset|Время начала развертывания.|
|деплойментенддатетиме|DateTimeOffset|Время окончания развертывания.|
|таржетедаппкаунт|Int32|Количество целевых приложений.|
|таржетедполицикаунт|Int32|Количество целевых политик.|
|енроллментфаилуредетаилс|String.|Сведения о сбоях при регистрации.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "deviceRegisteredDateTime": "String (timestamp)",
  "enrollmentStartDateTime": "String (timestamp)",
  "enrollmentType": "String",
  "deviceSerialNumber": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "windowsAutopilotDeploymentProfileDisplayName": "String",
  "enrollmentState": "String",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "String",
  "deploymentState": "String",
  "osVersion": "String",
  "deploymentDuration": "String (duration)",
  "deploymentTotalDuration": "String (duration)",
  "devicePreparationDuration": "String (duration)",
  "deviceSetupDuration": "String (duration)",
  "accountSetupDuration": "String (duration)",
  "deploymentStartDateTime": "String (timestamp)",
  "deploymentEndDateTime": "String (timestamp)",
  "targetedAppCount": 1024,
  "targetedPolicyCount": 1024,
  "enrollmentFailureDetails": "String"
}
```



