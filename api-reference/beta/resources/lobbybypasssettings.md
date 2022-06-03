---
title: Тип ресурса lobbyBypassSettings
description: Указывает, какие участники могут обходить зал ожидания собрания.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: db525d4d3a4f2999dd637745532789043b4f68df
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884169"
---
# <a name="lobbybypasssettings-resource-type"></a>Тип ресурса lobbyBypassSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, какие участники могут обходить зал ожидания собрания.

## <a name="properties"></a>Свойства

| Свойство              | Тип    | Описание                                                         |
| --------------------- | ------- | ------------------------------------------------------------------- |
| scope                 | [lobbyBypassScope](#lobbybypassscope-values)  | Указывает тип участников, которые автоматически допускаются в собрание, минуя зал ожидания. Необязательно.|
| isDialInBypassEnabled | Boolean | Указывает, следует ли всегда разрешать вызывающим абонентам входить в зал ожидания. Необязательно. |

### <a name="lobbybypassscope-values"></a>Значения lobbyBypassScope

В следующей таблице перечислены элементы [развиваемого перечисления](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). Необходимо использовать заголовок `Prefer: include-unknown-enum-members` запроса, чтобы получить следующие значения в этом развиваемом перечислении: `invited`, `organizationExcludingGuests`.

| Значение                    | Описание     |
| ------------------------ | --------------------------------------------------- |
| organizer | Только организатор допускается в собрание и обходит зал ожидания. Все остальные участники помещаются в зал ожидания собрания. |
| organization; | В собрание могут входить только участники  одной компании и гости, которые обходят "зал ожидания". Все остальные участники помещаются в зал ожидания собрания. |
| organizationAndFederated | Только участники из одной компании или доверенной организации и гости могут быть допущены на собрание и обходить "зал ожидания". Все остальные участники помещаются в зал ожидания собрания. |
| Все | Все участники могут быть допущены к собранию. Участники не помещаются в зал ожидания собрания. |
| Пригласил | Только пользователи, приглашенные организатором, могут входить в собрание и обходить зал ожидания. Все остальные участники помещаются в зал ожидания собрания. |
| organizationExcludingGuests |  Только участники из одной компании могут быть допущены в собрание и обходить "зал ожидания". Все остальные участники помещаются в зал ожидания собрания. |
| unknownFutureValue | Значение sentinel для развиваемого перечисления. Не следует использовать. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
