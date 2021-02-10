---
title: Тип ресурса urlAssessmentRequest
description: Используется для создания и извлечения оценки угрозы URL-адреса.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7046d322a351834a6271d4349c3964607312af85
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156653"
---
# <a name="urlassessmentrequest-resource-type"></a>Тип ресурса urlAssessmentRequest

Используется для создания и извлечения оценки угрозы URL-адреса, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [urlAssessmentRequest](urlAssessmentRequest.md) | Создайте новый запрос на оценку URL-адреса, опубликовав объект **urlAssessmentRequest.** |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [urlAssessmentRequest](urlassessmentrequest.md) | Чтение свойств и связей объекта **urlAssessmentRequest.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|url|String|Строка URL-адреса.|
|category|[threatCategory](enums.md#threatcategory-values)|Категория угрозы. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|Тип контента оценки угроз. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|Ожидаемая оценка от ubmitter. Возможные значения: `block`, `unblock`.|
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
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
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

