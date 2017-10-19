---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 9a5214f9c5e161de0be66ac634c7c5538b203772
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="filesysteminfo-facet"></a>Аспект FileSystemInfo

Ресурс **FileSystemInfo** содержит свойства, которые отображаются в локальной файловой системе устройства для локальной версии элемента.
Этот аспект можно использовать, чтобы указать дату создания или последнего изменения элемента, какой она была на локальном устройстве.

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
| **lastAccessedDateTime** | DateTimeOffset | Дата и время последнего использования файла в формате UTC. Доступно только для [списка последних файлов](../api/drive_recent.md). |
| **lastModifiedDateTime** | DateTimeOffset | Дата и время последнего изменения файла в клиентском устройстве в формате UTC.                                                        |

## <a name="notes"></a>Примечания

Значения свойств **createdDateTime** и **lastModifiedDateTime** отличаются от этих же свойств ресурса [DriveItem](driveitem.md).
В качестве значений для ресурса DriveItem выступают дата и время создания или изменения, которые зарегистрированы в службе.
Значения, хранящиеся в ресурсе **FileSystemInfo**, предоставляет клиент.

Например, если файл был создан на устройстве в понедельник, но не отправлен в службу до вторника, клиент, отправляющий файл, должен записать дату создания, соответствующую понедельнику, в аспект `fileSystemInfo`. При получении метаданных элемента в качестве даты его создания будет указан вторник, но в аспекте `fileSystemInfo` будет отображаться исходная дата создания — понедельник.

Эти свойства доступны для чтения и записи. Если вы загружаете файл и вам известны локальные клиентские значения для этих полей, их необходимо включить в запрос.

Если содержимое файла обновлено и эти свойства не предоставлены, **lastModifiedDateTime** автоматически сбрасывает текущее время.

## <a name="remarks"></a>Примечания

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
