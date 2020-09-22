---
title: Тип ресурса Воркбукнамедитем
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 9cfef2da8204723d6f6aac2bd4006edc3a62789e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070439"
---
# <a name="workbooknameditem-resource-type"></a>Тип ресурса Воркбукнамедитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[воркбукнамедитем](workbooknameditem.md)|Добавляет новое имя в определенную коллекцию.|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[воркбукнамедитем](workbooknameditem.md)|Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.|
|[Get NamedItem](../api/nameditem-get.md) | [воркбукнамедитем](workbooknameditem.md) |Чтение свойств и связей объекта namedItem.|
|[Обновление](../api/nameditem-update.md) | [воркбукнамедитем](workbooknameditem.md)   |Обновление объекта NamedItem. |
|[Range](../api/nameditem-range.md)|[workbookRange](workbookrange.md)|Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.|
|[Список](../api/nameditem-list.md) | Коллекция [workbookNamedItem](workbooknameditem.md) |Получение коллекции объектов namedItem. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string|Имя объекта. Только для чтения.|
|comment|string|Представляет примечание, связанное с этим именем.|
|scope|string|Указывает, относится ли имя к книге или определенному листу. Только для чтения.|
|type|string|Указывает тип ссылки, связанный с именем. Возможные значения: `String`, `Integer`, `Double`, `Boolean`, `Range`. Только для чтения.|
|value|строка|Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4.75 и т. д. Только для чтения.|
|visible|boolean|Определяет, является ли объект видимым.|

## <a name="relationships"></a>Отношения
| Связь     | Тип   |Описание|
|:---------------|:--------|:----------|
|worksheet|[воркбукворкшит](workbookworksheet.md)|Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
  "visible": true

}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


