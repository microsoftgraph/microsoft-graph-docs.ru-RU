---
title: Отчеты об активности в группах Yammer
description: Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: cdeb94c9b5b687ab9584a236daaafb7c018a809c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897472"
---
# <a name="yammer-groups-activity-reports"></a>Отчеты об активности в группах Yammer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить подробные сведения о действиях в группах Yammer в Организации и узнать, сколько групп Yammer создается и используется.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports: активность групп Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [яммерграупсактивитидетаил](../resources/yammergroupsactivitydetail.md) | Получите сведения об активности в группах Yammer. |
| [Получение количества групп](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Поток          | [яммерграупсактивитиграупкаунтс](../resources/yammergroupsactivitygroupcounts.md) | Узнайте, сколько всего существовало групп и в скольких из них была активность. |
| [Получение количества действий](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [яммерграупсактивитикаунтс](../resources/yammergroupsactivitycounts.md) | Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах. |
