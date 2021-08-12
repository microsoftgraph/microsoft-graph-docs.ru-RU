---
title: тип ресурса externalItem
description: Элемент, добавленный к подключению microsoft Graph.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 74fbabcb749be4e388f3fe335b57857e76a73616885558700779ccd52c0c929e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212090"
---
# <a name="externalitem-resource-type"></a>тип ресурса externalItem

Пространство имен: microsoft.graph.externalConnectors

Элемент, добавленный к подключению microsoft [Graph.](externalconnectors-externalconnection.md) 

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Создание externalItem](../api/externalconnectors-externalitem-create.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Создайте [новый объект externalItem.](../resources/externalconnectors-externalitem.md)|
|[Get externalItem](../api/externalconnectors-externalitem-get.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Ознакомьтесь с свойствами и отношениями [объекта externalItem.](../resources/externalconnectors-externalitem.md)|
|[Обновление externalItem](../api/externalconnectors-externalitem-update.md)|[externalItem](../resources/externalconnectors-externalitem.md)|Обновление свойств объекта [externalItem.](../resources/externalconnectors-externalitem.md)|
|[Удаление externalItem](../api/externalconnectors-externalitem-delete.md)|Нет|Удаляет [объект externalItem.](../resources/externalconnectors-externalitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|acl|[коллекция microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)|Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. Обязательный элемент.|
|содержимое|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. Необязательно.|
|id|String|Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnectors-externalconnection.md) Должно быть альфа-числом и не более 128 символов. Обязательный элемент.|
|properties|[microsoft.graph.externalConnectors.properties](../resources/externalconnectors-properties.md)|Пакет свойств со свойствами элемента. Свойства должны соответствовать [схеме,](externalconnectors-schema.md) определенной для [externalConnection.](externalconnectors-externalconnection.md) Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "openType": false
}
-->
```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant"
    }
  ],
  "id": "String (identifier)",
  "properties": {
    "@odata.type": "microsoft.graph.externalConnectors.properties"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
  }
}
```

