---
title: тип ресурса workbookApplication
description: Представляет приложение Excel, которое управляет книгой.
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3663ba238ac0ab7a2346786d775b16326ddf0193
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139473"
---
# <a name="workbookapplication-resource-type"></a>тип ресурса workbookApplication

Пространство имен: microsoft.graph

Представляет приложение Excel, которое управляет книгой.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get workbookApplication](../api/workbookapplication-get.md) | [workbookApplication](workbookapplication.md) |Чтение свойств и связей объекта workbookApplication.|
|[Calculate](../api/workbookapplication-calculate.md)|Нет|Пересчитывает данные во всех открытых в текущий момент книгах Excel.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|calculationMode|string|Возвращает режим вычисления, который используется в книге. Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.|

## <a name="relationships"></a>Отношения
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

