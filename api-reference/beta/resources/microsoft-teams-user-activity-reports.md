---
title: Отчеты о действиях пользователей Microsoft Teams
description: Используйте отчеты о действиях пользователей Microsoft Teams, чтобы получить сведения о действиях пользователей Microsoft Teams в вашей организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 97a32ce99eab154a99a97d9c9dab7fc49d4a7a1d
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766121"
---
# <a name="microsoft-teams-user-activity-reports"></a>Отчеты о действиях пользователей Microsoft Teams

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте отчеты о действиях пользователей Microsoft Teams, чтобы получить сведения о действиях пользователей Microsoft Teams в вашей организации.

## <a name="methods"></a>Методы

| Метод                                                       | Возвращаемый тип                                                  | Описание                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | Получение сведения о действиях отдельных пользователей Microsoft Teams.     |
| [Получение количества действий](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Получение количества действий Microsoft Teams по типам. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. Действия выполняются лицензированными пользователями Microsoft Teams. |
| [Общее количество действий](../api/reportroot-getteamsuseractivitytotalcounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Получение количества действий Microsoft Teams по типам. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. Действия выполняются лицензированными или не лицензированными пользователями Microsoft Teams. |
| [Получение количества пользователей](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Получите число лицензированных пользователей Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Общее количество пользователей](../api/reportroot-getteamsuseractivitytotalusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Получите число пользователей Microsoft Teams, лицензированных или не лицензированных по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) | Получите число лицензированных пользователей Microsoft Teams по типу активности за выбранный период. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний. |
| [Общее количество пользователей в распределении](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) | Получите число пользователей Microsoft Teams, лицензированных или не лицензированных по типу действий за выбранный период. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний. |


