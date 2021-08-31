---
title: тип ресурса windowsPrivacyDataAccessControlItem
description: Укажите уровень управления доступом в каждой категории данных конфиденциальности
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5667c2172f6cd633dd688ce104704c4f997449f8
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795201"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>тип ресурса windowsPrivacyDataAccessControlItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Укажите уровень управления доступом в каждой категории данных конфиденциальности

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsPrivacyDataAccessControlItems](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|[коллекция windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Список свойств и связей [объектов windowsPrivacyDataAccesssControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|
|[Get windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Чтение свойств и связей [объекта windowsPrivacyDataAccesssControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|
|[Создание windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Создайте [новый объект WindowsPrivacyDataAccessControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|
|[Удаление windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|Нет|Удаляет [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).|
|[Обновление windowsPrivacyDataAccessControlItem](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Обновление свойств объекта [windowsPrivacyDataAccesssControlItem.](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ WindowsPrivacyDataAccessControlItem.|
|accessLevel|[windowsPrivacyDataAccessLevel](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Это указывает уровень доступа к категории данных конфиденциальности, которой будет предоставлено указанное приложение. Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|dataCategory|[windowsPrivacyDataCategory](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Это указывает на категорию данных конфиденциальности, к которой будет применяться определенный контроль доступа. Возможные значения: `notConfigured` `accountInfo` , , , , , `appsRunInBackground` , , , `calendar` `callHistory` , , `camera` `contacts` `diagnosticsInfo` `email` , `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` .|
|appPackageFamilyName|Строка|Имя семейства пакета приложения Windows. При наборе уровень доступа применяется к указанному приложению.|
|appDisplayName|String|Имя семейства пакета приложения Windows. При наборе уровень доступа применяется к указанному приложению.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```



