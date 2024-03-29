---
title: Тип ресурса contact
description: Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8833fca292efffc631f190b0f9e201d5f0d02929
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014035"
---
# <a name="contact-resource-type"></a>Тип ресурса contact

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контакт — элемент в Outlook, в котором вы можете упорядочить и хранить сведения о людях и организациях, с которыми поддерживаете связь. Контакты содержатся в папках контактов.

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/contact-delta.md)).

## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение контакта](../api/contact-get.md) | [contact](contact.md) |Считывание свойств и отношений объекта contact.|
|[Создание](../api/user-post-contacts.md) | [contact](contact.md) |Добавление контакта в корневую папку с контактами или конечную точку контактов другой папки с контактами.|
|[Обновление](../api/contact-update.md) | [contact](contact.md) |Обновление объекта contact. |
|[Удаление](../api/contact-delete.md) | Нет |Удаление объекта contact. |
|[delta](../api/contact-delta.md)|Коллекция [contact](contact.md)| Получение набора контактов, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[contact](contact.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем контакте.   |
|[Получение контакта с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [contact](contact.md) | Получение контактов, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [contact](contact.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем контакте.  |
|[Получение контакта с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [contact](contact.md) | Получение контакта, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assistantName|String|Имя помощника контакта.|
|birthday|DateTimeOffset|Дата рождения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|categories|Коллекция String|Категории, связанные с контактом. Каждая категория соответствует свойству **displayName** объекта [outlookCategory](outlookcategory.md), определенного для пользователя.|
|changeKey|Строка|Указывает версию контакта. При каждом изменении контакта также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|children|Коллекция String|Имена детей контакта.|
|companyName|String|Название компании контакта.|
|createdDateTime|DateTimeOffset|Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|department|String|Отдел контакта.|
|displayName|String|Отображаемое имя контакта. Отображаемое имя можно указать в операции [создания](../api/user-post-contacts.md) или [обновления](../api/contact-update.md). Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName. Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию [обновления](../api/contact-update.md).|
|emailAddresses|[коллекция typedEmailAddress](typedemailaddress.md)|Электронные адреса контакта.|
|fileAs|String|Имя, под которым хранится контакт.|
|flag|[followupFlag](followupflag.md)|Значение флага, которое указывает состояние, дату начала, дату выполнения или дату завершения контакта. |
|gender |Строка |Пол контакта. |
|generation|String|Поколение контакта.|
|givenName|String|Имя контакта.|
|id|Строка| Уникальный идентификатор для контакта. [!INCLUDE [outlook-beta-id](../../includes/outlook-immutable-id.md)] Только для чтения. |
|imAddresses|Коллекция String|Адреса контакта для обмена мгновенными сообщениями.|
|initials|String|Инициалы контакта.|
|jobTitle|String|Должность контакта.|
|lastModifiedDateTime|DateTimeOffset|Время изменения контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|manager|String|Имя руководителя контакта.
|middleName|String|Отчество контакта.|
|nickName|String|Псевдоним контакта.|
|officeLocation|String|Расположение офиса контакта.|
|parentFolderId|String|Идентификатор родительской папки контакта.|
|personalNotes|String|Заметки пользователя о контакте.|
|phones |Коллекция [phone](phone.md) |Телефон, связанные с контактом, например домашний телефон, мобильный телефон и бизнес-телефон. |
|postalAddresses |[коллекция physicalAddress](physicaladdress.md) |Адреса, связанные с контактом, например домашний адрес и бизнес-адрес. |
|profession|String|Профессия контакта.|
|spouseName|String|Имя супруга или супруги контакта.|
|surname|String|Фамилия контакта.|
|title|String|Звание контакта.|
|websites |Коллекция [website](website.md)|Веб-сайты, связанные с контактом. |
|weddingAnniversary |Дата |Годовщина свадьбы контакта. |
|yomiCompanyName|String|Название компании контакта, записанное так, как оно звучит по-японски.|
|yomiGivenName|String|Имя контакта, записанное так, как оно звучит по-японски.|
|yomiSurname|String|Фамилия контакта, записанная так, как она звучит по-японски.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для контакта. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для контакта. Только для чтения. Допускается значение null.|
|Фотография
|[photo](profilephoto.md)| Необязательное фото контакта. Можно получить или задать фото для контакта.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для контакта. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.typedEmailAddress"}],
  "fileAs": "string",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "gender": "string",
  "generation": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "nickName": "string",
  "officeLocation": "string",
  "parentFolderId": "string",
  "personalNotes": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.physicalAddress"}],
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "weddingAnniversary": "date",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string"
}
```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)
- [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages)
- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


