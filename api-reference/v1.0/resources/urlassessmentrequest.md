---
title: Тип ресурса Урлассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для URL-адресов.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6723e2c4ce080555bf9932bb5c75012110d7b754
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090608"
---
# <a name="urlassessmentrequest-resource-type"></a>Тип ресурса Урлассессментрекуест

Используется для создания и извлечения средства оценки угроз URL-адресов, производного от [среатассессментрекуест](threatAssessmentRequest.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [urlAssessmentRequest](urlAssessmentRequest.md) | Создание нового запроса на оценку URL-адреса путем отправки объекта **урлассессментрекуест** . |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [urlAssessmentRequest](urlassessmentrequest.md) | Чтение свойств и связей объекта **урлассессментрекуест** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|url|String|Строка URL-адреса.|
|category|[среаткатегори](enums.md#threatcategory-values)|Категория угроз. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[среатассессментконтенттипе](enums.md#threatassessmentcontenttype-values)|Тип контента для оценки угроз. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|експектедассессмент|[среатекспектедассессмент](enums.md#threatexpectedassessment-values)|Ожидаемая Оценка из убмиттер. Возможные значения: `block`, `unblock`.|
|id|Строка|Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).|
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
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "url": "String",
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
  "description": "urlAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

