---
title: тип ресурса iosMobileAppConfiguration
description: Содержит свойства, унаследованные свойства и действия для конфигураций мобильного приложения для iOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 576f29db33adc430603648c0db065ff73b83505f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418570"
---
# <a name="iosmobileappconfiguration-resource-type"></a>тип ресурса iosMobileAppConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, унаследованные свойства и действия для конфигураций мобильного приложения для iOS.


Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosMobileAppConfigurations](../api/intune-apps-iosmobileappconfiguration-list.md)|коллекция [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|Список свойств и связей объектов [iosUpdateConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).|
|[Получить iosMobileAppConfiguration](../api/intune-apps-iosmobileappconfiguration-get.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|Считывание свойств и связей объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).|
|[Создать iosMobileAppConfiguration](../api/intune-apps-iosmobileappconfiguration-create.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|Создание нового объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).|
|[Удалить iosMobileAppConfiguration](../api/intune-apps-iosmobileappconfiguration-delete.md)|Отсутствует|Удаляет [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).|
|[Обновить iosMobileAppConfiguration](../api/intune-apps-iosmobileappconfiguration-update.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|targetedMobileApps|Коллекция String|приложение-обработчик Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|roleScopeTagIds|Коллекция String|Список областей теги для данного объекта конфигурации приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|описание|String|Администратор предоставил описание конфигурация устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|displayName|String|Администратор предоставил название конфигурации устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|версия|Int32|Версия конфигурации устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|encodedSettingXml|Двоичный|конфигурация приложения службы управления мобильными устройствами двоичная Base64.|
|параметры|коллекция [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)|элементы параметра конфигурации приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Список заданий группы для настройки приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) коллекции|Список ManagedDeviceMobileAppConfigurationDeviceStatus. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|userStatuses|Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)|Список объектов ManagedDeviceMobileAppConfigurationUserStatus. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Общие сведения о состоянии устройства, связанном с настройкой приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|Общие сведения о состоянии пользователя, связанном с настройкой приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "encodedSettingXml": "binary",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "String",
      "appConfigKeyType": "String",
      "appConfigKeyValue": "String"
    }
  ]
}
```




