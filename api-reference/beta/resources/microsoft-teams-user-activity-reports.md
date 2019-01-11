---
title: Отчеты о действиях пользователей Microsoft Teams
description: Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.
localization_priority: Normal
ms.openlocfilehash: 2fc2eee8243a338204687114d2f1de3d2e794a9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845524"
---
# <a name="microsoft-teams-user-activity-reports"></a>Отчеты о действиях пользователей Microsoft Teams

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается. Эти интерфейсы API в Китае Microsoft Graph обслуживается 21Vianet не поддерживаются.

Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.

## <a name="methods"></a>Методы

| Метод                                   | Возвращаемый тип                              | Описание                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | Получение сведения о действиях отдельных пользователей Microsoft Teams. |
| [Получение количества действий](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Получение количества действий Microsoft Teams по типам. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Получение количества пользователей](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Получение сведений о количестве пользователей по типам действий. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
