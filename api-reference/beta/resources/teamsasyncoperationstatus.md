---
title: Тип перечисления teamsAsyncOperationStatus
description: Описывает текущее состояние teamsAsyncOperation.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511711"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>Тип перечисления teamsAsyncOperationStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает текущее состояние [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="members"></a>Элементы

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|Invalid|(0)|Недопустимое значение|
|notStarted|$1|Эта операция не запущена.|
|InProgress|–2|Выполнение операции.|
|succeeded|–3|Операция успешно завершена.|
|failed|4|Сбой операции.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
