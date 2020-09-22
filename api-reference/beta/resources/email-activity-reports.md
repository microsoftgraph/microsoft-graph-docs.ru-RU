---
title: Отчеты о работе с электронной почтой
description: С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации. Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f3c1ccd2700bce7a054cfec8fed943c01a3f4a1c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055549"
---
# <a name="email-activity-reports"></a>Отчеты о работе с электронной почтой

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью страницы отчеты вы можете получить высокоуровневое представление трафика электронной почты в вашей организации. Вы также можете перейти на мини-приложение "действия электронной почты", чтобы ознакомиться с тенденциями и сведениями о действиях с электронной почтой в вашей организации.

> **Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-Activity email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [емаилактивитюсердетаил](../resources/emailactivityuserdetail.md) | Узнайте, какие действия пользователи выполняли с электронной почтой. |
| [Получение количества действий](../api/reportroot-getemailactivitycounts.md) | Stream          | [емаилактивитисуммари](../resources/emailactivitysummary.md) | Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации. |
| [Получение количества пользователей](../api/reportroot-getemailactivityusercounts.md) | Stream          | [емаилактивитисуммари](../resources/emailactivitysummary.md) | Позволяет понять, как меняется количество уникальных пользователей, которые отправляют, читают и получают письма. |


