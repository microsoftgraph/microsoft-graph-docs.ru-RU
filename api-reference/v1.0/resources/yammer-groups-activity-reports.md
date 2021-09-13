---
title: Отчеты об активности в группах Yammer
description: Эти отчеты позволяют получить представление об активности в группах Yammer в организации и узнать, сколько групп Yammer создается и используется.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7365466d0cdb9971b35f0196b672091fddd12bac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078604"
---
# <a name="yammer-groups-activity-reports"></a>Отчеты об активности в группах Yammer

Пространство имен: microsoft.graph

Эти отчеты позволяют получить представление об активности в группах Yammer в организации и узнать, сколько групп Yammer создается и используется.

> **Примечание:** Сведения о различных представлениях отчетов и именах см. в [Microsoft 365 отчетов — Yammer групп.](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getyammergroupsactivitydetail.md) | Поток      | Получите сведения об активности в группах Yammer. |
| [Получение количества групп](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Поток      | Узнайте, сколько всего существовало групп и в скольких из них была активность. |
| [Получение количества действий](../api/reportroot-getyammergroupsactivitycounts.md) | Stream      | Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах. |

