---
title: Тип перечисления clonableTeamParts
description: 'Описывается, какие часть команды должны клонируется. '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511466"
---
# <a name="clonableteamparts-enum-type"></a>Тип перечисления clonableTeamParts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывается, какие части [группы](../resources/team.md) должны клонировании. 

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|apps|$1|Скопируйте список установленных приложениях.|
|Tabs|–2|Копирует вкладок между каналами.|
|settings|4|Копирует все параметры в рамках рабочей группы, а также параметры ключа группы.|
|каналы|: = 8|Копирует структуру канала (но не сообщения в канале).|
|members|1.6|Копирует участников и владельцев группы.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
