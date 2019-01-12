---
title: Отчеты об использовании почтовых приложений
description: Можно видеть, сколько приложений электронной почты используются для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: 6a75b494705c56e63d4b7d5b2f58d76de64b9bce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912920"
---
# <a name="email-app-usage-reports"></a>Отчеты об использовании почтовых приложений

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Можно видеть, сколько приложений электронной почты используются для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) | Узнайте, какие действия пользователи выполняли в различных почтовых приложениях. |
| [Получение количества пользователей по приложениям](../api/reportroot-getemailappusageappsusercounts.md) | Поток          | [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) | Узнайте, сколько уникальных пользователей у каждого почтового приложения. |
| [Получение количества пользователей](../api/reportroot-getemailappusageusercounts.md) | Stream          | [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) | Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения. |
| [Получение количества пользователей по версиям](../api/reportroot-getemailappusageversionsusercounts.md) | Поток          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера. |
