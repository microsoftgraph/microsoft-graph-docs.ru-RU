---
title: Тип ресурса Свапшифтсчанжерекуест
description: Представляет тип запроса на смену для замены смены другим пользователем в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a172737f40572b29358ecdc6fba804db2a8b80e5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951960"
---
# <a name="swapshiftschangerequest-resource-type"></a>Тип ресурса Свапшифтсчанжерекуест

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на сдвиг для замены [смены](../resources/shift.md) другим пользователем в [команде](../resources/team.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | Коллекция [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Перечисление свойств и связей объектов **свапшифтсчанжерекуест** в команде. |
| [создание](../api/swapshiftschangerequest-post.md); | [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Создайте экземпляр объекта свапшифтсчанжерекуест. |
| [получение](../api/swapshiftschangerequest-get.md); | [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Чтение свойств и связей объекта **свапшифтсчанжерекуест** . |
|[Утвердить](../api/swapshiftschangerequest-approve.md)|Нет|Утверждение свапшифтсчанжерекуест. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|реЦипиентшифтид|String|Идентификатор получателя запроса на замену. Это пользователь, с которым запрос перенаправляется.|

## <a name="relationships"></a>Отношения

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
