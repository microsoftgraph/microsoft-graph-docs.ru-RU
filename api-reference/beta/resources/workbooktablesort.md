---
title: Тип ресурса Воркбуктаблесорт
description: Управляет операциями сортировки для объектов Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ea0332f1ad00029cf511f2bc55aca80836e5ef2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007034"
---
# <a name="workbooktablesort-resource-type"></a>Тип ресурса Воркбуктаблесорт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управляет операциями сортировки для объектов Table.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableSort](../api/tablesort-get.md) | [Воркбуктаблесорт](workbooktablesort.md) |Чтение свойств и связей объекта tableSort.|
|[Apply](../api/tablesort-apply.md)|Нет|Выполняет сортировку.|
|[Clear](../api/tablesort-clear.md)|Нет|Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.|
|[Reapply](../api/tablesort-reapply.md)|Нет|Повторно применяет текущие параметры сортировки к таблице.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|matchCase|boolean|Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.|
|method|string|Указывает метод сортировки китайских символов, который использовался при последней сортировке таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|fields|[Воркбуксортфиелд](workbooksortfield.md)|Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
 
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "id": "string",
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
