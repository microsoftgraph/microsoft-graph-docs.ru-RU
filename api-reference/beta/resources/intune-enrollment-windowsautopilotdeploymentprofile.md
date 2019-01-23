---
title: Тип ресурса windowsAutopilotDeploymentProfile
description: Windows автопилот развертывания профилей
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f97603980f4e76c4dd2f63287822a1e8e984ded
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394112"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>Тип ресурса windowsAutopilotDeploymentProfile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows автопилот развертывания профилей

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsAutopilotDeploymentProfile](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Чтение свойства и связи объекта [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .|
|[Действие assign](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша профилей|
|displayName|String|Имя профиля|
|description|String|Описание профиля|
|language|String|Язык, настроенных на устройстве|
|createdDateTime|DateTimeOffset|Время создания профилей|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения профиля|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|В соответствующем взаимодействия параметр|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Параметр экрана состояния подачи заявок|
|extractHardwareHash|Логический|Извлечение HardwareHash для профиля|
|deviceNameTemplate|String|Шаблон, используемый для имя устройства автопилот. Это может быть настраиваемого текста, а также может содержать серийный номер устройства или случайное число. Общая длина текста, созданной с помощью шаблона может быть не более 15 символов.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) коллекции|Список устройств, назначенных для профиля.|
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) коллекции|Список назначений группы для профиля.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String"
}
```




