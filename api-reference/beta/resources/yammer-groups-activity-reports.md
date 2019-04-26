---
title: Отчеты об активности в группах Yammer
description: Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9035984cf33c56811dc411a6c9cc01e6d438d194
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342795"
---
# <a name="yammer-groups-activity-reports"></a>Отчеты об активности в группах Yammer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [Яммерграупсактивитидетаил](../resources/yammergroupsactivitydetail.md) | Получите сведения об активности в группах Yammer. |
| [Получение количества групп](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Поток          | [Яммерграупсактивитиграупкаунтс](../resources/yammergroupsactivitygroupcounts.md) | Узнайте, сколько всего существовало групп и в скольких из них была активность. |
| [Получение количества действий](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [Яммерграупсактивитикаунтс](../resources/yammergroupsactivitycounts.md) | Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах. |
