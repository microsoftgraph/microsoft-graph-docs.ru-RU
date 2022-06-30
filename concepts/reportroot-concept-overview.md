---
title: Обзор API отчетов Microsoft Graph
description: С помощью API отчетов можно внедрить данные об использовании Microsoft 365 в используемое в организации решение для отчетности, чтобы все отчеты ИТ-служб находились в одном расположении.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
ms.custom: scenarios:getting-started
ms.openlocfilehash: 84718f4a6fb1b0046387e6338980c99e5d91b881
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446128"
---
# <a name="microsoft-graph-reports-api-overview"></a>Обзор API отчетов Microsoft Graph

API отчетов Microsoft Graph позволяют получить представление о действиях приложений и ресурсов в клиенте Azure Active Directory (Azure AD).

> [!VIDEO https://www.youtube-nocookie.com/embed/P6HneRXYdx8]

## <a name="why-use-the-reports-api"></a>Зачем использовать API отчетов?

### <a name="integrate-microsoft-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Интеграция отчетов об использовании Microsoft 365 с имеющимся в организации решением для отчетности
Во многих компаниях уже есть решения для отчетности, использующие приложение или веб-портал для создания отчетов. С помощью API отчетов вы можете внедрить данные об использовании Microsoft 365 в имеющееся в организации решение для отчетности, чтобы все отчеты ИТ-служб находились в одном расположении.

### <a name="retain-usage-reports-for-historical-analysis"></a>Сохранение отчетов об использовании для анализа архивных данных
С помощью API отчетов вы можете получать данные, доступные во всех отчетах об использовании, включая сводки на уровне организации по службам, сведения об использовании на уровне сущности (пользователей, сайтов, учетных записей) за последние 7, 30, 90 или 180 дней, а также сводные показатели по действиям за день. Благодаря этому вы можете хранить статистические сведения об использовании столько, сколько нужно.

### <a name="analyze-ad-fs-application-activity-and-configuration"></a>Анализ конфигурации и работы приложений AD FS
Содержит сведения о настройке проверяющей стороны с помощью служб федерации Active Directory (AD FS), обобщенные сведения об использовании, а также о том, можно ли перенести настройку проверяющей стороны в Azure Active Directory.

### <a name="monitor-application-sign-ins"></a>Мониторинг входов в учетные записи в приложении

Отслеживание использования приложений и принятие решений об их использовании

### <a name="determine-who-is-using-your-applications-and-how-are-they-using-them"></a>Определяйте, кто и как будет использовать ваши приложения.

Отчеты об использовании методов проверки подлинности позволяют понять, как пользователи в вашей организации используют функции Azure Active Directory (Azure AD), такие как самостоятельный сброс пароля и многофакторная проверка подлинности (MFA). Эти отчеты помогают определить, какие методы проверки подлинности более успешны в вашей организации, с какими типами ошибок сталкиваются пользователи и какую кампанию нужно провести, чтобы помочь пользователям с внедрением самостоятельного сброса паролей и MFA.

### <a name="monitor-activity-on-an-azure-ad-tenant"></a>Отслеживание активности в клиенте Azure AD

Получите более ясное представление о том, как пользователи получают доступ к службам Azure AD и используют их. Данные можно анализировать и создавать настраиваемые решения, которые отвечают потребностям вашей организации.

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>К каким данным можно получать доступ с помощью API отчетов?

С помощью API отчетов вы можете получать доступ к наборам данных, перечисленным в приведенной ниже таблице.

| API отчетов | Набор данных |
|:------------ |:-------- |
| Действие | [Аудит каталога](/graph/api/resources/directoryaudit)<br/>[Вход](/graph/api/resources/signin)<br/>[Provisioning](/graph/api/resources/provisioningobjectsummary) |
| Приложения AD FS | [Подробная сводка проверяющей стороны (предварительная версия)](/graph/api/resources/relyingpartydetailedsummary) |
| Регистрация приложения | [Счетчик регистрации пользователей учетных данных (предварительная версия)](/graph/api/resources/credentialuserregistrationcount)<br/>[Сведения о регистрации пользователей учетных данных (предварительная версия)](/graph/api/resources/credentialuserregistrationdetails) <br/>[Сведения об использовании учетных данных пользователей (предварительная версия)](/graph/api/resources/usercredentialusagedetails) <br/>[Сводка использования учетных данных (предварительная версия)](/graph/api/resources/credentialusagesummary)|
| Вход в приложение | [Сводка входа (предварительная версия)](/graph/api/resources/applicationsigninsummary) <br/>[Сведения о входе (предварительная версия)](/graph/api/resources/applicationsignindetailedsummary)|
| Microsoft Teams | [Использование устройств](/graph/api/resources/microsoft-teams-device-usage-reports)<br/>[Использование команды](/graph/api/resources/microsoft-teams-team-usage-reports)<br/>[Действия пользователей](/graph/api/resources/microsoft-teams-user-activity-reports)|
| Microsoft 365 (общая) | [Активации](/graph/api/resources/office-365-activations-reports)<br/>[Активные пользователи](/graph/api/resources/office-365-active-users-reports)<br/>[Действия в группах](/graph/api/resources/office-365-groups-activity-reports) |
| OneDrive | [Действия](/graph/api/resources/onedrive-activity-reports)<br/>[Использование](/graph/api/resources/onedrive-usage-reports) |
| Outlook | [Действия](/graph/api/resources/email-activity-reports)<br/>[Использование приложений](/graph/api/resources/email-app-usage-reports)<br/>[Использование почтовых ящиков](/graph/api/resources/mailbox-usage-reports) |
| SharePoint | [Действия](/graph/api/resources/sharepoint-activity-reports)<br/>[Использование сайтов](/graph/api/resources/sharepoint-site-usage-reports) |
| Skype для бизнеса | [Действия](/graph/api/resources/skype-for-business-activity-reports)<br/>[Использование устройств](/graph/api/resources/skype-for-business-device-usage-reports)<br/>[Использование устройств](/graph/api/resources/skype-for-business-device-usage-reports)<br/>[Действия участников](/graph/api/resources/skype-for-business-participant-activity-reports)<br/>[Одноранговые действия](/graph/api/resources/skype-for-business-peer-to-peer-activity) |
| Yammer | [Действия](/graph/api/resources/yammer-activity-reports)<br/>[Использование устройств](/graph/api/resources/yammer-device-usage-reports)<br/>[Действия в группах](/graph/api/resources/yammer-groups-activity-reports) |

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [API отчетов об удостоверении и доступе в бета-версии Microsoft Graph](/graph/api/resources/report-identity-access?view=graph-rest-beta&preserve-view=true)
- [API отчетов об использовании Microsoft 365 в Microsoft Graph 1.0](/graph/api/resources/report?view=graph-rest-1.0&preserve-view=true)
- [API отчетов об использовании Microsoft 365 в бета-версии Microsoft Graph](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Дальнейшие действия

* Изучайте интерфейсы API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
