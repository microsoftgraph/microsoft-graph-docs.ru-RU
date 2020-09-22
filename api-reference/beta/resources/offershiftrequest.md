---
title: Тип ресурса Оффершифтрекуест
description: Представляет тип запроса на смену для предоставления смены другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e7c41461848fab45f3d291b175e6c584f98326fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021275"
---
# <a name="offershiftrequest-resource-type"></a>Тип ресурса Оффершифтрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на смену для предоставления смены другому пользователю в команде.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/offershiftrequest-post.md) | [оффершифтрекуест](offershiftrequest.md) | Создайте экземпляр объекта Оффершифтрекуест. |
| [получение](../api/offershiftrequest-get.md); | [оффершифтрекуест](offershiftrequest.md) | Чтение свойств и связей объекта Оффершифтрекуест. |
| [List](../api/offershiftrequest-list.md) | Коллекция [оффершифтрекуест](offershiftrequest.md) | Чтение свойств и связей всех объектов Оффершифтрекуест в команде. |
|[Утвердить](../api/offershiftrequest-approve.md)|Нет|Утверждение Оффершифтрекуест. |
|[Отклоня](../api/offershiftrequest-decline.md)|Нет|Отклонить Оффершифтрекуест. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|реЦипиентактиондатетиме|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|реЦипиентактионмессаже|String| Настраиваемое сообщение, отправленное получателем запроса на смену предложением. |
|реЦипиентусерид|String| Идентификатор пользователя, который является получателем запроса на смену.|
|сендершифтид|String| Идентификатор пользователя отправителя запроса на смену.|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest",
  "baseType": ""
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


