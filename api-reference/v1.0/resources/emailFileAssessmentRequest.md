---
title: Тип ресурса emailFileAssessmentRequest
description: Используется для создания и извлечения оценки угрозы файла электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 43c7f1cbfe3087a092ca498969ce6df5250a7af8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153461"
---
# <a name="emailfileassessmentrequest-resource-type"></a>Тип ресурса emailFileAssessmentRequest

Используется для создания и извлечения оценки угрозы файла электронной почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)

Файл электронной почты может быть EML-файлом.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [emailFileAssessmentRequest](emailFileAssessmentRequest.md) | Создайте новый запрос на оценку файлов электронной почты, опубликовав объект **emailFileAssessmentRequest.** |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [emailFileAssessmentRequest](emailfileassessmentrequest.md) | Чтение свойств и связей объекта **emailFileAssessmentRequest.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|contentData|String|Содержимое eml-файла электронной почты в коде Base64. Содержимое файла не может получить обратно, так как оно не хранится.|
|destinationRoutingReason|[mailDestinationRoutingReason](enums.md#maildestinationroutingreason-values)|Причина перенаправления почты в место назначения. Возможные значения: `none` , , , , , , , `mailFlowRule` , , `safeSender` , `blockedSender` `advancedSpamFiltering` , `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` . `junk`|
|recipientEmail|String|Получатель почты, политики которого используются для оценки почты.|
|category|[threatCategory](enums.md#threatcategory-values)|Категория угрозы. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|Тип контента для оценки угроз. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|Ожидаемая оценка от подавщика. Возможные значения: `block`, `unblock`.|
|id|String|Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|Источник запроса на оценку угроз. Возможные значения: `user`, `administrator`.|
|status|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|Состояние процесса оценки. Возможные значения: `pending`, `completed`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|results|[Коллекция threatAssessmentResult](threatassessmentresult.md)|Коллекция результатов оценки угроз. Только для чтения. По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "destinationRoutingReason": "String",
  "recipientEmail": "String",
  "category": "String",
  "contentType": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "expectedAssessment": "String",
  "id": "String (identifier)",
  "requestSource": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailFileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

