---
title: Тип ресурса requestSchedule
description: Расписание запроса может быть включено в запрос на назначение пакета доступа и присутствует в назначении пакета доступа. В PIM используйте этот ресурс, чтобы определить расписание, в течение которых субъекту будет присвоено допустимое или активное назначение ролей.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1e8988f70ba9ee108248bbb7ce2322bb0136d00f
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899131"
---
# <a name="requestschedule-resource-type"></a>Тип ресурса requestSchedule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-overview.md) запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета для доступа. Этот запрос может включать расписание, в течение которых пользователь должен иметь назначение.  Назначение пакета для доступа, которое является результатом такого запроса, также имеет расписание.

В PIM используйте этот ресурс, чтобы определить расписание, в течение которых субъекту будет присвоено допустимое или активное назначение ролей.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|startDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. В PIM, когда допустимое или активное назначение становится активным.|
|Истечения срока действия|[expirationPattern](expirationpattern.md)|При управлении правами, когда срок действия доступа должен истечь.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Для повторяющегося доступа, допустимого или активного назначения. В настоящее время это свойство не поддерживается как в PIM, так и в управлении правами.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
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


