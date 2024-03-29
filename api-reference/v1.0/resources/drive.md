---
author: JeremyKelley
title: Тип ресурса drive
description: Ресурс drive — объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: eb7070e357681311cfe0d881940c3047dbac5505
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560238"
---
# <a name="drive-resource-type"></a>Тип ресурса drive

Пространство имен: microsoft.graph

Объект верхнего уровня, представляющий хранилище OneDrive пользователя или библиотеку документов в SharePoint.

Для пользователей OneDrive всегда будет доступен хотя бы один диск (диск по умолчанию). Для пользователей, у которых нет лицензии на OneDrive, такой диск может быть недоступен.

## <a name="methods"></a>Методы

|                        Метод                              |         Тип возвращаемых данных         | Описание |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| [Получение объекта drive][drive-get]                                     | drive                       | Получение метаданных о диске |
| [Получение корня диска][item-get]                                 | [driveItem][]               | Получение корневой папки диска |
| [Список отслеживаемых элементов][drive-following]                     | Коллекция [driveItem][]    | Получение списка отслеживаемых объектов driveItems пользователя |
| [Список дочерних элементов][item-children]                             | Коллекция [driveItem][]    | Получение списка дочерних элементов корневой папки диска |
| [Список изменений][item-changes]                               | Коллекция [driveItem][]    | Получение списка изменений для всех объектов driveItems в ресурсе Drive |
| [Search][item-search]                                      | Коллекция [driveItem][]    | Поиск объектов driveItems на диске |
| [Получение специальной папки](../api/drive-get-specialfolder.md)    | [driveItem][]               | Доступ к специальной папке по ее каноническому имени |


## <a name="properties"></a>Свойства

| Свойство             | Тип                          | Описание                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [identitySet][]               | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | Дата и время создания элемента. Только для чтения.                                                                                                                                                                                       |
| description          | String                        | Предоставляет видимое пользователю описание диска. Чтение и запись. 
| driveType            | Строка                        | Описывает тип диска, представленного данным ресурсом. Для личных дисков OneDrive возвращается `personal`. В случае дисков OneDrive для бизнеса возвращается `business`. В случае библиотек документов SharePoint возвращается `documentLibrary`. Только для чтения. |
| id                   | String                        | Уникальный идентификатор диска. Только для чтения.                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | Дата и время последнего изменения элемента. Только для чтения.                                                                                                                                                                             |
| name                 | string                        | Имя элемента. Чтение и запись.                                                                                                                                                                                                |
| owner                | [identitySet](identityset.md) | Необязательный параметр. Учетная запись пользователя, которому принадлежит диск. Только для чтения.                                                                                                                                                                       |
| quota                | [quota](quota.md)             | Необязательный параметр. Сведения о квоте на дисковое пространство. Только для чтения.                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения. Это свойство не возвращается по умолчанию и должно быть выбрано с помощью параметра запроса `$select`.  |
| system               | [systemFacet][]               | Если имеется это свойство, оно указывает, что данным диском управляет система. Только для чтения.
| webUrl               | строка (url-адрес)                  | URL-адрес для отображения ресурса в браузере. Только для чтения.                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>Связи

| Связь | Тип                                 | Описание
|:-------------|:-------------------------------------|:-----------------------
| bundles      | Коллекция [driveItem][]             | Коллекция объектов [bundles][bundle] (альбомы и наборы общих элементов с множественным выбором). Только в OneDrive для личного пользования.
| following    | Коллекция [driveItem][]             | Список элементов, которые отслеживает пользователь. Только в OneDrive для бизнеса.
| items        | Коллекция [driveItem][]             | Все элементы, содержащиеся на диске. Только для чтения. Допускается значение null.
| root         | [driveItem][]                        | Корневая папка на диске. Только для чтения.
| special      | Коллекция [driveItem][]             | Коллекция общих папок, доступных в OneDrive. Только для чтения. Допускается значение null.
| список         | [list][]                             | Для дисков в SharePoint, базовый список библиотек документов. Только для чтения. Допускается значение null.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление этого ресурса в формате JSON.

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
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [{"@odata.type": "microsoft.graph.driveItem"}],
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem"},
  "sharepointIds": {"@odata.type": "microsoft.graph.sharepointIds"},
  "special": [{"@odata.type": "microsoft.graph.driveItem"}],
  "system": {"@odata.type": "microsoft.graph.systemFacet"},
  "webUrl": "string",

}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[list]: list.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive&quot;: &quot;#"
  },
  "suppressions": []
}
-->


