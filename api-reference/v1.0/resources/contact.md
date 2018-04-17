# <a name="contact-resource-type"></a>Тип ресурса contact

Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам с помощью [расширений](../../../concepts/extensibility_overview.md);
- использование [запроса изменений](../../../concepts/delta_query_overview.md) для отслеживания добавочных дополнений, удалений и обновлений благодаря функции [delta](../api/contact_delta.md).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение контакта](../api/contact_get.md) | [contact](contact.md) |Считывание свойств и отношений объекта contact.|
|[Создание](../api/user_post_contacts.md) | [contact](contact.md) |Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.|
|[Обновление](../api/contact_update.md) | [contact](contact.md) |Обновление объекта contact. |
|[Удаление](../api/contact_delete.md) | Нет |Удаление объекта contact. |
|[delta](../api/contact_delta.md)|Коллекция [contact](contact.md)| Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](../../../concepts/extensibility_schema_groups.md) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[contact](contact.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.   |
|[Получение контакта с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [contact](contact.md) | Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [contact](contact.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.  |
|[Получение контакта с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [contact](contact.md) | Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assistantName|String|Имя помощника контакта.|
|birthday|DateTimeOffset|Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|businessAddress|[PhysicalAddress](physicaladdress.md)|Рабочий адрес контакта.|
|businessHomePage|String|Домашняя страница контакта (рабочая).|
|businessPhones|Коллекция String|Рабочие номера телефонов контакта.|
|categories|Коллекция String|Категории, связанные с контактом.|
|changeKey|Строка|Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|children|Коллекция String|Имена детей контакта.|
|companyName|String|Название компании контакта.|
|createdDateTime|DateTimeOffset|Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|отделу;|String|Отдел контакта.|
|displayName|String|Отображаемое имя контакта.|
|emailAddresses|Коллекция [EmailAddress](emailaddress.md)|Электронные адреса контакта.|
|flag|[followUpFlag](followupflag.md)|Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения для сообщения.|
|fileAs|String|Имя, под которым хранится контакт.|
|generation|String|Поколение контакта.|
|givenName|String|Имя контакта.|
|homeAddress|[PhysicalAddress](physicaladdress.md)|Домашний адрес контакта.|
|homePhones|Коллекция String|Номера домашних телефонов контакта.|
|id|String|Уникальный идентификатор контакта. Только для чтения.|
|imAddresses|Коллекция String|Адреса контакта для обмена мгновенными сообщениями.|
|initials|String|Инициалы контакта.|
|jobTitle|String|Должность контакта.|
|lastModifiedDateTime|DateTimeOffset|Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|manager|String|Имя руководителя контакта.
|middleName|String|Отчество контакта.|
|mobilePhone|String|Номер мобильного телефона контакта.|
|nickName|String|Псевдоним контакта.|
|officeLocation|String|Расположение офиса контакта.|
|otherAddress|[PhysicalAddress](physicaladdress.md)|Другие адреса контакта.|
|parentFolderId|String|Идентификатор родительской папки контакта.|
|personalNotes|String|Заметки пользователя о контакте.|
|profession|String|Профессия контакта.|
|spouseName|String|Имя супруга или супруги контакта.|
|surname|String|Фамилия контакта.|
|title|String|Звание контакта.|
|yomiCompanyName|String|Название компании контакта, записанное так, как оно звучит по-японски.|
|yomiGivenName|String|Имя контакта, записанное так, как оно звучит по-японски.|
|yomiSurname|String|Фамилия контакта, записанная так, как она звучит по-японски.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для контакта. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.|
|Фотография
|[profilePhoto](profilephoto.md)| Необязательное фото контакта. Можно получить или задать фото для контакта.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью разностного запроса](../../../concepts/delta_query_overview.md)
- [Получение добавочных изменений сообщений в папке](../../../concepts/delta_query_messages.md)
- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](../../../concepts/extensibility_open_users.md)
- [Добавление пользовательских данных в группы с помощью расширений схемы](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
