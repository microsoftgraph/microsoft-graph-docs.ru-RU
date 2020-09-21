---
title: Тип ресурса Емаилфилеассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для файла электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 848ba0e1d7bfae16270f12d5acb153c083ca1d06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989572"
---
# <a name="emailfileassessmentrequest-resource-type"></a>Тип ресурса Емаилфилеассессментрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для создания и извлечения средства оценки угроз для файла электронной почты, производного от [среатассессментрекуест](threatAssessmentRequest.md).

Файл электронной почты может иметь тип EML.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [emailFileAssessmentRequest](emailFileAssessmentRequest.md) | Создание нового запроса на оценку файла электронной почты путем отправки объекта **емаилфилеассессментрекуест** . |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [emailFileAssessmentRequest](emailfileassessmentrequest.md) | Чтение свойств и связей объекта **емаилфилеассессментрекуест** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|контентдата|String|Содержимое файла электронной почты в кодировке Base64. EML. Не удается вернуть содержимое файла, так как оно не хранится.|
|дестинатионраутингреасон|[маилдестинатионраутингреасон](enums.md#maildestinationroutingreason-values)|Причина, по которой почта перенаправляется в назначение. Возможные значения: `none` , `mailFlowRule` ,,,,, `safeSender` `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` ,,, `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` , `autoPurgeToJunk` , `autoPurgeToDeleted` , `outbound` , `notJunk` , `junk` .|
|реЦипиентемаил|String|Получатель почты, политики которого используются для оценки почты.|
|category|[среаткатегори](enums.md#threatcategory-values)|Категория угроз. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[среатассессментконтенттипе](enums.md#threatassessmentcontenttype-values)|Тип контента для оценки угроз. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|експектедассессмент|[среатекспектедассессмент](enums.md#threatexpectedassessment-values)|Ожидаемая Оценка от отправителя. Возможные значения: `block`, `unblock`.|
|id|String|Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).|
|рекуестсаурце|[среатассессментрекуестсаурце](enums.md#threatassessmentrequestsource-values)|Источник запроса на оценку угроз. Возможные значения: `user`, `administrator`.|
|status|[среатассессментстатус](enums.md#threatassessmentstatus-values)|Состояние процесса оценки. Возможные значения: `pending`, `completed`.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|results|Коллекция [среатассессментресулт](threatassessmentresult.md)|Коллекция результатов оценки угроз. Только для чтения. По умолчанию объект a не `GET /threatAssessmentRequests/{id}` возвращает это свойство, пока не применено `$expand` к нему.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "baseType": "",
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


