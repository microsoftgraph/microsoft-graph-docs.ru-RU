---
title: тип ресурса orgContact
description: Представляет организационный контакт
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 05a78598cb249d203510674ac96b2dd69d236e26
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721546"
---
# <a name="orgcontact-resource-type"></a>тип ресурса orgContact

Пространство имен: microsoft.graph

Представляет организационный контакт. Организационные контакты управляются администраторами организации и отличаются от [личных контактов.](contact.md) Кроме того, организационные контакты синхронизируются из локального каталога или из Exchange Online и являются только для чтения.

Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/orgcontact-delta.md).

## <a name="methods"></a>Методы

| Метод                                                                  | Возвращаемый тип                                      | Описание                                                                                                                 |
|:------------------------------------------------------------------------|:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------|
| [Список организационных контактов](../api/orgcontact-list.md)               | [orgContact](orgcontact.md)                      | Список свойств организационных контактов.                                                                                 |
| [Получить организационный контакт](../api/orgcontact-get.md)                  | [orgContact](orgcontact.md)                      | Чтение свойств и связей организационного контакта.                                                             |
| [Получение имени руководителя](../api/orgcontact-get-manager.md)                         | [directoryObject](directoryobject.md)            | Получите менеджера контактной организации.                                                                                   |
| [Список directReports](../api/orgcontact-list-directreports.md)           | Коллекция [directoryObject](directoryobject.md) | Список прямых отчетов контактов организации.                                                                           |
| [Перечисление memberOf](../api/orgcontact-list-memberof.md)                     | Коллекция [directoryObject](directoryobject.md) | Список групп, в которые входит организационный контакт.                                                                   |
| [Список transitiveMemberOf](../api/orgcontact-list-transitivememberof.md) | Коллекция [directoryObject](directoryobject.md) | Список групп, в которые входит организационный контакт, в том числе группы, в которых вложен организационный контакт. |
| [checkMemberGroups](../api/orgcontact-checkmembergroups.md)             | Коллекция String                                | Проверка членства в группе.                                                                                                 |
| [getMemberGroups](../api/orgcontact-getmembergroups.md)                 | Коллекция String                                | Верни все группы, в которые входит указанный организационный контакт.                                             |
| [getMemberObjects](../api/orgcontact-getmemberobjects.md)               | Коллекция String                                | Возвращает список directoryObjects, в который входит организационный контакт.                                               |

## <a name="properties"></a>Свойства

| Свойство                     | Тип                                                                     | Описание                                                                                                                                                                                                                                                                                |
|:-----------------------------|:-------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| addresses                    | [коллекция physicalOfficeAddress](physicalofficeaddress.md)             | Почтовые адреса для этого организационного контакта. Пока у контакта может быть только один физический адрес.                                                                                                                                                                                    |
| companyName                  | String                                                                   | Имя компании, к которую принадлежит этот организационный контакт.                                                                                                                                                                                                                            |
| department                   | String                                                                   | Имя отдела, в котором работает контакт.                                                                                                                                                                                                                                    |
| displayName                  | String                                                                   | Отображение имени для этого организационного контакта.                                                                                                                                                                                                                                              |
| givenName;                    | String                                                                   | Имя для этого организационного контакта.                                                                                                                                                                                                                                                |
| id                           | String                                                                   | Уникальный идентификатор для этого организационного контакта.                                                                                                                                                                                                                                         |
| jobTitle;                     | String                                                                   | Название задания для этого организационного контакта.                                                                                                                                                                                                                                                 |
| mail                         | String                                                                   | Адрес SMTP для контакта, например, "jeff@contoso.onmicrosoft.com".                                                                                                                                                                                                             |
| mailNickname                 | String                                                                   | Псевдоним электронной почты (часть адреса электронной почты, предварительно ожидающих символ @) для этого организационного контакта.                                                                                                                                                                                           |
| onPremisesLastSyncDateTime   | DateTimeOffset                                                           | Дата и время последней синхронизации этого организационного контакта с локальной AD. Эта информация о дате и времени использует формат ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.                            |
| onPremisesProvisioningErrors | Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md) | Список ошибок в обеспечении синхронизации для этого организационного контакта.                                                                                                                                                                                                           |
| onPremisesSyncEnabled        | Логический                                                                  | **верно,** если этот объект синхронизирован из локального каталога; **false,** если этот объект был первоначально синхронизирован из локального каталога, но больше не синхронизирован и теперь освоен в Exchange; **null,** если этот объект никогда не был синхронизирован из локального каталога (по умолчанию). |
| phones                       | Коллекция [phone](phone.md)                                             | Список телефонов для этого организационного контакта. Типы телефонов могут быть мобильными, бизнес и businessFax. Только один из каждого типа может присутствовать в коллекции.                                                                                                                         |
| proxyAddresses               | Коллекция String                                                        | Например: SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com". Для выражений фильтра в случае многозначных свойств требуется оператор **any**. Поддерживает \$ фильтр.                                                                                                                |
| surname                      | String                                                                   | Фамилия для этого организационного контакта.                                                                                                                                                                                                                                                 |

## <a name="relationships"></a>Связи

| Связь       | Тип                                             | Описание                                                                                                                        |
|:-------------------|:-------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------|
| directReports      | Коллекция [directoryObject](directoryobject.md) | Прямые отчеты контакта. (Пользователи и контакты с свойством диспетчера, заданной для этого контакта.)  Только для чтения. Допускается значение null. |
| manager            | [directoryObject](directoryobject.md)            | Пользователь или контакт, который является менеджером этого контакта. Только для чтения.                                                                     |
| memberOf           | Коллекция [directoryObject](directoryobject.md) | Группы, в которые входит этот контакт. Только для чтения. Допускается значение null.                                                                      |
| transitiveMemberOf | Коллекция [directoryObject](directoryobject.md) | Группы, в которые этот контакт входит, в том числе группы, вложенные в контакт. Только для чтения. Допускается значение null.                   |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
{
  "addresses": [{"@odata.type": "microsoft.graph.physicalOfficeAddress"}],
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "string (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "proxyAddresses": ["string"],
  "surname": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

