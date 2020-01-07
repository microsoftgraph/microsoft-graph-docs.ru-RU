---
title: Тип ресурса Оффершифтрекуест
description: Представляет тип запроса на смену для предоставления смены другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2b12dd9df816ad7fecbf6c520f0fff579087428
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952295"
---
# <a name="offershiftrequest-resource-type"></a>Тип ресурса Оффершифтрекуест

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
