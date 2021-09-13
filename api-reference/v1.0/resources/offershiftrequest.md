---
title: тип ресурса offerShiftRequest
description: Представляет запрос на предложение о переходе другому пользователю в команде.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10e96e9260f1027db87884bc8b01582fb7743a75
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094228"
---
# <a name="offershiftrequest-resource-type"></a>тип ресурса offerShiftRequest

Пространство имен: microsoft.graph

Представляет запрос на предложение о переходе другому пользователю в команде.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление](../api/offershiftrequest-list.md) | Коллекция [offerShiftRequest](offershiftrequest.md) | Ознакомьтесь с свойствами и отношениями всех **объектов offerShiftRequest** в команде. |
| [Создание](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | Создание экземпляра объекта **offerShiftRequest.** |
| [получение](../api/offershiftrequest-get.md); | [offerShiftRequest](offershiftrequest.md) | Ознакомьтесь с свойствами и отношениями объекта **offerShiftRequest.** |
|[Утвердить](../api/offershiftrequest-approve.md)|Нет|Утверждение **предложенияShiftRequest**. |
|[Отклонение](../api/offershiftrequest-decline.md)|Нет|Отклонение **предложенияShiftRequest**. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|recipientActionMessage|String| Настраиваемые сообщения, отправленные получателем запроса на перенос предложения. |
|recipientUserId|Строка| Пользовательский ID получателя запроса на перенос предложения.|
|senderShiftId|Строка| Пользовательский ID отправитель запроса на перенос предложения.|

## <a name="relationships"></a>Отношения

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

