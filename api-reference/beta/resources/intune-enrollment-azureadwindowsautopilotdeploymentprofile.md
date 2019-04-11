---
title: Тип ресурса Азуреадвиндовсаутопилотдеплойментпрофиле
description: Профиль развертывания Windows для автопилота
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef04802ab7c53b88b5e3afc3e70b6ce3f0137b07
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773660"
---
# <a name="azureadwindowsautopilotdeploymentprofile-resource-type"></a>Тип ресурса Азуреадвиндовсаутопилотдеплойментпрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль развертывания Windows для автопилота


НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Азуреадвиндовсаутопилотдеплойментпрофилес](../api/intune-enrollment-azureadwindowsautopilotdeploymentprofile-list.md)|Коллекция [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)|Список свойств и связей объектов [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .|
|[Получение Азуреадвиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-azureadwindowsautopilotdeploymentprofile-get.md)|[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)|Чтение свойств и связей объекта [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .|
|[Создание Азуреадвиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-azureadwindowsautopilotdeploymentprofile-create.md)|[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)|Создание нового объекта [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .|
|[Удаление Азуреадвиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-azureadwindowsautopilotdeploymentprofile-delete.md)|Нет|Удаляет объект [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).|
|[Обновление Азуреадвиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-azureadwindowsautopilotdeploymentprofile-update.md)|[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)|Обновление свойств объекта [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ профиля, наСледуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|description|String|Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|language|String|Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|createdDateTime|DateTimeOffset|Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения профиля, наСледуемого от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Настройка "от" в рамке наСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|Енроллментстатусскринсеттингс|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Параметр экрана состояния регистрации, наСледуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|Екстраксардварехаш|Boolean|Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|Девиценаметемплате|String|Шаблон, используемый для именования автоПилотного устройства. Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число. Общая длина текста, созданного шаблоном, не может превышать 15 символов. НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|Тип устройства автоПилота, к которому применяется этот профиль. НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md). Возможные значения: `windowsPc`, `surfaceHub2`.|
|Енаблевхитеглове|Boolean|Включите для профиля белый Глове для автопилотного развертывания. НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Ассигнеддевицес|Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Список назначенных устройств для профиля. НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|
|assignments|Коллекция [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Список назначений групп для профиля. НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.azureADWindowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
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
  "enableWhiteGlove": true
}
```





