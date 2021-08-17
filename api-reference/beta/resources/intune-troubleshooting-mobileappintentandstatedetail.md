---
title: тип ресурса mobileAppAppIntentAndStateDetail
description: Намерение мобильного приложения и установка состояния для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f0bb527af5e155ecb55558e890e551eb15b9791
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256649"
---
# <a name="mobileappintentandstatedetail-resource-type"></a>тип ресурса mobileAppAppIntentAndStateDetail

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Намерение мобильного приложения и установка состояния для данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationId|String|Идентификатор MobieApp.|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор.|
|mobileAppIntent|[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);|Намерение мобильного приложения. Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.|
|displayVersion|String|Читаемая для человека версия приложения|
|installState|[resultantAppState](../resources/intune-troubleshooting-resultantappstate.md)|Состояние установки приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|supportedDeviceTypes|[коллекция mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)|Поддерживаемые платформы для приложения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```




