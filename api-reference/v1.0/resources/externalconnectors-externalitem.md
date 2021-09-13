---
title: тип ресурса externalItem
description: Элемент, добавленный к подключению microsoft Graph.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e50a494898faa377123e96238dee0bf1109d798d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123449"
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
|acl|[коллекция microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)|Массив записей управления доступом. Каждая запись указывает доступ, предоставленный пользователю или группе. Обязательное.|
|содержимое|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|Простое текстовое представление содержимого элемента. Текст в этом свойстве индексироваться с полным текстом. Необязательное.|
|id|Строка|Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnectors-externalconnection.md) Должно быть альфа-числом и не более 128 символов. Обязательный.|
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

