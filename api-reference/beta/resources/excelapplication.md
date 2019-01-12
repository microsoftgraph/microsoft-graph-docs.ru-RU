---
title: Тип ресурса приложения
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 250141ff6c6da3a81a1b3492908bc2e04b5a0605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921978"
---
# <a name="application-resource-type"></a>Тип ресурса приложения

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет приложение Excel, которое управляет книгой.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение приложения](../api/excelapplication-get.md) | [Application](application.md) |Чтение свойства и связи объекта приложения.|
|[Calculate](../api/excelapplication-calculate.md)|Нет|Пересчитывает данные во всех открытых в текущий момент книгах Excel.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|calculationMode|строка|Возвращает режим вычисления, используемый в книге. Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`. Только для чтения.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
