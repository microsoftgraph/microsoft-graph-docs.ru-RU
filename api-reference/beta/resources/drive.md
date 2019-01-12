---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 581a611fa077eab6d44db01d998d5ea42886f052
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938190"
---
# <a name="drive-resource-type"></a>Тип ресурса диска

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.

Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса Drive в формате JSON.

Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

| Свойство             | Тип                          | Описание                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [identitySet][]               | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | Дата и время создания элемента. Только для чтения.                                                                                                                                                                                       |
| описание          | String                        | Предоставляет описание объекта drive, которое видит пользователь. Чтение и запись.
| driveType            | Строка                        | Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения. |
| id                   | String                        | Уникальный идентификатор диска. Только для чтения.                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | Дата и время последнего изменения элемента. Только для чтения.                                                                                                                                                                             |
| name                 | строка                        | Имя элемента. Чтение и запись.                                                                                                                                                                                                |
| owner                | [identitySet](identityset.md) | Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.                                                                                                                                                                       |
| quota                | [quota](quota.md)             | Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                                                                                                                                                         |
| system               | [systemFacet][]               | Если это свойство задано, оно указывает, что данным объектом drive управляет система. Только для чтения.
| webUrl               | строка (url-адрес)                  | URL-адрес для отображения ресурса в браузере. Только для чтения.                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>Связи

| Связь | Тип                                 | Описание
|:-------------|:-------------------------------------|:-----------------------
| activities   | Коллекция [itemActivity][]          | Список последних действий, выполненных для этого объекта drive.
| items        | Коллекция [driveitem](driveitem.md) | Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.
| root         | [driveitem](driveitem.md)            | Корневая папка на диске. Только для чтения.
| special      | Коллекция [driveitem](driveitem.md) | Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.
| следующие    | [DriveItem](driveitem.md) коллекции | Список элементов, которые подписан пользователь. Только в OneDrive для бизнеса.

## <a name="methods"></a>Методы

|                        Стандартная задача                         |         Метод HTTP         |
| :--------------------------------------------------------- | :-------------------------- |
| [Получение метаданных другого ресурса Drive][drive-get]           | `GET /drives/{drive-id}`    |
| [Получение корневой папки для ресурса Drive, используемого по умолчанию для пользователя][item-get]       | `GET /drive/root`           |
| [Список действий для ресурса Drive][drive-activities]        | `GET /drive/activities`     |
| [Список, а затем элементов][drive-following]                     | `GET /drive/following`      |
| [Получение списка дочерних элементов ресурса Drive][item-children]             | `GET /drive/root/children`  |
| [Получение списка изменений для всех элементов в ресурсе Drive][item-changes]    | `GET /drive/root/delta`     |
| [Поиск элементов в ресурсе Drive][item-search]               | `GET /drive/root/search`    |
| [Доступ к специальной папке](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

В предыдущей таблице, используйте приведенные примеры `/drive`, но другие пути являются допустимыми слишком.

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
