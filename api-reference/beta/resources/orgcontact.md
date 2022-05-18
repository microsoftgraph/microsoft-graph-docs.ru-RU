---
title: Тип ресурса orgContact
description: Ниже этот ресурс представлен в формате JSON.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5d8386244faac145508ef8a1c1fb0da39d7445bc
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461396"
---
# <a name="orgcontact-resource-type"></a>Тип ресурса orgContact

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контакт организации. Контакты организации управляются администраторами организации и отличаются от [личных контактов](contact.md). Кроме того, контакты организации синхронизируются из локальных каталогов или из Exchange Online и доступны только для чтения в Microsoft Graph.

Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/orgcontact-delta.md). Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
| ------ | ----------- | ----------- |
| **Контакты организации** |
| [Перечисление контактов организации](../api/orgcontact-list.md) | [Коллекция orgContact](orgcontact.md) | Список свойств контактов организации. |
| [Получение контакта организации](../api/orgcontact-get.md) | [orgContact](orgcontact.md) | Чтение свойств и связей объекта orgContact. |
| **Иерархия организации** |
| [Получение имени руководителя](../api/orgcontact-get-manager.md) | [directoryObject](directoryobject.md) | Получите руководителя контакта. |
| [Получение transitiveReports](../api/orgcontact-get-transitivereports.md) | Целое число | Получение количества транзитивных отчетов для контакта организации из свойства навигации transitiveReports. |
| [Список directReports](../api/orgcontact-list-directreports.md) | Коллекция [directoryObject](directoryobject.md) | Вывод списка прямых отчетов контакта. |
| [Список memberOf](../api/orgcontact-list-memberof.md) | Коллекция [directoryObject](directoryobject.md) | Получение коллекции объектов memberOf. |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | Коллекция String | Проверьте членство в группе. |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | Коллекция String | Возвращает все группы, участником которых является указанный контакт. |
| [checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | Коллекция String | Проверьте членство в группах, административных единицах и ролях каталогов. |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md) | Коллекция String | Получение списка групп, административных единиц и ролей каталогов, участником в которые является контакт. |

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#organizational-contacts-properties).

| Свойство | Тип | Описание |
| -------- | ---- | ----------- |
| Адреса | [Коллекция physicalOfficeAddress](physicalofficeaddress.md) | Почтовые адреса для этого контакта организации. На данный момент контакт может иметь только один физический адрес. |
| CompanyName | String | Название компании, к которой принадлежит этот контакт организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| department | String | Имя отдела, в котором работает контакт. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| displayName | String | Отображаемое имя для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`), `$search` и `$orderBy`.  |
| givenName | String | Имя для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`).  |
| id | String | Уникальный идентификатор для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| jobTitle; | String | Должность для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| почта; | String | SMTP-адрес контакта, например "jeff@contoso.onmicrosoft.com". Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| mailNickname | String | Псевдоним электронной почты (часть адреса электронной почты перед ожиданием символа @) для этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`). |
| onPremisesLastSyncDateTime | DateTimeOffset | Дата и время последней синхронизации этого контакта организации из локальной службы AD. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
| onPremisesProvisioningErrors | Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md) | Список ошибок подготовки синхронизации для данного контакта организации. Поддерживает `$filter` (`eq`, `not`). |
| onPremisesSyncEnabled | Boolean | **Значение true**, если этот объект синхронизирован из локального каталога; **значение false**, если этот объект изначально был синхронизирован из локального каталога, но больше не синхронизирован и теперь Exchange; **Значение NULL**, если этот объект никогда не был синхронизирован из локального каталога (по умолчанию). <br/> <br/>Поддерживает `$filter` (`eq`, `ne`, `not`, `in` и `eq` по `null` значениям). |
| phones | Коллекция [phone](phone.md) | Список телефонов для этого контакта организации. Телефон типы могут быть мобильными, бизнес-и бизнес-факсами. В коллекции может присутствовать только один тип. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
| proxyAddresses | Коллекция String | Например, "SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com". Для выражений фильтра в случае многозначных свойств требуется оператор **any**. `$filter` Поддерживает (`eq`, `not`, `ge`, `le`, и `startsWith`подсчитывает пустые коллекции). |
| surname | String | Фамилия этого контакта организации. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`и `eq` для значений `null`). |

## <a name="relationships"></a>Отношения

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| directReports | Коллекция [directoryObject](directoryobject.md) | Прямые отчеты контакта. (Пользователи и контакты, для которых свойству руководителя задано значение этого контакта.) Только для чтения. Допускается значение null. Поддерживает `$expand`. |
| manager | [directoryObject](directoryobject.md) | Пользователь или контакт, который является руководителем этого контакта. Только для чтения. Поддерживает `$expand`. |
| memberOf | Коллекция [directoryObject](directoryobject.md) | Группы, участником которых является этот контакт. Только для чтения. Допускается значение null. Поддерживает `$expand`. |
| transitiveReports | Коллекция [directoryObject](directoryobject.md) | Транзитивные отчеты для контакта. Только для чтения. |

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
