---
title: Отчеты об использовании почтовых приложений
description: Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: df40e61108a3933801f5e7c21057f71600b496ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340199"
---
# <a name="email-app-usage-reports"></a>Отчеты об использовании почтовых приложений

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [Емаилаппусажеусердетаил](../resources/emailappusageuserdetail.md) | Узнайте, какие действия пользователи выполняли в различных почтовых приложениях. |
| [Получение количества пользователей по приложениям](../api/reportroot-getemailappusageappsusercounts.md) | Stream          | [Емаилаппусажеаппсусеркаунтс](../resources/emailappusageappsusercounts.md) | Узнайте, сколько уникальных пользователей у каждого почтового приложения. |
| [Получение количества пользователей](../api/reportroot-getemailappusageusercounts.md) | Stream          | [Емаилаппусажеусеркаунтс](../resources/emailappusageusercounts.md) | Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения. |
| [Получение количества пользователей по версиям](../api/reportroot-getemailappusageversionsusercounts.md) | Поток          | [Емаилаппусажеверсионсусеркаунтс](../resources/emailappusageversionsusercounts.md) | Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера. |
