---
title: Отчеты об использовании почтовых приложений
description: Вы можете узнать, сколько почтовых приложений используется для подключения к Exchange Online. Вы также можете посмотреть, какие версии приложений Outlook используются, что позволит вам выявить пользователей старых версий и связаться с ними по поводу обновления.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 7f332359af9a6147894bb69e6d12532a83394bb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506687"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
