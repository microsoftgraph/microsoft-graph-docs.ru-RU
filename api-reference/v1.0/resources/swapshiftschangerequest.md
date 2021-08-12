---
title: тип ресурса swapShiftsChangeRequest
description: Представляет тип запроса на смену для замены смены с другим пользователем в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8e534e40b9ad273c89808409db0078c4e0a62031684c9748336afc8823a8a797
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222653"
---
# <a name="swapshiftschangerequest-resource-type"></a>тип ресурса swapShiftsChangeRequest

Пространство имен: microsoft.graph

Представляет тип запроса на смену для замены [смены](../resources/shift.md) с другим пользователем [в команде.](../resources/team.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/swapshiftschangerequest-list.md) | Коллекция [swapShiftsChangeRequest](swapshiftschangerequest.md) | Список свойств и связей **объектов swapShiftsChangeRequest** в группе. |
| [Создание](../api/swapshiftschangerequest-post.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Создайте экземпляр объекта **swapShiftsChangeRequest.** |
| [Получение](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Ознакомьтесь с свойствами и отношениями объекта **swapShiftsChangeRequest.** |
|[Утвердить](../api/swapshiftschangerequest-approve.md)|Нет|Утверждение **swapShiftsChangeRequest.** |
|[Отклонение](../api/swapshiftschangerequest-decline.md)|Нет|Отклонение **swapShiftsChangeRequest**.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|recipientShiftId|String|ShiftId для пользователя получателя, с которым запрашивается замена.|

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

