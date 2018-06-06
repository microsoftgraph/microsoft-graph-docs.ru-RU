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
|Microsoft Teams|[Использование устройств](../api-reference/v1.0/resources/microsoft_teams_device_usage_reports.md)<br/>|[Действия пользователей](../api-reference/v1.0/resources/microsoft_teams_user_activity_reports.md)|
|Office 365 (общее) |[Активации](../api-reference/v1.0/resources/office_365_activations_reports.md)<br/>[Активные пользователи](../api-reference/v1.0/resources/office_365_active_users_reports.md)<br/>[Действия в группах](../api-reference/v1.0/resources/office_365_groups_activity_reports.md)|
|OneDrive |[Действия](../api-reference/v1.0/resources/onedrive_activity_reports.md)<br/>[Использование](../api-reference/v1.0/resources/onedrive_usage_reports.md)|
|Outlook|[Действия](../api-reference/v1.0/resources/email_activity_reports.md)<br/>[Использование приложений](../api-reference/v1.0/resources/email_app_usage_reports.md)<br/>[Использование почтовых ящиков](../api-reference/v1.0/resources/mailbox_usage_reports.md)|
|SharePoint |[Действия](../api-reference/v1.0/resources/sharepoint_activity_reports.md)<br/>[Использование сайтов](../api-reference/v1.0/resources/sharepoint_site_usage_reports.md)|
|Skype для бизнеса |[Действия](../api-reference/v1.0/resources/skype_for_business_activity_reports.md)<br/>[Использование устройств](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[Использование устройств](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[Действия участников](../api-reference/v1.0/resources/skype_for_business_participant_activity_reports.md)<br/>[Одноранговые действия](../api-reference/v1.0/resources/skype_for_business_peer_to_peer_activity.md)|
|Yammer |[Действия](../api-reference/v1.0/resources/yammer_activity_reports.md)<br/>[Использование устройств](../api-reference/v1.0/resources/yammer_device_usage_reports.md)<br/>[Действия в группах](../api-reference/v1.0/resources/yammer_groups_activity_reports.md)|

## <a name="next-steps"></a>Дальнейшие действия

* Изучите API в [песочнице Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).
* Узнайте больше об [использовании REST API отчетов](../api-reference/v1.0/resources/report.md).
