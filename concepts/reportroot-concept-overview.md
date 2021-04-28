---
title: Обзор API отчетов Microsoft Graph
description: API отчетов Microsoft Graph позволяют получить представление о действиях ресурсов приложений и клиента.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.custom: scenarios:getting-started
ms.openlocfilehash: 52247aa125745055f4fec5b651c8c175597d1b82
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055598"
---
# <a name="microsoft-graph-reports-api-overview"></a>Обзор API отчетов Microsoft Graph

API отчетов Microsoft Graph позволяют получить представление о действиях приложений и ресурсов в клиенте Azure Active Directory.

> [!VIDEO https://www.youtube-nocookie.com/embed/P6HneRXYdx8]

## <a name="why-use-the-reports-api"></a>Зачем использовать API отчетов?

### <a name="integrate-microsoft-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Интеграция отчетов об использовании Microsoft 365 с имеющимся в организации решением для отчетности
Во многих компаниях уже есть решения для отчетности, использующие приложение или веб-портал для создания отчетов. С помощью API отчетов вы можете внедрить данные об использовании Microsoft 365 в имеющееся в организации решение для отчетности, чтобы все отчеты ИТ-служб находились в одном расположении.

### <a name="retain-usage-reports-for-historical-analysis"></a>Сохранение отчетов об использовании для анализа архивных данных
С помощью API отчетов вы можете получать данные, доступные во всех отчетах об использовании, включая сводки на уровне организации по службам, сведения об использовании на уровне сущности (пользователей, сайтов, учетных записей) за последние 7, 30, 90 или 180 дней, а также сводные показатели по действиям за день. Благодаря этому вы можете хранить статистические сведения об использовании столько, сколько нужно.

### <a name="analyze-ad-fs-application-activity-and-configuration"></a>Анализ конфигурации и работы приложений AD FS
Содержит сведения о настройке проверяющей стороны с помощью служб федерации Active Directory (AD FS), обобщенные сведения об использовании, а также о том, можно ли перенести настройку проверяющей стороны в Azure Active Directory.

### <a name="monitor-application-sign-ins"></a>Мониторинг входов в учетные записи в приложении

Отслеживание использования приложений и принятие решений об их использовании

### <a name="determine-who-is-using-your-applications-and-how-are-they-using-them"></a>Определяйте, кто и как будет использовать ваши приложения.

Отчеты об использовании методов проверки подлинности позволяют понять, как пользователи в вашей организации используют функции Azure Active Directory (Azure AD), такие как самостоятельный сброс пароля и многофакторная проверка подлинности (MFA). Эти отчеты помогают определить, какие методы проверки подлинности более успешны в вашей организации, с какими типами ошибок сталкиваются пользователи и какую кампанию нужно провести, чтобы помочь пользователям с внедрением самостоятельного сброса паролей и MFA.

### <a name="monitor-activity-on-an-azure-ad-tenant"></a>Отслеживание активности в клиенте Azure AD

Получите более ясное представление о том, как пользователи получают доступ к службам Azure AD и используют их. Данные можно анализировать и создавать настраиваемые решения, которые отвечают потребностям вашей организации.

## <a name="what-data-can-i-access-by-using-the-reports-apis"></a>К каким данным можно получать доступ с помощью API отчетов?

С помощью API отчетов можно получать доступ к наборам данных, перечисленным в приведенной ниже таблице.

| API отчетов | Набор данных |
|:------------ |:-------- |
| Действие | [Аудит каталога](/graph/api/resources/directoryaudit?view=graph-rest-1.0)<br/>[Вход](/graph/api/resources/signin?view=graph-rest-1.0)<br/>[Подготовка (Предварительная версия)](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) |
| Приложения AD FS | [Детальная сводка о проверяющей части (Предварительная версия)](/graph/api/resources/relyingpartydetailedsummary?view=graph-rest-beta) |
| Регистрация приложения | [Счетчик регистрации пользователей учетных данных (Предварительная версия)](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta)<br/>[Сведения о регистрации пользователей учетных данных (Предварительная версия)](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) <br/>[Сведения об использовании учетных данных пользователей (Предварительная версия)](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) <br/>[Сводка по использованию учетных данных (Предварительная версия)](/graph/api/resources/credentialusagesummary?view=graph-rest-beta)|
| Вход в приложение | [Сводка по входу (Предварительная версия)](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) <br/>[Данные для входа (Предварительная версия)](/graph/api/resources/applicationsignindetailedsummary?view=graph-rest-beta)|
| Microsoft Teams | [Использование устройств](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0)<br/>[Действия пользователей](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0) |
| Microsoft 365 (общая) | [Активации](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0)<br/>[Активные пользователи](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0)<br/>[Действия в группах](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0) |
| OneDrive | [Действия](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0)<br/>[Использование](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0) |
| Outlook | [Действия](/graph/api/resources/email-activity-reports?view=graph-rest-1.0)<br/>[Использование приложений](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0)<br/>[Использование почтовых ящиков](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0) |
| SharePoint | [Действия](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0)<br/>[Использование сайтов](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0) |
| Skype для бизнеса | [Действия](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0)<br/>[Использование устройств](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Использование устройств](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Действия участников](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0)<br/>[Одноранговые действия](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0) |
| Yammer | [Действия](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0)<br/>[Использование устройств](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0)<br/>[Действия в группах](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0) |

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API отчетов об удостоверении и доступе в бета-версии Microsoft Graph](/graph/api/resources/report-identity-access?view=graph-rest-beta)
- [API отчетов об использовании Microsoft 365 в Microsoft Graph 1.0](/graph/api/resources/report?view=graph-rest-1.0)
- [API отчетов об использовании Microsoft 365 в бета-версии Microsoft Graph](/graph/api/resources/report?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

* Изучите API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
* Узнайте больше об [использовании REST API отчетов](/graph/api/resources/report?view=graph-rest-1.0).
