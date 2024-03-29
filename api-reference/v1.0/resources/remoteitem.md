---
author: JeremyKelley
title: remoteItem
ms.localizationpriority: medium
description: Ресурс remoteItem указывает, что элемент driveItem ссылается на элемент, находящийся на другом диске.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 2c9a71820f0862c827a62e827899de483fedbb0f
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034441"
---
# <a name="remoteitem-resource-type"></a>Тип ресурса remoteItem

Пространство имен: microsoft.graph

Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске.
Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.

[**driveItems**](driveitem.md) с аспектом **remoteItem**, не равным NULL, — это ресурсы, которые совместно используются, добавляются в пользовательские OneDrive или элементы, возвращаемые из шестнадцатеричных коллекций элементов (например, результаты поиска).

>**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image" : { "@odata.type": "microsoft.graph.image" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

| Имя свойства        | Тип                                | Описание                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [IdentitySet](identityset.md)       | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.                                                                                  |
| createdDateTime      | Timestamp                           | Дата и время создания элемента. Только для чтения.                                                                                                                        |
| file                 | [File](file.md)                     | Указывает, что удаленный элемент является файлом. Только для чтения.                                                                                                              |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md) | Сведения об удаленном элементе из локальной файловой системы. Только для чтения.                                                                                          |
| folder               | [Folder](folder.md)                 | Указывает, что удаленный элемент является папкой. Только для чтения.                                                                                                            |
| id                   | Строка                              | Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.                                                                                                    |
| image                | [Image](image.md)                   | Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.                                                                                               |
| lastModifiedBy       | [IdentitySet](identityset.md)       | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.                                                                            |
| lastModifiedDateTime | Timestamp                           | Дата и время последнего изменения элемента. Только для чтения.                                                                                                              |
| name                 | String                              | Необязательное свойство. Имя файла удаленного элемента. Только для чтения.                                                                                                                 |
| пакет              | [Package](package.md)               | В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения. |
| parentReference      | [ItemReference](itemreference.md)   | Свойства родительского элемента удаленного элемента. Только для чтения.                                                                                                           |
| общие               | [shared](shared.md)                 | Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.                                       |
| sharepointIds        | [SharepointIds](sharepointids.md)   | Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.                                          |
| size                 | Int64                               | Размер удаленного элемента. Только для чтения.                                                                                                                               |
| specialFolder        | [specialFolder][]                   | Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.                                                                     |
| video                | [Video](video.md)                   | Метаданные видео, если в роли элемента выступает видео. Только для чтения.                                                                                                    |
| webDavUrl            | Url                                 | URL-адрес, совместимый с протоколом DAV, для элемента.                                                                                                                                  |
| webUrl               | URL-адрес                                 | URL-адрес для отображения ресурса в браузере. Только для чтения.                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->

