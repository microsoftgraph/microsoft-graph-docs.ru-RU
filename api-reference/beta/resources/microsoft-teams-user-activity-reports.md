---
title: Отчеты о действиях пользователей Microsoft Teams
description: Используйте отчеты Microsoft Teams действий пользователей, чтобы получить сведения о Microsoft Teams действий пользователей в организации.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 46ab4747f5ce4e38ab57a56e54528f4c3dfb9360
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044682"
---
# <a name="microsoft-teams-user-activity-reports"></a>Отчеты о действиях пользователей Microsoft Teams

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте отчеты Microsoft Teams действий пользователей, чтобы получить сведения о Microsoft Teams действий пользователей в организации.

## <a name="methods"></a>Методы

| Метод                                                       | Возвращаемый тип | Описание                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsuseractivityuserdetail.md) | Stream      | Получение сведения о действиях отдельных пользователей Microsoft Teams.     |
| [Получение количества действий](../api/reportroot-getteamsuseractivitycounts.md) | Stream      | Получение количества действий Microsoft Teams по типам. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. Действия выполняются Microsoft Teams лицензированными пользователями. |
| [Общее количество действий](../api/reportroot-getteamsuseractivitytotalcounts.md) | Stream      | Получение количества действий Microsoft Teams по типам. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. Эти действия выполняются Microsoft Teams или не лицензированными пользователями. |
| [Получение количества пользователей](../api/reportroot-getteamsuseractivityusercounts.md) | Stream      | Получите количество лицензированных Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Общее количество пользователей](../api/reportroot-getteamsuseractivitytotalusercounts.md) | Stream      | Получите число пользователей, Microsoft Teams лицензированных или не лицензированных пользователей по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | Stream      | Получите количество лицензированных Microsoft Teams по типу действия за выбранный период. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний. |
| [Общее количество пользователей в распределении](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | Stream      | Получите количество лицензированных Microsoft Teams пользователей по типу активности за выбранный период. Типы действий — это количество командных сообщений чата, частных сообщений чата, звонков и собраний. |


