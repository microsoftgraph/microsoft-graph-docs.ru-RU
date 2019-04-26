---
title: тип перечисления объекта teamsasyncoperationtype
description: Типы Теамсасинкоператион. Элементы будут добавлены здесь, так как поддерживаются дополнительные асинхронные операции.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553640"
---
# <a name="teamsasyncoperationtype-enum-type"></a>тип перечисления объекта teamsasyncoperationtype

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Типы [теамсасинкоператион](teamsasyncoperation.md). Элементы будут добавлены здесь, так как поддерживаются дополнительные асинхронные операции.

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|Недопустимый|нуль|Недопустимое значение.|
|Клонетеам|1 |Операция клонирования команды.|
|Арчиветеам|2 |Операция архивации команды.|
|Унарчиветеам|3 |Операция восстановления архивной команды.|
|Креатетеам|3 |Операция по созданию команды с нуля.|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
