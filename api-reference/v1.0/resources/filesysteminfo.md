---
author: JeremyKelley
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
description: Ресурс FileSystemInfo содержит свойства, которые отображаются в локальной файловой системе устройства для локальной версии элемента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f080e6222555f2bc9fcea8cb8a3a157a8e2eb096
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240061"
---
# <a name="filesysteminfo-facet"></a>Аспект FileSystemInfo

Пространство имен: microsoft.graph

Ресурс **FileSystemInfo** содержит свойства, которые отображаются в локальной файловой системе устройства для локальной версии элемента. Этот аспект можно использовать, чтобы указать последнюю дату изменения или создания элемента, какой она была на локальном устройстве.

Он доступен в свойстве fileSystemInfo ресурсов [driveItem][item-resource].

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a>Свойства

| Свойство                 | Тип           | Описание                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| **createdDateTime**      | DateTimeOffset | Дата и время создания файла в клиентском устройстве в формате UTC.                                                              |
| **lastAccessedDateTime** | DateTimeOffset | Дата и время последнего использования файла в формате UTC. Доступно только для [списка последних файлов](../api/drive-recent.md). |
| **lastModifiedDateTime** | DateTimeOffset | Дата и время последнего изменения файла в клиентском устройстве в формате UTC.                                                        |

## <a name="notes"></a>Примечания

Значения свойств **createdDateTime** и **lastModifiedDateTime** отличаются от этих же свойств ресурса [DriveItem](driveitem.md). В качестве значений для ресурса DriveItem выступают созданные или измененные дата и время, которые можно увидеть в службе. Значения, хранящиеся в ресурсе **FileSystemInfo**, предоставляются клиентом.

Например, если файл был создан на устройстве в понедельник, но не загружен в службу до вторника, клиент, загружающий файл, должен прописать аспект `fileSystemInfo`включить дату создания в понедельник. При получении метаданных элемента в качестве даты его создания указывается вторник, но в аспекте `fileSystemInfo` отображается исходная дата создания — понедельник.

Эти свойства доступны для чтения и записи. Если вы загружаете файл и вам известны локальные клиентские значения для этих полей, их необходимо включить в запрос.

Если содержимое файла обновлено и эти свойства не предоставлены, **lastModifiedDateTime** автоматически сбрасывает текущее время.

## <a name="remarks"></a>Замечания

* Свойство **lastAccessedDateTime** недоступно для элементов в SharePoint Online или в OneDrive для бизнеса.

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->

