---
title: Отчеты о работе с электронной почтой
description: Высокоуровневое представление трафика электронной почты можно получить в рамках организации на странице отчеты. Вы также можете перейти в мини-приложения электронной почты активности понять тенденции и сведения на одного пользователя действия электронной почты в вашей организации.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: e11de43f197e520d653961af9b9090d06b085369
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528307"
---
# <a name="email-activity-reports"></a>Отчеты о работе с электронной почтой

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Высокоуровневое представление трафика электронной почты можно получить в рамках организации на странице отчеты. Вы также можете перейти в мини-приложения электронной почты активности понять тенденции и сведения на одного пользователя действия электронной почты в вашей организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Узнайте, какие действия пользователи выполняли с электронной почтой. |
| [Получение количества действий](../api/reportroot-getemailactivitycounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации. |
| [Получение количества пользователей](../api/reportroot-getemailactivityusercounts.md) | Поток          | [emailActivitySummary](../resources/emailactivitysummary.md) | Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
