---
title: Тип ресурса orgContact
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01f606e8fb1f6ae51608853eed3bc39e0ec124df
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508687"
---
# <a name="orgcontact-resource-type"></a>Тип ресурса orgContact

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение orgContact](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |Чтение свойства и связи объекта orgContact.|
|[Получение manager](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| Получите диспетчера контактов.|
|[Список directReports](../api/orgcontact-list-directreports.md) |Коллекция [directoryObject](directoryobject.md)| Список контактов прямые отчеты.|
|[Перечисление memberOf](../api/orgcontact-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получите коллекцию объектов член групп.|
|[Delete](../api/orgcontact-delete.md) | Нет |Удалите объект orgContact. |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|Коллекция String| Проверьте наличие членства в группе. |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|Коллекция String| Возвращает все группы, принадлежит указанный контакт. |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|Коллекция String| Возвращает список directoryObjects, которому контакт. |

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| addresses                    | [physicalOfficeAddress](physicalofficeaddress.md)            | Почтовые адреса для этого контакта организации. В данный момент контакт может иметь только один физический адрес. |
| companyName                  | String                                                    | Имя компании, принадлежащих организации контакта.                                                                                                                                                                                                                                                                                                                 |
| отделу;                   | String                                                     | Имя для отдела, в котором работает.                                                                                                                                                                                                                                                                                                                                |
| displayName                  | String                                                     | Отображаемое имя для этого контакта организации.                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | Имя для этого контакта организации.                                                                                                                                                                                                                                                                                                                                     |
| id                           | Строка                                                     | Уникальный идентификатор для этого контакта организации.                                                                                                                                                                                                                                                                                                                             |
| imAddresses                  | Коллекция String                          | Список адресов обмена мгновенными Сообщениями для этого контакта организации. В данный момент контакт может иметь только один адрес SIP.                                                                                                                                                                                                                        |
| jobTitle                     | String                                                     | Должность для этого контакта организации.                                                                                                                                                                                                                                                                                                                                      |
|mail|String| SMTP-адрес контакта, например, «jeff@contoso.onmicrosoft.com». |
| mailNickname                 | String                                                     | Псевдоним электронной почты (часть адреса электронной почты предварительно ожидающие символа @) для этого контакта организации.                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | Дата и время последнего организационной контакта синхронизируются из локальной AD. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь UTC 1 января 2014 г будет выглядеть следующим образом: "2014-01-01T00:00:00Z".   |
| onPremisesProvisioningErrors |Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md)       | Список любого синхронизации подготовки ошибки для этого контакта организации.                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Логическое|**значение true,** Если этот объект синхронизируется в локальном каталоге; **значение false,** Если этот объект исходно синхронизирован из локального каталога, но более не синхронизирован и теперь создаются в Exchange; **значение null,** Если этот объект никогда не синхронизированы из локального каталога (по умолчанию).|
| phones                       | Коллекция [phone](phone.md)                            | Список телефонов для этого контакта организации. Типы телефона может быть mobile, бизнеса и рабочий. Только один из каждого типа никогда не могут быть представлены в коллекции.                                                                                                                       |
| proxyAddresses               | Коллекция String                                         | Например: ["SMTP: bob@contoso.com», «smtp: bob@sales.contoso.com»]. Для выражений фильтра в случае многозначных свойств требуется оператор **any**. Поддерживает параметр $filter.                                                                                                                                                                               |
| surname                      | String                                                     | Фамилия для этого контакта организации.                          |

## <a name="relationships"></a>Отношения

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|directReports|Коллекция [directoryObject](directoryobject.md)| Прямые отчеты контакта. (Пользователей и контактов, у диспетчера свойство значение для этого контакта.)  Только для чтения. Допускается значение null.|
|manager|[directoryObject](directoryobject.md)| Пользователь или контакт, менеджер по этому контакту. Только для чтения.|
|memberOf|Коллекция [directoryObject](directoryobject.md)| Группы, которым принадлежит этот контакт. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/orgcontact.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
