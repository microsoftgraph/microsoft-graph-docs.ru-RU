---
title: Тип ресурса orgContact
description: Представляет контактное лицо организации
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: cd5a39f35465ca001eece05a0ff1fabb5852418a
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461326"
---
# <a name="orgcontact-resource-type"></a>Тип ресурса orgContact

Пространство имен: microsoft.graph

Представляет контакт организации. Контакты организации управляются администраторами организации и отличаются от [личных контактов](contact.md). Кроме того, контакты организации синхронизируются из локальных каталогов или из Exchange Online и доступны только для чтения в Microsoft Graph.

Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/orgcontact-delta.md). Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

## <a name="methods"></a>Методы

| Метод                                                                  | Возвращаемый тип                                      | Описание                                                                                                                 |
|:------------------------------------------------------------------------|:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------|
| **Контакты организации** |
| [Перечисление контактов организации](../api/orgcontact-list.md)               | [orgContact](orgcontact.md)                      | Список свойств контактов организации.                                                                                 |
| [Получение контакта организации](../api/orgcontact-get.md)                  | [orgContact](orgcontact.md)                      | Чтение свойств и связей контактов организации.                                                             |
| **Иерархия организации** |
| [Получение имени руководителя](../api/orgcontact-get-manager.md)                         | [directoryObject](directoryobject.md)            | Получите руководителя контактного лица организации.                                                                                   |
| [Список directReports](../api/orgcontact-list-directreports.md)           | Коллекция [directoryObject](directoryobject.md) | Вывод списка прямых отчетов контактного лица организации.                                                                           |
| [Список memberOf](../api/orgcontact-list-memberof.md)                     | Коллекция [directoryObject](directoryobject.md) | Перечисление групп, участником в которые является контакт организации.                                                                   |
| [Перечисление transitiveMemberOf](../api/orgcontact-list-transitivememberof.md) | Коллекция [directoryObject](directoryobject.md) | Список групп, участником которых является контакт организации, включая группы, в которые вложен контакт организации. |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md)             | Коллекция String                                | Проверьте членство в группе.                                                                                                 |
| [getMemberGroups](../api/directoryobject-getmembergroups.md)                 | Коллекция String                                | Возвращает все группы, участником которых является указанный контакт организации.                                             |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md)               | Коллекция String                                | Возвращает список объектов directoryObjects, в которые входит контакт организации.                                               |

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#organizational-contacts-properties).

| Свойство                     | Тип                                                                     | Описание                                                                                                                                                                                                                                                                                                                        |
|:-----------------------------|:-------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Адреса                    | [Коллекция physicalOfficeAddress](physicalofficeaddress.md)             | Почтовые адреса для этого контакта организации. На данный момент контакт может иметь только один физический адрес.                                                                                                                                                                                                                            |
| CompanyName                  | String                                                                   | Имя компании, к которой принадлежит этот контакт организации.  Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям).                                                                                                                                                                                          |
| department                   | String                                                                   | Имя отдела, в котором работает контакт.  Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).                                                                                                                                                                                                   |
| displayName                  | Строка                                                                   | Отображаемое имя для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`), `$search` и `$orderBy`.                                                                                                                                                                                   |
| givenName                    | String                                                                   | Имя для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).                                                                                                                                                                                                                |
| id                           | String                                                                   | Уникальный идентификатор для этого контакта организации.  Поддерживает `$filter` (`eq`, `ne`, `not`, `in`).                                                                                                                                                                                                                                  |
| jobTitle;                     | String                                                                   | Должность для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).                                                                                                                                                                                                                 |
| почта;                         | String                                                                   | SMTP-адрес контакта, например "jeff@contoso.onmicrosoft.com". Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).                                                                                                                                                                             |
| mailNickname                 | String                                                                   | Псевдоним электронной почты (часть адреса электронной почты перед ожиданием символа @) для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).                                                                                                                                                           |
| onPremisesLastSyncDateTime   | DateTimeOffset                                                           | Дата и время последней синхронизации этого контакта организации из локальной службы AD. Эти сведения о дате и времени используют формат ISO 8601 и всегда имеют время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`).                             |
| onPremisesProvisioningErrors | Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md) | Список ошибок подготовки синхронизации для данного контакта организации. Поддерживает `$filter` (`eq`, `not`).                                                                                                                                                                                                                 |
| onPremisesSyncEnabled        | Boolean                                                                  | `true`Значение , если этот объект синхронизирован из локального каталога; `false` Значение , если этот объект изначально был синхронизирован из локального каталога, но больше не синхронизирован и теперь находится в Exchange; `null` если этот объект никогда не синхронизирован из локального каталога (по умолчанию). <br/> <br/> Поддерживает `$filter` (`eq`, `ne`, `not`, `in` и `eq` по `null` значениям). |
| phones                       | Коллекция [phone](phone.md)                                             | Список телефонов для этого контакта организации. Телефон типы могут быть мобильными, бизнес-и бизнес-факсами. В коллекции может присутствовать только один тип.                                                                                                                                                                 |
| proxyAddresses               | Коллекция String                                                        | Например, "SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com". Для выражений фильтра в случае многозначных свойств требуется оператор **any**. `$filter` Поддерживает (`eq`, `not`, `ge`, `le`, и `startsWith`подсчитывает пустые коллекции).                                                                                                              |
| surname                      | String                                                                   | Фамилия этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).                                                                                                                                                                                                                 |

## <a name="relationships"></a>Отношения

| Связь       | Тип                                             | Описание                                                                                                                                            |
|:-------------------|:-------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------|
| directReports      | Коллекция [directoryObject](directoryobject.md) | Прямые отчеты контакта. (Пользователи и контакты, для которых свойству руководителя задано значение этого контакта.)  Только для чтения. Допускается значение null. Поддерживает `$expand`. |
| manager            | [directoryObject](directoryobject.md)            | Пользователь или контакт, который является руководителем этого контакта. Только для чтения. Поддерживает `$expand`.                                                                     |
| memberOf           | Коллекция [directoryObject](directoryobject.md) | Группы, участником которых является этот контакт. Только для чтения. Допускается значение null. Поддерживает `$expand`.                                                                      |
| transitiveMemberOf | Коллекция [directoryObject](directoryobject.md) | Группы, в которые входит этот контакт, включая группы, в которые он вложен. Только для чтения. Допускается значение null.                                       |

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

