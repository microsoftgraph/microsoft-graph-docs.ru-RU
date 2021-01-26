---
title: Отчеты об использовании почтовых приложений
description: Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: efa7a747ae26da8f34c32d9473a84f95b7433ee0
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982707"
---
# <a name="email-app-usage-reports"></a>Отчеты об использовании почтовых приложений

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании почтовых приложений.](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) | Узнайте, какие действия пользователи выполняли в различных почтовых приложениях. |
| [Получение количества пользователей по приложениям](../api/reportroot-getemailappusageappsusercounts.md) | Поток          | [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) | Узнайте, сколько уникальных пользователей у каждого почтового приложения. |
| [Получение количества пользователей](../api/reportroot-getemailappusageusercounts.md) | Stream          | [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) | Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения. |
| [Получение количества пользователей по версиям](../api/reportroot-getemailappusageversionsusercounts.md) | Поток          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера. |


