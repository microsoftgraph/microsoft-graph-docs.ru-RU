---
title: Отчеты о работе со Skype для бизнеса
description: Можно получить подробные сведения об активности внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a81e27d58316cb415d6296b4f77519a3f2125643
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512397"
---
# <a name="skype-for-business-activity-reports"></a>Отчеты о работе со Skype для бизнеса

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Можно получить подробные сведения об активности внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | Получите сведения о действиях пользователей в Skype для бизнеса. |
| [Получение количества действий](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Узнайте, как меняется количество организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Поток          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Отследите, как меняется количество уникальных организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
