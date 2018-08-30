# <a name="organization-resource-type"></a>Тип ресурса organization

Представляет клиента Azure Active Directory. Для клиентов поддерживаются только операции чтения и обновления. Создание и удаление не поддерживаются. Наследуется от [directoryObject](directoryobject.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](../../../concepts/extensibility_overview.md).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение организации](../api/organization_get.md) | [organization](organization.md) |Считывание свойств и связей объекта организации.|
|[Обновление](../api/organization_update.md) | [organization](organization.md)  |Обновление объекта организации. Обновлять можно только эти свойства: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** и **privacyProfile**. |
|**Открытые расширения**| | ||**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](../../../concepts/extensibility_schema_groups.md) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства

| Свойство                             | Тип                                                              | Описание                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | Коллекция [assignedPlan](assignedplan.md)                        | Коллекция планов обслуживания, сопоставленных с клиентом. Значение NULL не допускается.                                                                                                                                                                                                            |
| city                                 | String (строка)                                                            | Название города в адресе организации                                                                                                                                                                                                                                        |
| companyLastDirSyncTime               | DateTimeOffset                                                    | Дата и время последней синхронизации клиента с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'` |
| country                              | String (строка)                                                            | Название страны или региона в адресе организации.                                                                                                                                                                                                                              |
| countryLetterCode                    | String (строка)                                                            | Сокращенное название страны или региона для организации.                                                                                                                                                                                                                                     |
| deletionTimestamp                    | DateTimeOffset                                                    | Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`                                                                                     |
| dirSyncEnabled                       | Boolean (логический)                                                           | Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).                        |
| displayName                          | String (строка)                                                            | Отображаемое имя для клиента.                                                                                                                                                                                                                                                     |
| id                                   | String (строка)                                                            | Уникальный идентификатор клиента. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.                                                                                                                                                            |
| marketingNotificationEmails          | Коллекция String                                                 | Значение null не допускается.                                                                                                                                                                                                                                                                        |
| objectType                           | String (строка)                                                            | Строка, которая определяет тип объекта. Для клиентов всегда задается значение Company.                                                                                                                                                                                                 |
| postalCode                           | String (строка)                                                            | Почтовый индекс в адресе организации                                                                                                                                                                                                                                      |
| preferredLanguage                    | String (строка)                                                            | Предпочитаемый язык для организации. Он должен быть представлен в формате ISO 639-1. Пример: ru.                                                                                                                                                                                         |
| privacyProfile                       | [privacyProfile](privacyprofile.md)                               | Профиль конфиденциальности организации.                                                                                                                                                                                                                                              |
| provisionedPlans                     | Коллекция [ProvisionedPlan](provisionedplan.md)                  | Значение null не допускается.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | Коллекция String                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | Коллекция String                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | String (строка)                                                            | Название республики, области или края в адресе организации                                                                                                                                                                                                                                       |
| street                               | String (строка)                                                            | Название улицы в адресе организации                                                                                                                                                                                                                                          |
| technicalNotificationMails           | Коллекция String                                                 | Значение null не допускается.                                                                                                                                                                                                                                                                        |
| telephoneNumber                      | String (строка)                                                            | Номер телефона организации                                                                                                                                                                                                                                                |
| verifiedDomains                      | Коллекция [VerifiedDomain](verifieddomain.md)                    | Коллекция доменов, сопоставленных с этим клиентом. Значение null не допускается.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для организации. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Описание в формате JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "companyLastDirSyncTime": "2018-05-12T13:09:20.111Z",
  "country": "string",
  "countryLetterCode": "string",
  "deletionTimestamp": "2018-05-12T15:37:52.763Z",
  "dirSyncEnabled": true,
  "displayName": "string",
  "id": "string (identifier)",
  "marketingNotificationEmails": ["string"],
  "objectType": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "telephoneNumber": "555-555-6568",
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}

```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](../../../concepts/extensibility_open_users.md)
- [Добавление пользовательских данных в группы с помощью расширений схемы](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'businessPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesLastSyncDateTime' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesSyncEnabled' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationMails' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table."
  ],
  "tocPath": ""
}-->
