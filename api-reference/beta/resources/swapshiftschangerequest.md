---
title: Тип ресурса Свапшифтсчанжерекуест
description: Представляет тип запроса на смену для замены смены другим пользователем в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d274c73cfcfb71bb86349dbe4cbbc7661e9e7a16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078152"
---
# <a name="swapshiftschangerequest-resource-type"></a>Тип ресурса Свапшифтсчанжерекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на сдвиг для замены [смены](../resources/shift.md) другим пользователем в [команде](../resources/team.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/swapshiftschangerequest-list.md) | Коллекция [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Перечисление свойств и связей объектов **свапшифтсчанжерекуест** в команде. |
| [Создание](../api/swapshiftschangerequest-post.md) | [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Создайте экземпляр объекта свапшифтсчанжерекуест. |
| [получение](../api/swapshiftschangerequest-get.md); | [свапшифтсчанжерекуест](swapshiftschangerequest.md) | Чтение свойств и связей объекта **свапшифтсчанжерекуест** . |
|[Утвердить](../api/swapshiftschangerequest-approve.md)|Нет|Утверждение **свапшифтсчанжерекуест**. |
|[Отклоня](../api/swapshiftschangerequest-decline.md)|Нет|Отклонить **свапшифтсчанжерекуест**.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|реЦипиентшифтид|String|Идентификатор смены для пользователя получателя, с которым отправляется запрос на переключение.|

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


