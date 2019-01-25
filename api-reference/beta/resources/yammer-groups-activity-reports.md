---
title: Отчеты об активности в группах Yammer
description: Можно воспользоваться сведениями в действие группы Yammer в вашей организации и видеть, сколько групп Yammer создаются и используются.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 05e5826a85e7d2e37af82cdf6277857746b1b922
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514161"
---
# <a name="yammer-groups-activity-reports"></a>Отчеты об активности в группах Yammer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Можно воспользоваться сведениями в действие группы Yammer в вашей организации и видеть, сколько групп Yammer создаются и используются.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | Получите сведения об активности в группах Yammer. |
| [Получение количества групп](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | Узнайте, сколько всего существовало групп и в скольких из них была активность. |
| [Получение количества действий](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | Узнайте, сколько сообщений Yammer было отправлено, прочитано и оценено в группах. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
