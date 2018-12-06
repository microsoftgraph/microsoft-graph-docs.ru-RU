---
title: Обзор API отчетов Microsoft Graph
description: Отчеты об использовании в Центре администрирования Microsoft 365 помогают администраторам понимать, как используются службы Office 365 в организации. С помощью API отчетов в Microsoft Graph вы можете выполнить интеграцию с отчетами об использовании Office 365.
ms.openlocfilehash: d923d0003a276be15620998c53693a9bab7116d5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092693"
---
# <a name="microsoft-graph-reports-api-overview"></a>Обзор API отчетов Microsoft Graph

Отчеты об использовании в Центре администрирования Microsoft 365 помогают администраторам понимать, как используются службы Office 365 в организации. С помощью API отчетов в Microsoft Graph вы можете выполнить интеграцию с отчетами об использовании Office 365.

## <a name="why-use-the-reports-api"></a>Зачем использовать API отчетов?

### <a name="integrate-office-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Интеграция отчетов об использовании Office 365 с имеющимся в организации решением для отчетности
Во многих компаниях уже есть решения для отчетности, использующие приложение или веб-портал для создания отчетов. С помощью API отчетов вы можете внедрить данные об использовании Office 365 в имеющееся в организации решение для отчетности, чтобы все отчеты ИТ-служб находились в одном расположении.  

### <a name="retain-usage-reports-for-historical-analysis"></a>Сохранение отчетов об использовании для анализа архивных данных
С помощью API отчетов вы можете получать данные, доступные во всех отчетах об использовании, включая сводки на уровне организации по службам, сведения об использовании на уровне объектов (пользователей, сайтов, учетных записей) за последние 7, 30, 90 или 180 дней, а также сводные показатели по действиям за день. Благодаря этому вы можете хранить статистические сведения об использовании столько, сколько нужно.

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>К каким данным можно получать доступ с помощью API отчетов?

С помощью API отчетов вы можете получать доступ к наборам данных, перечисленным в приведенной ниже таблице.

|Приложение Office 365|Набор данных|
|:--------|:--------|
|Microsoft Teams|[Использование устройств](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0)<br/>|[Действия пользователей](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0)|
|Office 365 (общее) |[Активации](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0)<br/>[Активные пользователи](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0)<br/>[Действия в группах](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0)|
|OneDrive |[Действия](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0)<br/>[Использование](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0)|
|Outlook|[Действия](/graph/api/resources/email-activity-reports?view=graph-rest-1.0)<br/>[Использование приложений](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0)<br/>[Использование почтовых ящиков](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0)|
|SharePoint |[Действия](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0)<br/>[Использование сайтов](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0)|
|Skype для бизнеса |[Действия](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0)<br/>[Использование устройств](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Использование устройств](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Действия участников](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0)<br/>[Одноранговые действия](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0)|
|Yammer |[Действия](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0)<br/>[Использование устройств](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0)<br/>[Действия в группах](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0)|

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API отчетов об использовании Office 365 в Microsoft Graph 1.0](/graph/api/resources/report?view=graph-rest-1.0)
- [API отчетов об использовании Office 365 в бета-версии Microsoft Graph](/graph/api/resources/report?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

* Изучите API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
* Узнайте больше об [использовании REST API отчетов](/graph/api/resources/report?view=graph-rest-1.0).
