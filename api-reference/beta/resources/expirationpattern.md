---
title: Тип ресурса expirationPattern
description: Шаблон срока действия в расписании запроса может быть включен в запрос на назначение пакета доступа и присутствует в назначении пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5a6ae13816c3b59905ee66ad5d2d18f6a71270bd
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777621"
---
# <a name="expirationpattern-resource-type"></a>Тип ресурса expirationPattern

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа. Этот запрос может включать расписание для того, когда пользователь хочет получить назначение.  Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.  Поле окончания срока действия [requestSchedule](requestschedule.md) указывает, когда должен истечь срок действия назначения пакета доступа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|duration|Длительность|Желаемая продолжительность доступа запрашиваемого. Если указан в запросе, endDateTime не должен присутствовать.|
|type|expirationPatternType|Желаемый тип шаблона истечения срока действия запросителем.|

### <a name="expirationpatterntype-values"></a>Значения expirationPatternType

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|notSpecified|0|Расписание окончания срока действия не задано.|
|noExpiration|1 |Запросителем не хотелось, чтобы срок действия доступа истекал.|
|afterDateTime|2 |Срок действия доступа истекает по истечении указанной даты и времени.|
|afterDuration|3 |Срок действия доступа истекает по истечении указанного срока, относительно предоставленного доступа.|

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


