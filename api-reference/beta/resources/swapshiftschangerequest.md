---
title: Тип ресурса Свапшифтсчанжерекуест
description: Представляет тип запроса на смену для замены смены другим пользователем в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0fbc0f392a6efa1b0a0ba5f1568451a6fe7d1cf
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219757"
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
|[Утвердить](../api/swapshiftschangerequest-approve.md)|Нет|Утверждение **свапшифтсчанжерекуест**. |
|[Отклоня](../api/swapshiftschangerequest-decline.md)|Нет|Отклонить **свапшифтсчанжерекуест**.|

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
