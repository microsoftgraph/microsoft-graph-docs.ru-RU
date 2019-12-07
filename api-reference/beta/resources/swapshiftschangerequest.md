---
title: Тип ресурса Свапшифтсчанжерекуест
description: Представляет тип запроса на смену для замены смены другим пользователем в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 80149a37dfb4d8d900066d11c315d125ff7fd670
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895845"
---
# <a name="swapshiftschangerequest-resource-type"></a>Тип ресурса Свапшифтсчанжерекуест

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на сдвиг для замены [смены](../resources/shift.md) другим пользователем в [команде](../resources/team.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/swapshiftschangerequest-get.md); | [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Чтение свойств и связей объекта **свапшифтсчанжерекуест** . |
| [обновление](../api/swapshiftschangerequest-update.md). | [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Обновление объекта **свапшифтсчанжерекуест** . |
| [удаление](../api/swapshiftschangerequest-delete.md); | Нет | Удаление объекта **свапшифтсчанжерекуест** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|реЦипиентшифтид|String|Идентификатор получателя запроса на замену. Это пользователь, с которым запрос перенаправляется.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": ""
}-->

```json
{
  "recipientShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftsChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
