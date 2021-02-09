---
title: Тип ресурса deviceManagementAutopilotEvent
description: Представляет событие потока Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef175825e7ab6d84200fdda6caca84b8c4110d1f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159887"
---
# <a name="devicemanagementautopilotevent-resource-type"></a>Тип ресурса deviceManagementAutopilotEvent

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет событие потока Autopilot.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementAutopilotEvents](../api/intune-troubleshooting-devicemanagementautopilotevent-list.md)|[Коллекция deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Список свойств и связей объектов [deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|
|[Get deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-get.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Чтение свойств и связей объекта [deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|
|[Создание deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-create.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Создание объекта [deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|
|[Удаление deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-delete.md)|Нет|Удаляет [deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|
|[Обновление deviceManagementAutopilotEvent](../api/intune-troubleshooting-devicemanagementautopilotevent-update.md)|[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|Обновление свойств объекта [deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|deviceId|String|ИД устройства, связанный с объектом|
|eventDateTime|DateTimeOffset|Время возникновения события.|
|deviceRegisteredDateTime|DateTimeOffset|Дата регистрации устройства.|
|enrollmentStartDateTime|DateTimeOffset|Дата начала регистрации устройства.|
|enrollmentType|[windowsAutopilotEnrollmentType](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|Тип регистрации. Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|String|Серийный номер устройства.|
|managedDeviceName|String|Имя управляемого устройства.|
|userPrincipalName|String|Имя основного пользователя, используемая для регистрации устройства.|
|windowsAutopilotDeploymentProfileDisplayName|String|Имя профиля Autopilot.|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации, например "Зарегистрировано", "Сбой". Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|Имя профиля страницы состояния регистрации|
|windows10EnrollmentCompletionPageConfigurationId|String|ИД профиля страницы состояния регистрации|
|deploymentState|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания, например Success, Failure, InProgress, SuccessWithTimeout. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|deviceSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания для этапа настройки устройства страницы состояния регистрации. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|accountSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания для этапа настройки учетной записи страницы состояния регистрации. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|osVersion|String|Версия операционной системы устройства.|
|deploymentDuration|Duration|Продолжительность развертывания Autopilot, включая регистрацию.|
|deploymentTotalDuration|Duration|Общая продолжительность развертывания от регистрации до экрана рабочего стола.|
|devicePreparationDuration|Duration|Время, затраченное на регистрацию устройств.|
|deviceSetupDuration|Duration|Время, затраченное на ESP устройства.|
|accountSetupDuration|Duration|Время, затраченное на ESP пользователя.|
|deploymentStartDateTime|DateTimeOffset|Время начала развертывания.|
|deploymentEndDateTime|DateTimeOffset|Время окончания развертывания.|
|targetedAppCount|Int32|Количество целевых приложений.|
|targetedPolicyCount|Int32|Количество целевых политик.|
|enrollmentFailureDetails|String|Сведения о сбое регистрации.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|policyStatusDetails|[Коллекция deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Сведения о политике и состоянии приложения для этого устройства.|

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
  "deviceId": "String",
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
  "windows10EnrollmentCompletionPageConfigurationId": "String",
  "deploymentState": "String",
  "deviceSetupStatus": "String",
  "accountSetupStatus": "String",
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




