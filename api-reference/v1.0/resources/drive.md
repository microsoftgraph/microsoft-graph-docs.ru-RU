---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
ms.openlocfilehash: 0b178967f7eb8da8bdf8584bb13a7d4f9950392b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="drive-resource-type"></a>Тип ресурса Drive

Ресурс Drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.

Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.

## <a name="json-representation"></a>Описание в формате JSON

Ниже показано представление ресурса Drive в формате JSON.

Ресурс **drive** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.drive",
       "keyProperty": "id", 
       "optionalProperties": [ "activities", "createdBy", "createdDateTime", "description", "lastModifiedBy", "lastModifiedDateTime", "name", "webUrl", "items", "root", "special", "system"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
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
| description          | String                        | Предоставляет отображаемое для пользователя описание диска. Чтение и запись.
| driveType            | Строка                        | Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения. |
| id                   | String                        | Уникальный идентификатор диска. Только для чтения.                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | Дата и время последнего изменения элемента. Только для чтения.                                                                                                                                                                             |
| name                 | string                        | Имя элемента. Чтение и запись.                                                                                                                                                                                                |
| owner                | [identitySet](identityset.md) | Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.                                                                                                                                                                       |
| quota                | [quota](quota.md)             | Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                                                                                                                                                         |
| system               | [systemFacet][]               | Если имеется это свойство, оно указывает, что данным диском управляет система. Только для чтения.
| webUrl               | строка (url-адрес)                  | URL-адрес для отображения ресурса в браузере. Только для чтения.                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>Связи

| Связь | Тип                                 | Описание
|:-------------|:-------------------------------------|:-----------------------
| items        | Коллекция [driveitem](driveitem.md) | Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.
| root         | [driveitem](driveitem.md)            | Корневая папка на диске. Только для чтения.
| special      | Коллекция [driveitem](driveitem.md) | Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.

## <a name="methods"></a>Методы

|                        Стандартная задача                         |         Метод HTTP         |
| :--------------------------------------------------------- | :-------------------------- |
| [Получение метаданных другого ресурса Drive][drive-get]           | `GET /drives/{drive-id}`    |
| [Получение корневой папки для ресурса Drive, используемого по умолчанию, пользователя][item-get]       | `GET /drive/root`           |
| [Получение списка дочерних элементов ресурса Drive][item-children]             | `GET /drive/root/children`  |
| [Получение списка изменений для всех элементов в ресурсе Drive][item-changes]    | `GET /drive/root/delta`     |
| [Поиск элементов в ресурсе Drive][item-search]               | `GET /drive/root/search`    |
| [Доступ к специальной папке](../api/drive_get_specialfolder.md) | `GET /drive/special/{name}` |

В примерах в предыдущей таблице используется каталог `/drive`, но можно использовать и другие пути.

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive_get.md
[item-get]: ../api/driveitem_get.md
[item-changes]: ../api/driveitem_delta.md
[item-search]: ../api/driveitem_search.md
[item-children]: ../api/driveitem_list_children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
