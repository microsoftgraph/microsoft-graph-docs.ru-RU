---
title: тип ресурса teamClassSettings
description: Представляет параметры, специфические для групп класса типа.
ms.localizationpriority: medium
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fd7a3163abd23d7c009ef3a03c668335eeb1e453
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134362"
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

