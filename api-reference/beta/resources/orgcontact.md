---
title: тип ресурса orgContact
description: Ниже этот ресурс представлен в формате JSON.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 09d2897bb2b722cd505402feabc572669c29b623
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014098"
---
# <a name="orgcontact-resource-type"></a>тип ресурса orgContact

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет организационный контакт. Организационные контакты управляются администраторами организации и отличаются от [личных контактов.](contact.md) Кроме того, организационные контакты синхронизируются из локального каталога или из Exchange Online и только для чтения в Microsoft Graph.

Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/orgcontact-delta.md). Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
| ------ | ----------- | ----------- |
| **Контакты организации** |
| [Список организационных контактов](../api/orgcontact-list.md) | [коллекция orgContact](orgcontact.md) | Список свойств организационных контактов. |
| [Получить организационный контакт](../api/orgcontact-get.md) | [orgContact](orgcontact.md) | Чтение свойств и связей объекта orgContact. |
| **Иерархия организации** |
| [Получение имени руководителя](../api/orgcontact-get-manager.md) | [directoryObject](directoryobject.md) | Получите диспетчера контакта. |
| [Получение transitiveReports](../api/orgcontact-get-transitivereports.md) | Целое число | Получите количество транзитных отчетов для контакта с организацией из свойства навигации transitiveReports. |
| [Список directReports](../api/orgcontact-list-directreports.md) | Коллекция [directoryObject](directoryobject.md) | Список прямых отчетов контакта. |
| [Список memberOf](../api/orgcontact-list-memberof.md) | Коллекция [directoryObject](directoryobject.md) | Получите коллекцию объектов memberOf. |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | Коллекция строк | Проверка членства в группе. |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | Коллекция строк | Верни все группы, в которые входит указанный контакт. |
| [checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | Коллекция String | Проверьте членство в группах, административных подразделениях и ролях каталогов. |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md) | Коллекция строк | Получите список ролей групп, административных подразделений и каталогов, в которые входит контактная группа. |

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#organizational-contacts-properties).

| Свойство | Тип | Описание |
| -------- | ---- | ----------- |
| addresses | [коллекция physicalOfficeAddress](physicalofficeaddress.md) | Почтовые адреса для этого организационного контакта. Пока у контакта может быть только один физический адрес. |
| CompanyName | String | Имя компании, к которую принадлежит этот организационный контакт. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| department | String | Имя отдела, в котором работает контакт. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| displayName | String | Отображение имени для этого организационного контакта. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`), `$search` и `$orderBy`.  |
| givenName | String | Имя для этого организационного контакта. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).  |
| id | String | Уникальный идентификатор для этого организационного контакта. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| jobTitle; | String | Название задания для этого организационного контакта. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| почта; | String | Адрес SMTP для контакта, например, "jeff@contoso.onmicrosoft.com". Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| mailNickname | String | Псевдоним электронной почты (часть адреса электронной почты, предварительно ожидающих символ @) для этого организационного контакта. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| onPremisesLastSyncDateTime | DateTimeOffset | Дата и время последней синхронизации этого организационного контакта с локальной AD. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
| onPremisesProvisioningErrors | Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md) | Список ошибок в обеспечении синхронизации для этого организационного контакта. Поддерживает `$filter` (`eq`, `not`). |
| onPremisesSyncEnabled | Логический | **верно,** если этот объект синхронизирован из локального каталога; **false,** если этот объект был первоначально синхронизирован из локального каталога, но больше не синхронизирован и теперь освоен в Exchange; **null,** если этот объект никогда не был синхронизирован из локального каталога (по умолчанию). <br/> <br/>Поддерживает `$filter` (`eq`, `ne`, `not`, `in` и `eq` для значений `null`). |
| phones | Коллекция [phone](phone.md) | Список телефонов для этого организационного контакта. Телефон могут быть мобильными, бизнес-и бизнесфаксами. Только один из каждого типа может присутствовать в коллекции. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| proxyAddresses | Коллекция строк | Например: SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com". Для выражений фильтра в случае многозначных свойств требуется оператор **any**. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`). |
| surname | String | Фамилия для этого организационного контакта. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`и `eq` для значений `null`). |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| directReports | Коллекция [directoryObject](directoryobject.md) | Прямые отчеты контакта. (Пользователи и контакты с свойством диспетчера, заданной для этого контакта.) Только для чтения. Допускается значение null. Поддерживает `$expand`. |
| manager | [directoryObject](directoryobject.md) | Пользователь или контакт, который является менеджером этого контакта. Только для чтения. Поддерживает `$expand`. |
| memberOf | Коллекция [directoryObject](directoryobject.md) | Группы, в которые входит этот контакт. Только для чтения. Допускается значение null. Поддерживает `$expand`. |
| transitiveReports | Коллекция [directoryObject](directoryobject.md) | Транзитные отчеты для контакта. Только для чтения. |

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
  "@odata.type": "microsoft.graph.orgContact"
}-->

``` json
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
