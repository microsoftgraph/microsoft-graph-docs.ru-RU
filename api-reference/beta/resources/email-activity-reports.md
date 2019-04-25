---
title: Отчеты о работе с электронной почтой
description: С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации. Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 748199a2e846cc71a3f04c3ea1bda97dcf2c7301
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542921"
---
# <a name="email-activity-reports"></a>Отчеты о работе с электронной почтой

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации. Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailactivityuserdetail.md) | Поток          | [Емаилактивитюсердетаил](../resources/emailactivityuserdetail.md) | Узнайте, какие действия пользователи выполняли с электронной почтой. |
| [Получение количества действий](../api/reportroot-getemailactivitycounts.md) | Stream          | [Емаилактивитисуммари](../resources/emailactivitysummary.md) | Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации. |
| [Получение количества пользователей](../api/reportroot-getemailactivityusercounts.md) | Поток          | [Емаилактивитисуммари](../resources/emailactivitysummary.md) | Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
