---
title: Тип перечисления teamsAsyncOperationType
description: Типы teamsAsyncOperation. Участники будут добавляться здесь дополнительных async поддерживают операции.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516569"
---
# <a name="teamsasyncoperationtype-enum-type"></a>Тип перечисления teamsAsyncOperationType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Типы [teamsAsyncOperation](teamsasyncoperation.md). Участники будут добавляться здесь дополнительных async поддерживают операции.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|Invalid|(0)|Недопустимое значение|
|cloneTeam|$1|Операция следует скопировать группы.|
|archiveTeam|–2|Операции в архив группы.|
|unarchiveTeam|–3|Операция восстановление архивированных группы.|
|createTeam|–3|Операция создать группу «с нуля».|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
