---
title: тип ресурса teamClassSettings
description: Представляет параметры, специфические для групп класса типа.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10ba45299a8c0d1b28b855aad3a2321930f618e9
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060475"
---
# <a name="teamclasssettings-resource-type"></a>тип ресурса teamClassSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства группы, определенные для [класса.](team.md) Доступна только в том случае, если команда представляет класс.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|Boolean|Если установлено, позволяет отправлять еженедельные назначения дайджест электронных писем родителям и опекунам, при условии, что администратор клиента включил `true` параметр глобально.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamClassSettings"
}-->

```json
{
  "notifyGuardiansAboutAssignments": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's classSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


