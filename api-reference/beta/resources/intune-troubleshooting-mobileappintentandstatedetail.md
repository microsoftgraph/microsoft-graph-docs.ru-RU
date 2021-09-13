---
title: тип ресурса mobileAppAppIntentAndStateDetail
description: Намерение мобильного приложения и установка состояния для данного устройства.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92f3e301e16b14f7a1aac1ed9dc27a60d53b2850
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59100892"
---
# <a name="mobileappintentandstatedetail-resource-type"></a>тип ресурса mobileAppAppIntentAndStateDetail

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Намерение мобильного приложения и установка состояния для данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationId|String|Идентификатор MobieApp.|
|displayName|String|Название приложения, которое предоставил или импортировал администратор.|
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




