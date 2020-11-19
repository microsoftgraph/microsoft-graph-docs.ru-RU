---
title: Тип ресурса orgContact
description: Ниже этот ресурс представлен в формате JSON.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ccd36e9d04a1404bb972694fdb9c2b0d8a5ccc3
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352377"
---
# <a name="orgcontact-resource-type"></a>Тип ресурса orgContact

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет организационный контакт. Организационные контакты управляются администраторами Организации и отличаются от [личных контактов](contact.md). Кроме того, контакты организации синхронизируются из локальных каталогов или из Exchange Online и доступны только для чтения.

Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/orgcontact-delta.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
| ------ | ----------- | ----------- |
| [Список контактов Организации](../api/orgcontact-list.md) | Коллекция [orgContact](orgcontact.md) | Перечисление свойств организационных контактов. |
| [Получение контактного лица Организации](../api/orgcontact-get.md) | [orgContact](orgcontact.md) | Чтение свойств и связей объекта orgContact. |
| [Получение имени руководителя](../api/orgcontact-get-manager.md) | [directoryObject](directoryobject.md) | Получение руководителя контакта. |
| [Список directReports](../api/orgcontact-list-directreports.md) | Коллекция [directoryObject](directoryobject.md) | Перечислите непосредственные отчеты контакта. |
| [Список memberOf](../api/orgcontact-list-memberof.md) | Коллекция [directoryObject](directoryobject.md) | Получение коллекции memberOf Objects. |
| [checkMemberGroups](../api/orgcontact-checkmembergroups.md) | Коллекция строк | Проверьте принадлежность к группе. |
| [getMemberGroups](../api/orgcontact-getmembergroups.md) | Коллекция строк | Возврат всех групп, членом которых является указанный контакт. |
| [getMemberObjects](../api/orgcontact-getmemberobjects.md) | Коллекция строк | Возвращает список Директорйобжектс, членом которых является контакт. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| -------- | ---- | ----------- |
| addresses | Коллекция [фисикалоффицеаддресс](physicalofficeaddress.md) | Почтовые адреса для этого организационного контакта. Теперь контакт может иметь только один физический адрес. |
| companyName | String | Имя компании, к которой принадлежит это Контактное лицо. |
| department | String | Имя отдела, в котором работает контакт. |
| displayName | Строка | Отображаемое имя для этого организационного контакта. |
| givenName | String | Имя для этого организационного контакта. |
| id | Строка | Уникальный идентификатор для этого организационного контакта. |
| jobTitle | String | Должность для этого контакта в Организации. |
| mail | String | SMTP-адрес контакта, например, "jeff@contoso.onmicrosoft.com". |
| mailNickname | String | Псевдоним электронной почты (часть адреса электронной почты, предварительно заданная в параметре @ Symbol) для этого контакта в Организации. |
| onPremisesLastSyncDateTime | DateTimeOffset | Дата и время последней синхронизации этого контакта в организации из локальной службы AD. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| onPremisesProvisioningErrors | Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md) | Список всех ошибок подготовки синхронизации для данного контакта Организации. |
| onPremisesSyncEnabled | Boolean | **значение true** , если объект синхронизирован из локального каталога; **false** , если этот объект изначально был синхронизирован из локального каталога, но больше не синхронизируется и не выполняется в Exchange. **значение NULL** , если объект никогда не был синхронизирован из локального каталога (по умолчанию). |
| phones | Коллекция [phone](phone.md) | Список телефонов для этого контакта в Организации. Типы телефонов могут быть мобильными, рабочими и Бусинессфакс. В коллекции всегда может присутствовать только один из этих типов. |
| proxyAddresses | Коллекция строк | Пример: "SMTP: bob@contoso.com", "SMTP: bob@sales.contoso.com". Для выражений фильтра в случае многозначных свойств требуется оператор **any**. Поддерживает параметр $filter. |
| surname | String | Фамилия для этого организационного контакта. |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| directReports | Коллекция [directoryObject](directoryobject.md) | Прямые отчеты контакта. (К этому контакту присвоено значение "Пользователи" и "Контакты", которому назначено свойство "руководитель"). Только для чтения. Допускается значение null. |
| manager | [directoryObject](directoryobject.md) | Пользователь или контакт, который является руководителем этого контакта. Только для чтения. |
| memberOf | Коллекция [directoryObject](directoryobject.md) | Группы, в которых входит этот контакт. Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Описание в формате JSON

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
