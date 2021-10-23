---
title: тип ресурса urlAssessmentRequest
description: Используется для создания и получения оценки угрозы URL-адреса.
ms.localizationpriority: medium
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: fa491683f436483a93702e724400f04df48e3d09
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561621"
---
# <a name="urlassessmentrequest-resource-type"></a>тип ресурса urlAssessmentRequest

Используется для создания и получения оценки угроз URL-адреса, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание объекта threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [urlAssessmentRequest](urlAssessmentRequest.md) | Создайте новый запрос на оценку URL-адресов, разместив **объект urlAssessmentRequest.** |
| [Получение объекта threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [urlAssessmentRequest](urlassessmentrequest.md) | Ознакомьтесь с свойствами и отношениями объекта **urlAssessmentRequest.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|url|String|Строка URL-адреса.|
|category|[threatCategory](enums.md#threatcategory-values)|Категория угроз. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|Тип контента оценки угрозы. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|Ожидаемая оценка от ubmitter. Возможные значения: `block`, `unblock`.|
|id|Строка|Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|Источник запроса на оценку угрозы. Возможные значения: `administrator` .|
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

