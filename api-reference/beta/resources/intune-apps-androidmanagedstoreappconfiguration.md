---
title: Тип ресурса Андроидманажедстореаппконфигуратион
description: Содержит свойства, унаследованные свойства и действия для конфигураций мобильного приложения Android Enterprise.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f89bd01897f7891bb32dac928686e02110aaa889
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261239"
---
# <a name="androidmanagedstoreappconfiguration-resource-type"></a>Тип ресурса Андроидманажедстореаппконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, унаследованные свойства и действия для конфигураций мобильного приложения Android Enterprise.


Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидманажедстореаппконфигуратионс](../api/intune-apps-androidmanagedstoreappconfiguration-list.md)|Коллекция [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|Список свойств и связей объектов [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|
|[Получение Андроидманажедстореаппконфигуратион](../api/intune-apps-androidmanagedstoreappconfiguration-get.md)|[андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|Чтение свойств и связей объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|
|[Создание Андроидманажедстореаппконфигуратион](../api/intune-apps-androidmanagedstoreappconfiguration-create.md)|[андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|Создание нового объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|
|[Удаление Андроидманажедстореаппконфигуратион](../api/intune-apps-androidmanagedstoreappconfiguration-delete.md)|Нет|Удаляет объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md).|
|[Обновление Андроидманажедстореаппконфигуратион](../api/intune-apps-androidmanagedstoreappconfiguration-update.md)|[андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|Обновление свойств объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|targetedMobileApps|Коллекция String|приложение-обработчик Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этой сущности конфигурации приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|description|String|Администратор предоставил описание конфигурации устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|displayName|String|Администратор предоставил название конфигурации устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|версия|Int32|Версия конфигурации устройства. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|packageId|String|Идентификатор пакета конфигурации корпоративных приложений Android.|
|пайлоаджсон|String|Полезные данные JSON конфигурации корпоративных приложений Android.|
|пермиссионактионс|Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)|Список разрешений приложений для Android и соответствующие действия с разрешениями.|
|аппсуппортсоемконфиг|Boolean|Указывает, является ли Аппконфиг политикой Оемконфиг.|
|профилеаппликабилити|[androidProfileApplicability](../resources/intune-apps-androidprofileapplicability.md)|Применимость профиля предприятия Android (Андроидворкпрофиле, Девицеовнер или Default (применяется к обоим). Возможные значения: `default`, `androidWorkProfile`, `androidDeviceOwner`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Список заданий группы для настройки приложения. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
|deviceStatuses|Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Список ManagedDeviceMobileAppConfigurationDeviceStatus. Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);|
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
  ],
  "appSupportsOemConfig": true,
  "profileApplicability": "String"
}
```




