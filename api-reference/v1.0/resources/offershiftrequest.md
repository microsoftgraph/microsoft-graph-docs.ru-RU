---
title: Тип ресурса offerShiftRequest
description: Представляет запрос на предложение смены другому пользователю в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d17ca029d29b2b8f27a923adf4ef019ac002f404
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158725"
---
# <a name="offershiftrequest-resource-type"></a>Тип ресурса offerShiftRequest

Пространство имен: microsoft.graph

Представляет запрос на предложение смены другому пользователю в команде.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/offershiftrequest-list.md) | Коллекция [offerShiftRequest](offershiftrequest.md) | Чтение свойств и связей всех объектов **offerShiftRequest** в команде. |
| [Создание](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Создание экземпляра объекта **offerShiftRequest.** |
| [Получение](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | Чтение свойств и связей объекта **offerShiftRequest.** |
|[Утвердить](../api/offershiftrequest-approve.md)|Нет|Утверждение **offerShiftRequest.** |
|[Отклонение](../api/offershiftrequest-decline.md)|Нет|Отклонение **предложенияShiftRequest.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|recipientActionMessage|String| Настраиваемые сообщения, отправленные получателем запроса на смену предложения. |
|recipientUserId|String| ИД пользователя получателя запроса на смену предложения.|
|senderShiftId|String| ИД отправитель запроса на смену предложения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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

