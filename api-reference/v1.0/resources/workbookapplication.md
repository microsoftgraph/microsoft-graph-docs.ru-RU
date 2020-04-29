---
title: Тип ресурса Воркбукаппликатион
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d4b2833910d22696ee95ed707469f6da2068453c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446725"
---
# <a name="workbookapplication-resource-type"></a>Тип ресурса Воркбукаппликатион

Пространство имен: microsoft.graph

Представляет приложение Excel, которое управляет книгой.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукаппликатион](../api/workbookapplication-get.md) | [воркбукаппликатион](workbookapplication.md) |Чтение свойств и связей объекта Воркбукаппликатион.|
|[Calculate](../api/workbookapplication-calculate.md)|Нет|Пересчитывает данные во всех открытых в текущий момент книгах Excel.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|калкулатионмоде|string|Возвращает режим вычисления, который используется в книге. Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
