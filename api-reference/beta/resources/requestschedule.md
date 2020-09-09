---
title: Тип ресурса Рекуестсчедуле
description: Расписание запроса можно включить в запрос на назначение пакета Access и оно присутствует в назначении пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d5a80db31b0499648c5f297b613a198ddec6d25d
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413397"
---
# <a name="requestschedule-resource-type"></a>Тип ресурса Рекуестсчедуле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access. Этот запрос может включать расписание, когда пользователь хочет назначить назначение.  Назначение пакета Access, полученное в результате такого запроса, также имеет расписание.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|срока действия|[експиратионпаттерн](expirationpattern.md)|По истечении срока действия доступа.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Для повторяющегося доступа. Не используется в данный момент.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule",
  "baseType": ""
}-->

```json
{
    "startDateTime": "2020-08-11T23:06:53.307Z",
    "expiration": {
        "endDateTime": "2020-09-10T23:06:53.307Z",
        "type": "afterDateTime"
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
