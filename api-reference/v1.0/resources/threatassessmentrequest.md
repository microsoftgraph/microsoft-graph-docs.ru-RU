---
title: тип ресурса threatAssessmentRequest
description: Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угрозы.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: aeb3733ed3c93896d701851a928e216a2b9c7c7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952503"
---
# <a name="threatassessmentrequest-resource-type"></a>тип ресурса threatAssessmentRequest

Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угрозы.

Запрос на оценку угроз может быть одним из следующих типов:

* Почта[(ресурс mailAssessmentRequest)](mailAssessmentRequest.md)
* Файл электронной почты[(ресурс emailFileAssessmentRequest)](emailFileAssessmentRequest.md)
* Файл[(ресурс fileAssessmentRequest)](fileAssessmentRequest.md)
* [URL-адрес (ресурс urlAssessmentRequest)](urlAssessmentRequest.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление объектов threatAssessmentRequest](../api/informationprotection-list-threatassessmentrequests.md) | [коллекция threatAssessmentRequest](threatassessmentrequest.md) | Список всех запросов на оценку угроз в клиенте. |
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [threatAssessmentRequest](threatassessmentrequest.md) | Создайте новый запрос на оценку угрозы, разместив производный тип ресурса: [mailAssessmentRequest,](../resources/mailAssessmentRequest.md) [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md). |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [threatAssessmentRequest](threatassessmentrequest.md) | Извлечение свойств и связей указанного ресурса **threatAssessmentRequest.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
| :-------------|:------------|:------------|
|category|[threatCategory](enums.md#threatcategory-values)|Категория угроз. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|Тип оценки угрозы контента. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|Ожидаемая оценка от подавщика. Возможные значения: `block`, `unblock`.|
|id|String|Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|Источник запроса на оценку угрозы. Возможные значения: `user`, `administrator`.|
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
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
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
  "description": "threatAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

