---
title: Тип ресурса Оффершифтрекуест
description: Представляет запрос, который предлагается переместить другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c507b8043c377dca0e13e079ff37e9499c00fbe1
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155119"
---
# <a name="offershiftrequest-resource-type"></a>Тип ресурса Оффершифтрекуест

Пространство имен: microsoft.graph

Представляет запрос, который предлагается переместить другому пользователю в команде.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List](../api/offershiftrequest-list.md) | Коллекция [оффершифтрекуест](offershiftrequest.md) | Чтение свойств и связей всех объектов **оффершифтрекуест** в команде. |
| [создание](../api/offershiftrequest-post.md); | [оффершифтрекуест](offershiftrequest.md) | Создайте экземпляр объекта **оффершифтрекуест** . |
| [получение](../api/offershiftrequest-get.md); | [оффершифтрекуест](offershiftrequest.md) | Чтение свойств и связей объекта **оффершифтрекуест** . |
|[Утвердить](../api/offershiftrequest-approve.md)|Нет|Утверждение **оффершифтрекуест**. |
|[Отклоня](../api/offershiftrequest-decline.md)|Нет|Отклонить **оффершифтрекуест**. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|реЦипиентактиондатетиме|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|реЦипиентактионмессаже|Строка| Настраиваемое сообщение, отправленное получателем запроса на смену предложением. |
|реЦипиентусерид|Строка| Идентификатор пользователя, который является получателем запроса на смену.|
|сендершифтид|Строка| Идентификатор пользователя отправителя запроса на смену.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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
