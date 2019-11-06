---
title: Тип ресурса Теамкласссеттингс
description: Представляет параметры, характерные для Teams типа Class.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8d345cd229c4a6c003c87865b5aaddf01096b4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998618"
---
# <a name="teamclasssettings-resource-type"></a>Тип ресурса Теамкласссеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства [команды](team.md), зависящие от класса. Доступно только в том случае, если команда представляет класс.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|нотифигуардиансабаутассигнментс|Boolean|Если задано `true`значение, разрешает отправку сообщений сводки по неделям в родительские и опекуны, если администратор клиента включил параметр глобально.|

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
