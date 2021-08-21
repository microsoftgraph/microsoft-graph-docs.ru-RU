---
title: тип ресурса requestSchedule
description: Расписание запросов может быть включено в запрос назначения пакета доступа и присутствует в назначении пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8336366a1e6c63b6f76b293b6445f5583a7fd32f
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454033"
---
# <a name="requestschedule-resource-type"></a>тип ресурса requestSchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа. Этот запрос может включать расписание, когда пользователь хотел бы получить назначение.  Назначение пакета доступа, которое является результатом такого запроса, также имеет расписание.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|истечение срока действия|[expirationPattern](expirationpattern.md)|По истечении срока действия доступа.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Для повторного доступа. Не используется в настоящее время.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule"
}-->

```json
{
    "startDateTime": "2020-08-11T23:06:53.307Z",
    "expiration": {
      "@odata.type": "microsoft.graph.expirationPattern"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


