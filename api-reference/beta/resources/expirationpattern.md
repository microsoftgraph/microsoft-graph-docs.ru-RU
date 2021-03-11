---
title: тип ресурса expirationPattern
description: Шаблон истечения срока действия в расписании запросов может быть включен в запрос на назначение пакета доступа и присутствует в назначении пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b6587d8ba410ba0240c0fd75b7c8ec37105061d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721301"
---
# <a name="expirationpattern-resource-type"></a>тип ресурса expirationPattern

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа. Этот запрос может включать расписание, когда пользователь хотел бы получить назначение.  Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.  Поле истечения срока действия [запросаSchedule](requestschedule.md) указывает, когда должно истекть назначение пакета доступа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|duration|Duration|Желаемая продолжительность доступа запрашиваемого запроса. Если указан в запросе, endDateTime не должен присутствовать.|
|type|expirationPatternType|Желаемый тип шаблона истечения срока действия запрашиваемого запроса.|

### <a name="expirationpatterntype-values"></a>значения expirationPatternType

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|notSpecified|0|Срок действия не указан.|
|noExpiration|1|Запросчик не хотел, чтобы срок действия доступа истек.|
|afterDateTime|2 |Срок доступа истекает после указанной даты и времени.|
|afterDuration|3 |Срок доступа истекает после указанной продолжительности, относительно предоставленного доступа.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern"
}-->

```json
{
    "endDateTime": "2020-09-10T23:06:53.307Z",
    "type": "afterDateTime"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expirationPattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


