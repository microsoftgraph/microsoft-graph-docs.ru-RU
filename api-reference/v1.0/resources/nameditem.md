---
title: Тип ресурса NamedItem
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2c92202e5e9d1671d72acecaec50203d01c5a90eb30436df0d70cb5518763258
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237616"
---
# <a name="nameditem-resource-type"></a>Тип ресурса NamedItem

Пространство имен: microsoft.graph

Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[WorkbookNamedItem](nameditem.md)|Добавляет новое имя в определенную коллекцию.|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[WorkbookNamedItem](nameditem.md)|Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.|
|[Get NamedItem](../api/nameditem-get.md) | [WorkbookNamedItem](nameditem.md) |Чтение свойств и связей объекта namedItem.|
|[Обновление](../api/nameditem-update.md) | [WorkbookNamedItem](nameditem.md)   |Обновление объекта NamedItem. |
|[Range](../api/nameditem-range.md)|[Range](range.md)|Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.|
|[Список](../api/nameditem-list.md) | Коллекция [WorkbookNamedItem](nameditem.md) |Получение коллекции объектов namedItem. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string|Имя объекта. Только для чтения.|
|comment|string|Представляет примечание, связанное с этим именем.|
|scope|string|Указывает, относится ли имя к книге или определенному листу. Только для чтения.|
|type|string|Указывает тип ссылки, связанный с именем. Допустимые значения: `String`, `Integer`, `Double`, `Boolean`, `Range`. Только для чтения.|
|value|Json|Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4,75 и т. д. Только для чтения.|
|visible|boolean|Определяет, является ли объект видимым.|

## <a name="relationships"></a>Связи
| Связь     | Тип   |Описание|
|:---------------|:--------|:----------|
|worksheet|[WorkbookWorksheet](worksheet.md)|Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true

}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

