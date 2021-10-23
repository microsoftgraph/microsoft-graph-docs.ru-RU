---
title: тип ресурса mailAssessmentRequest
description: Используется для создания и получения оценки угроз почты.
ms.localizationpriority: medium
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 83a2fb0fa5a309d880830a11f9806a729383b1d7
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560830"
---
# <a name="mailassessmentrequest-resource-type"></a>тип ресурса mailAssessmentRequest

Используется для создания и получения оценки угроз почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)

При создании запроса на оценку угрозы почты почта должна быть получена пользователем, указанным в `recipientEmail` . [Делегированная](/graph/permissions-reference#mail-permissions) почта разрешений (Mail.Read или Mail.Read.Shared) переквалифицироваться для доступа к почте, полученной пользователем или общим кем-то еще.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [mailAssessmentRequest](mailAssessmentRequest.md) | Создайте новый запрос на оценку почты, разместив объект **mailAssessmentRequest.** |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [mailAssessmentRequest](mailassessmentrequest.md) | Ознакомьтесь с свойствами и отношениями объекта **mailAssessmentRequest.** |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|destinationRoutingReason|[mailDestinationRoutingReason](enums.md#maildestinationroutingreason-values)|Причина направления почты в пункт назначения. Возможные значения: `none` `mailFlowRule` , , , , , `safeSender` , `blockedSender` , `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` , `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` , .|
|messageUri|Строка|URI ресурса почтового сообщения для оценки.|
|recipientEmail|Строка|Получатель почты, политики которого используются для оценки почты.|
|category|[threatCategory](enums.md#threatcategory-values)|Категория угроз. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|Тип оценки угрозы контента. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|Ожидаемая оценка от подавщика. Возможные значения: `block`, `unblock`.|
|id|Строка|Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|Источник запроса на оценку угроз. Возможные значения: `administrator` .|
|status|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|Состояние процесса оценки. Возможные значения: `pending`, `completed`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|results|[коллекция threatAssessmentResult](threatassessmentresult.md)|Коллекция результатов оценки угроз. Только для чтения. По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "destinationRoutingReason": "String",
  "messageUri": "String",
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
  "description": "mailAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

