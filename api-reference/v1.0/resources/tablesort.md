---
title: Тип ресурса TableSort
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 878dc98870c32f70ed9c4b36ff1252109c72d819b2a9912647ba80a54f0c6edd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222639"
---
# <a name="tablesort-resource-type"></a>Тип ресурса TableSort

Пространство имен: microsoft.graph

Управляет операциями сортировки для объектов Table.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableSort](../api/tablesort-get.md) | [WorkbookTableSort](tablesort.md) |Чтение свойств и связей объекта tableSort.|
|[Apply](../api/tablesort-apply.md)|Нет|Выполняет сортировку.|
|[Clear](../api/tablesort-clear.md)|Нет|Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.|
|[Reapply](../api/tablesort-reapply.md)|Нет|Повторно применяет текущие параметры сортировки к таблице.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fields|[Коллекция WorkbookSortField](sortfield.md)|Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.|
|matchCase|boolean|Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.|
|method|string|Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin` , `StrokeCount` . Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

