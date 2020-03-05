---
title: Тип ресурса Маилассессментрекуест
description: Используется для создания и получения оценки угроз электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97cf59e5342fe72a4acdf582c7f20f571e4d0156
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522885"
---
# <a name="mailassessmentrequest-resource-type"></a>Тип ресурса Маилассессментрекуест

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для создания и получения оценки угроз электронной почты, производных от [среатассессментрекуест](threatAssessmentRequest.md).

Когда вы создаете запрос оценки угроз для электронной почты, сообщение должно быть получено пользователем, указанным `recipientEmail`в. Делегированные [разрешения на почту](/graph/permissions-reference#mail-permissions) (mail. Read или mail. Read. shared) — рекуриед для доступа к почте, полученной пользователем или предоставленных другим пользователем.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [mailAssessmentRequest](mailAssessmentRequest.md) | Создание запроса на оценку почты путем отправки объекта **маилассессментрекуест** . |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [mailAssessmentRequest](mailassessmentrequest.md) | Чтение свойств и связей объекта **маилассессментрекуест** . |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|дестинатионраутингреасон|[маилдестинатионраутингреасон](enums.md#maildestinationroutingreason-values)|Причина, по которой почта перенаправляется в назначение. Возможные значения: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`,. `junk`|
|мессажеури|String|URI ресурса почтового сообщения для оценки.|
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
|results|Коллекция [среатассессментресулт](threatassessmentresult.md)|Коллекция результатов оценки угроз. Только для чтения. По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "",
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
