---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: tfitzmac
ms.openlocfilehash: 9e40f656a7ce4d511cdb4c597c2419e8cf886c12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353615"
---
# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Категории устройств используются для упорядочивания устройств. Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации.Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceCategories](../api/intune-shared-devicecategory-list.md) коллекции|Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Получение объекта deviceCategory](../api/intune-shared-devicecategory-get.md)|Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Создание объекта deviceCategory](../api/intune-shared-devicecategory-create.md)|Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Удаление deviceCategory](../api/intune-shared-devicecategory-delete.md).|
|[Обновление объекта deviceCategory](../api/intune-shared-devicecategory-update.md)|Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор категории устройства. Только для чтения.|
|**Адаптация новых сотрудников**|
|displayName|String|Отображаемое имя категории устройств.|
|описание|String|Необязательное описание категории устройств.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



