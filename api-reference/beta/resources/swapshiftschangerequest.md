---
title: Тип ресурса swapShiftsChangeRequest
description: Представляет тип запроса на смену для замены смены другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 813deba1207cc2eafee71dcdb951ba31b5526ba3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154791"
---
# <a name="swapshiftschangerequest-resource-type"></a>Тип ресурса swapShiftsChangeRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на смену для замены смены [другому](../resources/shift.md) пользователю в [команде.](../resources/team.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/swapshiftschangerequest-list.md) | Коллекция [swapShiftsChangeRequest](swapshiftschangerequest.md) | Список свойств и связей объектов **swapShiftsChangeRequest** в команде. |
| [Создание](../api/swapshiftschangerequest-post.md) | [swapshiftschangerequest](swapshiftschangerequest.md) | Создание экземпляра объекта swapshiftschangerequest. |
| [Получение](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Чтение свойств и связей объекта **swapShiftsChangeRequest.** |
|[Утвердить](../api/swapshiftschangerequest-approve.md)|Нет|Утверждение **swapShiftsChangeRequest.** |
|[Отклонение](../api/swapshiftschangerequest-decline.md)|Нет|Отклонение **swapShiftsChangeRequest.**|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|recipientShiftId|String|Shift ID для пользователя получателя, с которым требуется заменить запрос.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
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


