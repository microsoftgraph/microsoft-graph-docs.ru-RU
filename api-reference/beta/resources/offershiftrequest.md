---
title: тип ресурса offerShiftRequest
description: Представляет тип запроса на смену, чтобы предложить переход другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f80e8578422aa00d6af1d2df22a0dfb7472c8c8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721483"
---
# <a name="offershiftrequest-resource-type"></a>тип ресурса offerShiftRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на смену, чтобы предложить переход другому пользователю в команде.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Создание экземпляра объекта offerShiftRequest. |
| [получение](../api/offershiftrequest-get.md); | [offerShiftRequest](offershiftrequest.md) | Чтение свойств и связей объекта offerShiftRequest. |
| [List](../api/offershiftrequest-list.md) | Коллекция [offerShiftRequest](offershiftrequest.md) | Чтение свойств и связей всех объектов offerShiftRequest в команде. |
|[Утвердить](../api/offershiftrequest-approve.md)|Нет|Утверждение предложенияShiftRequest. |
|[Отклонение](../api/offershiftrequest-decline.md)|Нет|Отклонение предложенияShiftRequest. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|recipientActionMessage|String| Настраиваемые сообщения, отправленные получателем запроса на перенос предложения. |
|recipientUserId|String| Пользовательский id получателя запроса на перенос предложения.|
|senderShiftId|String| Пользовательский id отправитель запроса на перенос предложения.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest"
}-->

```json
{
  "recipientActionDateTime": "String (timestamp)",
  "recipientActionMessage": "String",
  "recipientUserId": "String",
  "senderShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "offerShiftRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


