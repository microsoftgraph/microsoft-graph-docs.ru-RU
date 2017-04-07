# <a name="organization-resource-type"></a>Тип ресурса organization

Представляет клиента Azure Active Directory. Для клиентов поддерживаются только операции чтения и обновления. Создание и удаление не поддерживаются. Наследуется от [directoryObject](directoryobject.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Get organization](../api/organization_get.md) | [organization](organization.md) |Считывание свойств и связей объекта организации.|
|[Update](../api/organization_update.md) | [organization](organization.md)  |Обновление объекта организации. (Можно обновлять только свойства **marketingNotificationMails** и **technicalNotificationMails**.) |

## <a name="properties"></a>Свойства

| Свойство                             | Тип                                                              | Описание                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | Коллекция [assignedPlan](assignedplan.md)                        | Коллекция планов обслуживания, сопоставленных с клиентом. Значение null не допускается.                                                                                                                                                                                                            |
| городу;                                 | String                                                            |                                                                                                                                                                                                                                                                                      |
| companyLastDirSyncTime               | DateTimeOffset                                                    | Дата и время последней синхронизации клиента с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
| country                              | String                                                            |                                                                                                                                                                                                                                                                                      |
| countryLetterCode                    | String                                                            |                                                                                                                                                                                                                                                                                      |
| deletionTimestamp                    | DateTimeOffset                                                    | Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.                                                                                     |
| dirSyncEnabled                       | Boolean                                                           | Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).                        |
| displayName                          | String                                                            | Отображаемое имя для клиента.                                                                                                                                                                                                                                                     |
| id                                   | String                                                            | Уникальный идентификатор клиента. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.                                                                                                                                                            |
| marketingNotificationEmails          | Коллекция String                                                 | Значение null не допускается.                                                                                                                                                                                                                                                                        |
| objectType                           | String                                                            | Строка, которая определяет тип объекта. Для клиентов всегда задается значение Company.                                                                                                                                                                                                 |
| postalCode                           | String                                                            |                                                                                                                                                                                                                                                                                      |
| preferredLanguage                    | String                                                            |                                                                                                                                                                                                                                                                                      |
| provisionedPlans                     | Коллекция [ProvisionedPlan](provisionedplan.md)                  | Значение null не допускается.                                                                                                                                                                                                                                                                        |
| provisioningErrors                   | Коллекция ProvisioningError | Значение null не допускается.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | Коллекция String                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | Коллекция String                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | String                                                            |                                                                                                                                                                                                                                                                                      |
| street                               | String                                                            |                                                                                                                                                                                                                                                                                      |
| technicalNotificationMails           | Коллекция String                                                 | Значение null не допускается.                                                                                                                                                                                                                                                                        |
| telephoneNumber                      | String                                                            |                                                                                                                                                                                                                                                                                      |
| verifiedDomains                      | Коллекция [VerifiedDomain](verifieddomain.md)                    | Коллекция доменов, сопоставленных с этим клиентом. Значение null не допускается.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "marketingNotificationEmails": ["string"],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
