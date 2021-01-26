---
title: Отчеты об активности в группах Yammer
description: Вы можете получить представление об активности групп Yammer в организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 09c8aa8476886f8bbf7266817449195b4c07aa05
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982427"
---
# <a name="yammer-groups-activity-reports"></a>Отчеты об активности в группах Yammer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить представление об активности групп Yammer в вашей организации и узнать, сколько групп Yammer создается и используется.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 о](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)действиях в группах Yammer.

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getyammergroupsactivitydetail.md) | Поток          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | Получите сведения об активности в группах Yammer. |
| [Получение количества групп](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Поток          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | Узнайте, сколько всего существовало групп и в скольких из них была активность. |
| [Получение количества действий](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах. |


