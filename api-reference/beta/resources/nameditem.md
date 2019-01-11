---
title: Тип ресурса NamedItem
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
ms.openlocfilehash: 5dd093976b2c09ae93c608144c8d6c2b7d7161c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815374"
---
# <a name="nameditem-resource-type"></a>Тип ресурса NamedItem

Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[NamedItem](nameditem.md)|Добавляет новое имя в определенную коллекцию.|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[NamedItem](nameditem.md)|Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.|
|[Get NamedItem](../api/nameditem-get.md) | [NamedItem](nameditem.md) |Чтение свойств и связей объекта namedItem.|
|[Обновление](../api/nameditem-update.md) | [NamedItem](nameditem.md)   |Обновление объекта NamedItem. |
|[Range](../api/nameditem-range.md)|[Range](range.md)|Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.|
|[Список](../api/nameditem-list.md) | Коллекция объектов [NamedItem](nameditem.md) |Получение коллекции объектов namedItem. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|строка|Имя объекта. Только для чтения.|
|comment|строка|Представляет примечание, связанное с этим именем.|
|scope|string|Указывает, относится ли имя к книге или определенному листу. Только для чтения.|
|type|строка|Указывает тип ссылки, связанный с именем. Возможные значения: `String`, `Integer`, `Double`, `Boolean`, `Range`. Только для чтения.|
|value|строка|Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4.75 и т. д. Только для чтения.|
|visible|boolean|Определяет, является ли объект видимым.|

## <a name="relationships"></a>Связи
| Связь     | Тип   |Описание|
|:---------------|:--------|:----------|
|worksheet|[worksheet](worksheet.md)|Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
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
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
