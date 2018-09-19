# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Интеграция оповещений API-интерфейса безопасности Microsoft Graph с SIEM

API-интерфейс безопасности Microsoft Graph позволяет осуществлять управление оповещениями системы безопасности из всех продуктов безопасности Майкрософт, известных как поставщики безопасности Microsoft Graph, через одну конечную точку REST. В некоторых организациях уже принимаются данные через монитор Azure в решения SIEM. В целях упрощения интеграции оповещения системы безопасности, доступные через API Microsoft Graph безопасности, могут также быть подготовлены клиентом для подписки с помощью Azure Monitor. Если в организации уже настроена интеграция монитора Azure с вашим решением SIEM, то вы можете легко выполнять потоковую передачу оповещений системы безопасности вашей организации в дополнение к существующим данным, доступным через Azure Monitor.

Azure Monitor поддерживает соединители, обеспечивающие подключение к нескольким продуктам SIEM. Список поддерживаемых продуктов SIEM см. в разделе [Отправка данных в концентратор событий](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Интеграция API-интерфейсов безопасности Microsoft Graph в настоящее время доступна для [Splunk](https://splunkbase.splunk.com/) и [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).

Чтобы получить сведения об интеграции API безопасности Microsoft Graph для конкретных решений SIEM, см.:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
