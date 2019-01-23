---
title: Тип ресурса androidManagedStoreAppConfiguration
description: Содержит свойства, наследуемые свойства и действия для конфигурации мобильного приложения Android предприятия.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b232bd2ad6c2eefb796387c3a8a881540f3e971a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412158"
---
# <a name="androidmanagedstoreappconfiguration-resource-type"></a>Тип ресурса androidManagedStoreAppConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, наследуемые свойства и действия для конфигурации мобильного приложения Android предприятия.


Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidManagedStoreAppConfigurations](../api/intune-apps-androidmanagedstoreappconfiguration-list.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) коллекции|Свойства списка и связей объектов [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|
|[Получение androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-get.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|Чтение свойства и связи объекта [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|
|[Создание androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-create.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|Создание нового объекта [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|
|[Удаление androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-delete.md)|Нет|Удаляет [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).|
|[Обновление androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-update.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|Обновление свойства объекта [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|

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
|packageId|String|Идентификатор приложения пакета конфигурации Android предприятия.|
|payloadJson|String|Android корпоративного приложения конфигурации JSON полезных данных.|
|permissionActions|[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) коллекции|Список разрешений для Android и соответствующие действия разрешений.|

## <a name="relationships"></a>Отношения
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
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
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
  "packageId": "String",
  "payloadJson": "String",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "String",
      "action": "String"
    }
  ]
}
```




