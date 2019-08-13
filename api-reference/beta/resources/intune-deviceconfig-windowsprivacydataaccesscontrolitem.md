---
title: Тип ресурса Виндовспривацидатаакцессконтролитем
description: Указание уровня контроля доступа для каждой категории данных о конфиденциальности
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 077af30aa9abe14ccc74c57a964074475d07cd4c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337708"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a>Тип ресурса Виндовспривацидатаакцессконтролитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указание уровня контроля доступа для каждой категории данных о конфиденциальности

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовспривацидатаакцессконтролитемс](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|Коллекция [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Список свойств и связей объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|
|[Получение Виндовспривацидатаакцессконтролитем](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Чтение свойств и связей объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|
|[Создание Виндовспривацидатаакцессконтролитем](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Создание нового объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|
|[Удаление Виндовспривацидатаакцессконтролитем](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|Нет|Удаляет объект [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).|
|[Обновление Виндовспривацидатаакцессконтролитем](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|Обновление свойств объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ Виндовспривацидатаакцессконтролитем.|
|accessLevel|[виндовспривацидатаакцесслевел](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|Указывает уровень доступа для категории данных о конфиденциальности, в которую будет передано указанное приложение. Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.|
|Категория "|[виндовспривацидатакатегори](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|Указывает категорию данных о конфиденциальности, к которой будет применяться конкретное управление доступом. Возможные значения: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar` `callHistory` `camera` `contacts` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` `microphone` `motion`,,,,,,,,,,,,,,,,,,,,, `diagnosticsInfo` `email` `location` `messaging` .|
|апппаккажефамилинаме|String|Имя семейства пакетов для приложения Windows. Если этот параметр установлен, уровень доступа применяется к указанному приложению.|
|appDisplayName|String|Имя семейства пакетов для приложения Windows. Если этот параметр установлен, уровень доступа применяется к указанному приложению.|

## <a name="relationships"></a>Отношения
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



