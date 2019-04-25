---
title: тип перечисления Теамсасинкоператионстатус
description: Описывает текущее состояние Теамсасинкоператион.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578865"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>тип перечисления Теамсасинкоператионстатус

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает текущее состояние [теамсасинкоператион](teamsasyncoperation.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|Недопустимый|нуль|Недопустимое значение.|
|notStarted|1 |Операция не запущена.|
|inProgress|2 |Выполняется операция.|
|закончил|3 |Операция выполнена успешно.|
|сбоев|4 |Сбой операции.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
