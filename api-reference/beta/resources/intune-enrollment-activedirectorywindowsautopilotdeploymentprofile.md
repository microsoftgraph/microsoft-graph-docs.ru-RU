---
title: Тип ресурса Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Профиль развертывания Windows для автопилота
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 700e89bc5c47b2a39d1aec7c6680a34e49a8a639
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080385"
---
# <a name="activedirectorywindowsautopilotdeploymentprofile-resource-type"></a>Тип ресурса Активедиректоривиндовсаутопилотдеплойментпрофиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль развертывания Windows для автопилота


Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Активедиректоривиндовсаутопилотдеплойментпрофилес](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-list.md)|Коллекция [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Список свойств и связей объектов [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|
|[Получение Активедиректоривиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-get.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Чтение свойств и связей объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|
|[Создание Активедиректоривиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-create.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Создание нового объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|
|[Удаление Активедиректоривиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-delete.md)|Нет|Удаляет объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).|
|[Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле](../api/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile-update.md)|[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)|Обновление свойств объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ профиля, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|displayName|String|Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|description|String|Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|language|String|Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|createdDateTime|DateTimeOffset|Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения профиля, наследуемого от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|Настройка "от" в рамке наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|енроллментстатусскринсеттингс|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|Параметр экрана состояния регистрации, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|екстраксардварехаш|Boolean|Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|девиценаметемплате|String|Шаблон, используемый для именования автопилотного устройства. Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число. Общая длина текста, созданного шаблоном, не может превышать 15 символов. Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|Тип устройства автопилота, к которому применяется этот профиль. Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md). Возможные значения: `windowsPc`, `surfaceHub2`, `holoLens`.|
|енаблевхитеглове|Boolean|Включите для профиля белый Глове для автопилотного развертывания. Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|roleScopeTagIds|Коллекция String|Теги областей для профиля. Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|хибридазуреаджоинскипконнективитичекк|Boolean|Процесс самопилотного подключения к гибридной среде Azure AD продолжится даже в том случае, если он не устанавливает подключение к контроллеру домена во время OOBE.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|ассигнеддевицес|Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Список назначенных устройств для профиля. Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|assignments|Коллекция [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|Список назначений групп для профиля. Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|
|домаинжоинконфигуратион|[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)|Конфигурация для присоединения к домену Active Directory|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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
  ],
  "hybridAzureADJoinSkipConnectivityCheck": true
}
```






