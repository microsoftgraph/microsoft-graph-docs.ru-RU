---
title: Отчеты об использовании почтовых приложений
description: Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 03d33080a1d37512431c1922c217a8abe83a4828
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055521"
---
# <a name="email-app-usage-reports"></a>Отчеты об использовании почтовых приложений

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.

> **Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [емаилаппусажеусердетаил](../resources/emailappusageuserdetail.md) | Узнайте, какие действия пользователи выполняли в различных почтовых приложениях. |
| [Получение количества пользователей по приложениям](../api/reportroot-getemailappusageappsusercounts.md) | Поток          | [емаилаппусажеаппсусеркаунтс](../resources/emailappusageappsusercounts.md) | Узнайте, сколько уникальных пользователей у каждого почтового приложения. |
| [Получение количества пользователей](../api/reportroot-getemailappusageusercounts.md) | Stream          | [емаилаппусажеусеркаунтс](../resources/emailappusageusercounts.md) | Узнайте, сколько уникальных пользователей подключалось к Exchange Online с помощью любого почтового приложения. |
| [Получение количества пользователей по версиям](../api/reportroot-getemailappusageversionsusercounts.md) | Поток          | [емаилаппусажеверсионсусеркаунтс](../resources/emailappusageversionsusercounts.md) | Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера. |


