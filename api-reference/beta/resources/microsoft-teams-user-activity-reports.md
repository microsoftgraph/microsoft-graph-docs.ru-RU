---
title: Отчеты о действиях пользователей Microsoft Teams
description: Использование отчетов об активности пользователей группами Майкрософт для получения полезные сведения о в действие пользователя группами Майкрософт в вашей организации.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2dd3ed3cde8f1a00ae7a48336bfaef857721f046
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991435"
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
