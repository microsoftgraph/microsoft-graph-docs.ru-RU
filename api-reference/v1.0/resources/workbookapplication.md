---
title: Тип ресурса Воркбукаппликатион
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a4f7d2cd6887598ac0a60522dc5bee1101dff9c9
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023250"
---
# <a name="workbookapplication-resource-type"></a>Тип ресурса Воркбукаппликатион

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

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

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
