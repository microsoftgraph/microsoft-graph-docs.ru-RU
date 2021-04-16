---
title: тип ресурса windowsAutopilotDeploymentProfile
description: Профиль развертывания автопилота Windows
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 101575bca59db6a19153b26e54fc868b2e1b6472
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864944"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>тип ресурса windowsAutopilotDeploymentProfile

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль развертывания автопилота Windows

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получить windowsAutopilotDeploymentProfile](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Чтение свойств и связей [объекта windowsAutopilotDeploymentProfile.](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|[Действие assign](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[действие hasPayloadLinks](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля|
|displayName|String|Имя профиля|
|description|String|Описание профиля|
|language|String|Язык, настроенный на устройстве|
|createdDateTime|DateTimeOffset|Время создания профиля|
|lastModifiedDateTime|DateTimeOffset|Последнее изменение профиля|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Параметр "Вне параметров работы с полем"|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Параметр состояния регистрации|
|extractHardwareHash|Логический|HardwareHash Extraction для профиля|
|deviceNameTemplate|String|Шаблон, используемый для имени устройства АвтоПилот. Это может быть пользовательский текст, который также может содержать либо серийный номер устройства, либо случайный генерируемый номер. Общая длина текста, генерируемого шаблоном, может быть не более 15 символов.|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|Тип устройства AutoPilot, к который применим этот профиль. Возможные значения: `windowsPc`, `surfaceHub2`.|
|enableWhiteGlove|Логический|Включить белую перчатку автопилота для профиля.|
|roleScopeTagIds|Коллекция String|Теги области для профиля.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Регистрация**|
|assignedDevices|[коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Список назначенных устройств для профиля.|
|assignments|[коллекция windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Список групповых назначений для профиля.|

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
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




