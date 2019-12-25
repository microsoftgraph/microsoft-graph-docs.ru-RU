---
title: Тип ресурса Среатассессментрекуест
description: Абстрактный тип ресурсов, используемый для представления элемента запроса оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8441fe14434733efda10c51d88e0750904ee1246
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867271"
---
# <a name="threatassessmentrequest-resource-type"></a>Тип ресурса Среатассессментрекуест

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип ресурсов, используемый для представления элемента запроса оценки угроз.

Запрос на оценку угроз может иметь один из следующих типов:

* Почта (ресурс[маилассессментрекуест](mailAssessmentRequest.md) )
* Файл электронной почты (ресурс[емаилфилеассессментрекуест](emailFileAssessmentRequest.md) )
* Файл (ресурс[филеассессментрекуест](fileAssessmentRequest.md) )
* URL-адрес (ресурс[урлассессментрекуест](urlAssessmentRequest.md) )

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Среатассессментрекуест](../api/informationprotection-list-threatassessmentrequests.md) | Коллекция [среатассессментрекуест](threatassessmentrequest.md) | Список всех запросов оценки угроз в клиенте. |
| [Создание Среатассессментрекуест](../api/informationprotection-post-threatassessmentrequests.md) | [среатассессментрекуест](threatassessmentrequest.md) | Создание запроса на оценку угроз путем отправки производного типа ресурса: [маилассессментрекуест](../resources/mailAssessmentRequest.md), [емаилфилеассессментрекуест](../resources/emailFileAssessmentRequest.md), [филеассессментрекуест](../resources/fileAssessmentRequest.md), [урлассессментрекуест](../resources/urlAssessmentRequest.md). |
| [Получение Среатассессментрекуест](../api/threatassessmentrequest-get.md) | [среатассессментрекуест](threatassessmentrequest.md) | Получение свойств и связей указанного ресурса **среатассессментрекуест** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
| :-------------|:------------|:------------|
|category|[среаткатегори](enums.md#threatcategory-values)|Категория угроз. Возможные значения: `spam`, `phishing`, `malware`.|
|contentType|[среатассессментконтенттипе](enums.md#threatassessmentcontenttype-values)|Тип контента для оценки угроз. Возможные значения: `mail`, `url`, `file`.|
|createdBy|[identitySet](identityset.md)|Создатель запроса на оценку угроз.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|експектедассессмент|[среатекспектедассессмент](enums.md#threatexpectedassessment-values)|Ожидаемая Оценка от отправителя. Возможные значения: `block`, `unblock`.|
|id|String|Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).|
|рекуестсаурце|[среатассессментрекуестсаурце](enums.md#threatassessmentrequestsource-values)|Источник запроса на оценку угроз. Возможные значения: `user`, `administrator`.|
|status|[среатассессментстатус](enums.md#threatassessmentstatus-values)|Состояние процесса оценки. Возможные значения: `pending`, `completed`.|

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|results|Коллекция [среатассессментресулт](threatassessmentresult.md)|Коллекция результатов оценки угроз. Только для чтения. По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "baseType": "",
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
