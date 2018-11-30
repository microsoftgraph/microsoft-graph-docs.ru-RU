---
title: Тип ресурса orgContact
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: fb0970b2eb973e516761ba1145d66b3af7fdef5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080322"
---
# <a name="orgcontact-resource-type"></a>Тип ресурса orgContact

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

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
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "officeLocation": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "proxyAddresses": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String| Город, в котором расположен контакт. |
|country|String| Страна/регион, в которой находится контакт. |
|department|String| Имя для отдела, в котором работает. |
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).|
|displayName|String| Отображаемое имя для этого контакта. |
|givenName|String| Имя (имя) контакта. |
|jobTitle|String| Название должности контакта. |
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последнего, в котором объект был синхронизирован с локального каталога. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) коллекции| Ошибки при использовании продуктов Майкрософт синхронизации во время подготовки. |
|mail|String| SMTP-адрес контакта, например, «jeff@contoso.onmicrosoft.com». |
|mailNickname|String| Псевдоним почтового контакта. |
|mobilePhone|String| Номер основной мобильного телефона контакта. |
|id|String| Уникальный идентификатор для этого контакта. Только для чтения.|
|officeLocation|String| Расположение комнаты на месте контакта бизнеса. |
|postalCode|String| Почтовый индекс для почтовый адрес контакта. Почтовый индекс для контакта страны или региона. В Соединенных Штатах Америки этот атрибут содержит ПОЧТОВЫЙ индекс. |
|proxyAddresses|Коллекция String| Например: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **любой** оператор для фильтра выражений на многозначные свойства. Только для чтения. Значение NULL не допускается. Поддерживает параметр $filter. |
|state|String| Область или край в адрес контакта. |
|streetAddress|String| Почтовый адрес контакта месте. |
|surname|String| Фамилию контакта (семейства имени или фамилии). |
|businessPhones|String| Число основных телефонных месте контакта. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|directReports|Коллекция [directoryObject](directoryobject.md)| Прямые отчеты контакта. (Пользователей и контактов, у диспетчера свойство значение для этого контакта.)  Только для чтения. Допускается значение null.|
|manager|[directoryObject](directoryobject.md)| Пользователь или контакт, менеджер по этому контакту. Только для чтения.|
|memberOf|Коллекция [directoryObject](directoryobject.md)| Группы, которым принадлежит этот контакт. Только для чтения. Допускается значение null.|

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->