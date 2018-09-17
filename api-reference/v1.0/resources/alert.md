# <a name="alert-resource-type"></a>тип ресурса оповещения

Отображает потенциальные проблемы безопасности в среде клиента, которые были идентифицированы решениями безопасности Microsoft или партнеров. Используйте оповещения, чтобы объединить и упростить управление проблемами безопасности во всех подключенных решениях. Для дополнительной информации посмотрите выборку запросов в [песочнице Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).

Оповещения можно извлечь в следующих службах: центр безопасности Azure и Защита идентификации Azure Active Directory. В ближайшие месяцы планируется интеграция дополнительных поставщиков оповещений.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Получение оповещения](../api/alert_get.md) | [оповещение](alert.md) | Чтение свойств и связей объекта оповещения.|
|[Обновление оповещения](../api/alert_update.md) | [оповещение](alert.md) |Изменение объекта оповещений. |
|[Список оповещений](../api/alert_list.md) | коллекция [оповещений](alert.md) |Получение коллекции оповещений объекта.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|activityGroupName|String|Наименование или псевдоним группы действий (злоумышленников), к которой относится это предупреждение.|
|assignedTo|String|Имя специалиста, назначенного на рассмотрение, расследование и исправление (поддерживает [обновление](../api/alert_update.md)).|
|azureSubscriptionId|String|Идентификатор подписки Azure, отображается, если оповещение связано со службой Azure.|
|azureTenantId *|String|Идентификатор клиента Azure Active Directory.|
|category|String|Категория оповещения (например, кража персональных данных, программа-шантажист и т.д.).|
|closedDateTime|DateTimeOffset|Дата и время закрытия оповещения. Тип данных Timestamp предоставляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'` (поддерживает [обновление](../api/alert_update.md)).|
|cloudAppStates|коллекция [cloudAppSecurityState](cloudappsecuritystate.md)|Связанная с безопасностью информация (сгенерированная поставщиком) о состоянии облачных приложениях, к которым относится данное оповещение.|
|comments|Коллекция String|Комментарии клиента к оповещениям (для управления оповещениями клиентом) (поддерживает [обновление](../api/alert_update.md)).|
|confidence|Int32|Степень достоверности обнаруженных логик (в процентах от 1 до 100).|
|createdDateTime *|DateTimeOffset|Дата и время создания поставщиком оповещения. Тип данных Timestamp предоставляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|String|Описание оповещения.|
|detectionIds|Коллекция String|Набор оповещений, связанных c объектом оповещения (каждое оповещение передается в систему SIEM (управление событиями и информацией в сфере безопасности) отдельной записью).|
|eventDateTime *|DateTimeOffset|Дата и время возникновения события, являющегося триггером для создания оповещения. Тип данных Timestamp предоставляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|feedback|alertFeedback|Отчет специалиста относительно оповещения. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. (поддерживает [обновление](../api/alert_update.md))|
|fileStates|коллекция [fileSecurityState](filesecuritystate.md)|Связанная с безопасностью информация (сгенерированная поставщиком) о состоянии файлов (файла), к которым относится данное оповещение.|
|hostStates|коллекция [hostSecurityState](hostsecuritystate.md)|Связанная с безопасностью информация (сгенерированная поставщиком) о состоянии узлов (узла), к которым относится данное оповещение.|
|id *|String|Генерированный поставщиком GUID (Глобально-уникальный идентификатор)/Уникальный идентификационный код. (только для чтения)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта оповещения. Тип данных Timestamp предоставляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|malwareStates|коллекция [malwareState](malwarestate.md)|Анализ угроз вредоносных программ, связанных с данным оповещением.|
|networkConnections|коллекция [networkConnection](networkconnection.md)|Связанная с безопасностью информация (сгенерированная поставщиком) о состоянии сетевых подключений (сетевого подключения), к которым относится данное оповещение.|
|processes|коллекция [process](process.md)|Связанная с безопасностью информация (сгенерированная поставщиком) о состоянии процессов (процесса), к которым относится данное оповещение.|
|recommendedActions|Коллекция String|Разработчик/поставщика рекомендуется необходимые действия из-за оповещения (например, изоляция компьютера, включить двухфакторную аутентификацию (2FA), восстановить образ узла).|
|registryKeyStates|коллекция [registryKeyState](registrykeystate.md)|Связанная с безопасностью информация (сгенерированная поставщиком) о состоянии разделов реестра (раздела реестра), к которым относится данное оповещение.|
|severity *|alertSeverity|Серьезность оповещения — устанавливается разработчиком/поставщиком. Возможные значения: `unknown`, `informational`, `low`, `medium`, `high`.|
|sourceMaterials|Коллекция String|Гиперссылки (URI) на исходные материалы, связанные с оповещением (например, пользовательский интерфейс поставщика для оповещений или журнал поиска и т.д.)|
|status *|alertStatus|Статус жизненного цикла оповещения (стадия). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`. (поддерживает [обновление](../api/alert_update.md))|
|tags|Коллекция String|Определяемые пользователем метки, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например «HVA», «SAW» и т.д.) (поддерживает [обновление](../api/alert_update.md)).|
|title *|String|Наименование оповещения.|
|triggers|коллекция [alertTrigger](alerttrigger.md)|Связанные с безопасностью сведения об определенных свойствах, которые вызывают оповещения (свойств, указанные в оповещении). Оповещения могут содержать сведения о нескольких пользователей, узлах, файлах, IP-адресах. Это поле отображает, какие свойства вызвали возникновение оповещений.|
|userStates|коллекция [userSecurityState](usersecuritystate.md)|Связанная с безопасностью информация (сгенерированная поставщиком) о состоянии учетных записей пользователей (учетной записи пользователя), к которым относится данное оповещение.|
|vendorInformation *|[securityVendorInformation](securityvendorinformation.md)|Комплексный тип, в котором содержатся сведения о безопасности продуктов и услуг разработчика, поставщика и субпоставщика (например, разработчик = Майкрософт; поставщик = ATP Защитник Windows; субпоставщик = AppLocker).|
|vulnerabilityStates|коллекция [vulnerabilityState](vulnerabilitystate.md)|Анализ угроз одного или более уязвимых мест, связанных с данным оповещением.|
(\* Эти поля носят обязательный характер.)

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->