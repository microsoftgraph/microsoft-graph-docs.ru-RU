---
title: тип ресурса orgContact
description: Представляет организационный контакт
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 983ed1b95df3c96e86626166df87d6f6973c234a
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60942550"
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
| [Список memberOf](../api/orgcontact-list-memberof.md)                     | Коллекция [directoryObject](directoryobject.md) | Список групп, в которые входит организационный контакт.                                                                   |
| [Список transitiveMemberOf](../api/orgcontact-list-transitivememberof.md) | Коллекция [directoryObject](directoryobject.md) | Список групп, в которые входит организационный контакт, в том числе группы, в которых вложен организационный контакт. |
| [checkMemberGroups](../api/orgcontact-checkmembergroups.md)             | Коллекция String                                | Проверка членства в группе.                                                                                                 |
| [getMemberGroups](../api/orgcontact-getmembergroups.md)                 | Коллекция String                                | Верни все группы, в которые входит указанный организационный контакт.                                             |
| [getMemberObjects](../api/orgcontact-getmemberobjects.md)               | Коллекция String                                | Возвращает список directoryObjects, в который входит организационный контакт.                                               |

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

| Свойство                     | Тип                                                                     | Описание                                                                                                                                                                                                                                                                                                                        |
|:-----------------------------|:-------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| адреса                    | [коллекция physicalOfficeAddress](physicalofficeaddress.md)             | Почтовые адреса для этого организационного контакта. Пока у контакта может быть только один физический адрес.                                                                                                                                                                                                                            |
| companyName                  | String                                                                   | Имя компании, к которой принадлежит этот организационный контакт.  Поддерживает `$filter` `eq` `ne` (, `NOT` , `ge` , , , , и по `le` `in` `startsWith` `eq` `null` значениям).                                                                                                                                                                                          |
| department                   | String                                                                   | Имя отдела, в котором работает контакт.  Поддерживает `$filter` `eq` `ne` (, `NOT` , `ge` , , , , и по `le` `in` `startsWith` `eq` `null` значениям).                                                                                                                                                                                                   |
| displayName                  | String                                                                   | Отображение имени для этого организационного контакта. Поддерживает `$filter` (, , , , , , , и по `eq` `ne` `NOT` `ge` `le` `in` `startsWith` `eq` `null` значениям), `$search` и `$orderBy` .                                                                                                                                                                                   |
| givenName                    | String                                                                   | Имя для этого организационного контакта. Поддерживает `$filter` `eq` `ne` (, `NOT` , `ge` , , , , и по `le` `in` `startsWith` `eq` `null` значениям).                                                                                                                                                                                                                |
| id                           | String                                                                   | Уникальный идентификатор для этого организационного контакта.  Поддерживает `$filter` (`eq`, `ne`, `NOT`, `in`).                                                                                                                                                                                                                                  |
| jobTitle;                     | String                                                                   | Название задания для этого организационного контакта. Поддерживает `$filter` `eq` `ne` (, `NOT` , `ge` , , , , и по `le` `in` `startsWith` `eq` `null` значениям).                                                                                                                                                                                                                 |
| почта;                         | String                                                                   | Адрес SMTP для контакта, например, "jeff@contoso.onmicrosoft.com". Поддерживает `$filter` `eq` `ne` (, `NOT` , `ge` , , , , и по `le` `in` `startsWith` `eq` `null` значениям).                                                                                                                                                                             |
| mailNickname                 | String                                                                   | Псевдоним электронной почты (часть адреса электронной почты, предварительно ожидающих символ @) для этого организационного контакта. Поддерживает `$filter` `eq` `ne` (, `NOT` , `ge` , , , , и по `le` `in` `startsWith` `eq` `null` значениям).                                                                                                                                                           |
| onPremisesLastSyncDateTime   | DateTimeOffset                                                           | Дата и время последней синхронизации этого организационного контакта с локальной AD. Эта информация о дате и времени использует формат ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`).                             |
| onPremisesProvisioningErrors | Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md) | Список ошибок в обеспечении синхронизации для этого организационного контакта. Поддерживает `$filter` (`eq`, `NOT`).                                                                                                                                                                                                                 |
| onPremisesSyncEnabled        | Логический                                                                  | `true`если этот объект синхронизирован из локального каталога; если этот объект был первоначально синхронизирован из локального каталога, но больше не синхронизирован и теперь освоен в Exchange; если этот объект никогда не синхронизировался из локального каталога `false` `null` (по умолчанию). <br/> <br/> Поддерживает `$filter` `eq` `ne` (, `NOT` , , `in` , и по `eq` `null` значениям). |
| phones                       | Коллекция [phone](phone.md)                                             | Список телефонов для этого организационного контакта. Телефон могут быть мобильными, бизнес-и бизнесфаксами. Только один из каждого типа может присутствовать в коллекции.                                                                                                                                                                 |
| proxyAddresses               | Коллекция String                                                        | Например: SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com". Для выражений фильтра в случае многозначных свойств требуется оператор **any**. Поддерживает `$filter` (`eq`, `NOT`, `ge`, `le`, `startsWith`).                                                                                                               |
| surname                      | String                                                                   | Фамилия для этого организационного контакта. Поддерживает `$filter` `eq` `ne` (, `NOT` , `ge` , , , , и по `le` `in` `startsWith` `eq` `null` значениям).                                                                                                                                                                                                                 |

## <a name="relationships"></a>Связи

| Связь       | Тип                                             | Описание                                                                                                                                            |
|:-------------------|:-------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------|
| directReports      | Коллекция [directoryObject](directoryobject.md) | Прямые отчеты контакта. (Пользователи и контакты с свойством диспетчера, заданной для этого контакта.)  Только для чтения. Допускается значение null. Поддерживает `$expand`. |
| manager            | [directoryObject](directoryobject.md)            | Пользователь или контакт, который является менеджером этого контакта. Только для чтения. Поддерживает `$expand`.                                                                     |
| memberOf           | Коллекция [directoryObject](directoryobject.md) | Группы, в которые входит этот контакт. Только для чтения. Допускается значение null. Поддерживает `$expand`.                                                                      |
| transitiveMemberOf | Коллекция [directoryObject](directoryobject.md) | Группы, в которые этот контакт входит, в том числе группы, вложенные в контакт. Только для чтения. Допускается значение null.                                       |

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

