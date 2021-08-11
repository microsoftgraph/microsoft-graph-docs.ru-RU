---
title: тип ресурса teamClassSettings
description: Представляет параметры, специфические для групп класса типа.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a28eb208ea36091b272bd38815a6b8bfb3839cbc84fe9c47075f2c85a863e32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54228977"
---
# <a name="teamclasssettings-resource-type"></a>тип ресурса teamClassSettings

Пространство имен: microsoft.graph

Представляет свойства группы, определенные для [класса.](team.md) Доступна только в том случае, если команда представляет класс.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|Логический|Если установлено, позволяет отправлять еженедельные назначения дайджест электронных писем родителям и опекунам, при условии, что администратор клиента включил `true` параметр глобально.|

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

