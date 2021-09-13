---
title: тип ресурса swapShiftsChangeRequest
description: Представляет тип запроса на смену для замены смены с другим пользователем в команде.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 396e4d9dd08044bd726b9e6f85ed808065ec37da
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134454"
---
# <a name="swapshiftschangerequest-resource-type"></a>тип ресурса swapShiftsChangeRequest

Пространство имен: microsoft.graph

Представляет тип запроса на смену для замены [смены](../resources/shift.md) с другим пользователем [в команде.](../resources/team.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление](../api/swapshiftschangerequest-list.md) | Коллекция [swapShiftsChangeRequest](swapshiftschangerequest.md) | Список свойств и связей **объектов swapShiftsChangeRequest** в группе. |
| [Создание](../api/swapshiftschangerequest-post.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Создайте экземпляр объекта **swapShiftsChangeRequest.** |
| [получение](../api/swapshiftschangerequest-get.md); | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Ознакомьтесь с свойствами и отношениями объекта **swapShiftsChangeRequest.** |
|[Утвердить](../api/swapshiftschangerequest-approve.md)|Нет|Утверждение **swapShiftsChangeRequest.** |
|[Отклонение](../api/swapshiftschangerequest-decline.md)|Нет|Отклонение **swapShiftsChangeRequest**.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|recipientShiftId|Строка|ShiftId для пользователя получателя, с которым запрашивается замена.|

## <a name="relationships"></a>Отношения

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

