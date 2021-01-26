---
title: Отчеты о работе с электронной почтой
description: Вы можете получить высокоуровневый вид трафика электронной почты в организации на странице "Отчеты". Кроме того, вы можете подробно и подробно разобраться в мини-приложениях "Действия с электронной почтой" в вашей организации.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: db9ea032b418a6beca7afb7c15eb16b762e6ed11
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983800"
---
# <a name="email-activity-reports"></a>Отчеты о работе с электронной почтой

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить высокоуровневый вид трафика электронной почты в организации на странице "Отчеты". Вы также можете и подробно разобраться в мини-приложениях "Действия с электронной почтой" в вашей организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Действия с почтой](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Узнайте, какие действия пользователи выполняли с электронной почтой. |
| [Получение количества действий](../api/reportroot-getemailactivitycounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации. |
| [Получение количества пользователей](../api/reportroot-getemailactivityusercounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма. |


