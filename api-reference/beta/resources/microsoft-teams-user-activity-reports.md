---
title: Отчеты о действиях пользователей Microsoft Teams
description: Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574721"
---
# <a name="microsoft-teams-user-activity-reports"></a>Отчеты о действиях пользователей Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.

## <a name="methods"></a>Методы

| Метод                                   | Возвращаемый тип                              | Описание                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | Получение сведения о действиях отдельных пользователей Microsoft Teams. |
| [Получение количества действий](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Получение количества действий Microsoft Teams по типам. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Получение количества пользователей](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Получение сведений о количестве пользователей по типам действий. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
