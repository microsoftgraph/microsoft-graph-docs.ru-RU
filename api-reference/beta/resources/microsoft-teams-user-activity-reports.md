---
title: Отчеты о действиях пользователей Microsoft Teams
description: Используйте Microsoft Teams отчеты о действиях пользователей, чтобы получить аналитические сведения о Microsoft Teams действий пользователей в организации.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: d49f7c0ebccbc70f10460673d73aab3794283195
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704235"
---
# <a name="microsoft-teams-user-activity-reports"></a>Отчеты о действиях пользователей Microsoft Teams

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте Microsoft Teams отчеты о действиях пользователей, чтобы получить аналитические сведения о Microsoft Teams действий пользователей в организации.

## <a name="methods"></a>Методы

| Метод                                                       | Возвращаемый тип | Описание                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsuseractivityuserdetail.md) | Stream      | Получение сведения о действиях отдельных пользователей Microsoft Teams.     |
| [Получение количества действий](../api/reportroot-getteamsuseractivitycounts.md) | Stream      | Получение количества действий Microsoft Teams по типам. Действия выполняются Microsoft Teams лицензированными пользователями. |
| [Получение общего количества действий](../api/reportroot-getteamsuseractivitytotalcounts.md) | Stream      | Получение количества действий Microsoft Teams по типам. Действия выполняются Microsoft Teams лицензированными или не лицензированным пользователями. |
| [Получение количества пользователей](../api/reportroot-getteamsuseractivityusercounts.md) | Stream      | Получение количества лицензированных Microsoft Teams по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Получение общего количества пользователей](../api/reportroot-getteamsuseractivitytotalusercounts.md) | Stream      | Получение количества лицензированных Microsoft Teams пользователей по типу действия. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | Stream      | Получение количества лицензированных Microsoft Teams по типу действия за выбранный период. Типы действий — это количество сообщений чата teams, сообщений частного чата, звонков и собраний. |
| [Получение общего количества пользователей для распространения](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | Stream      | Получение количества лицензированных Microsoft Teams пользователей по типу действия за выбранный период. Типы действий — это количество сообщений чата teams, сообщений частного чата, звонков и собраний. |
| [Получение общего количества действий распространения](../api/reportroot-getteamsuseractivitytotaldistributioncounts.md) | Stream      | Получение количества действий Microsoft Teams за выбранный период. Типы действий — это сообщения в чате группы, личные сообщения чата, звонки, собрания, организованные собрания, собрания, длительность звука, длительность видео, продолжительность демонстрации экрана, отправка сообщений и ответных сообщений. |

