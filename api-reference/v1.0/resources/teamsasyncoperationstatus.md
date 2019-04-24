---
title: тип перечисления Теамсасинкоператионстатус
description: Описывает текущее состояние Теамсасинкоператион.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b3ceaca73fe013b76f44cdf9290f3c0935e93b0a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462230"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>тип перечисления Теамсасинкоператионстатус

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает текущее состояние [теамсасинкоператион](teamsasyncoperation.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|Недопустимый|нуль|Недопустимое значение.|
|notStarted|1,1|Операция не запущена.|
|inProgress|2|Выполняется операция.|
|закончил|4|Операция выполнена успешно.|
|сбоев|SP4|Сбой операции.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
