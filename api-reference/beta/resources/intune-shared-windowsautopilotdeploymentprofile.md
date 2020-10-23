---
title: Тип ресурса windowsAutopilotDeploymentProfile
description: Профиль развертывания Windows для автопилота
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 43cd91db1eb0d0d476d590601ba131cc526ea90d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726275"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>Тип ресурса windowsAutopilotDeploymentProfile

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль развертывания Windows для автопилота

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsAutopilotDeploymentProfile](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Чтение свойств и связей объекта [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) .|
|[Действие assign](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[действие Хаспайлоадлинкс](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ профиля|
|displayName|Строка|Имя профиля|
|description|Строка|Описание профиля|
|language|String|Язык, настроенный на устройстве|
|createdDateTime|DateTimeOffset|Время создания профиля|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения профиля|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Настройка "нет на месте"|
|енроллментстатусскринсеттингс|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Настройка экрана состояния регистрации|
|екстраксардварехаш|Логический|Извлечение Хардварехаш для профиля|
|девиценаметемплате|Строка|Шаблон, используемый для именования автопилотного устройства. Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число. Общая длина текста, созданного шаблоном, не может превышать 15 символов.|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|Тип устройства автопилота, к которому применяется этот профиль. Возможные значения: `windowsPc`, `surfaceHub2`.|
|енаблевхитеглове|Логический|Включите для профиля белый Глове для автопилотного развертывания.|
|roleScopeTagIds|Коллекция строк|Теги областей для профиля.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Регистрации**|
|ассигнеддевицес|Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Список назначенных устройств для профиля.|
|assignments|Коллекция [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Список назначений групп для профиля.|

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





