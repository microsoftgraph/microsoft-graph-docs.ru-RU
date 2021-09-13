---
author: JeremyKelley
ms.date: 09/10/2017
title: FileSystemInfo
ms.localizationpriority: medium
description: Ресурс FileSystemInfo содержит свойства, которые отображаются в локальной файловой системе устройства для локальной версии элемента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 706128b116a7a8f8b4ff1450096f3335c44b165c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137681"
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
  "tocPath&quot;: &quot;Facets/FileSystemInfo"
} -->

