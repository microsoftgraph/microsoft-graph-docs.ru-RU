---
title: тип ресурса driveItemUploadableProperties
description: Ресурс driveItemUploadableProperties представляет элемент, загружаемый при создании сеанса загрузки.
localization_priority: Normal
author: JeremyKelley
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 6c00270f1e86e2bb8f44af36c6c514c9b80a647d
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236217"
---
# <a name="driveitemuploadableproperties-resource-type"></a>тип ресурса driveItemUploadableProperties

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **driveItemUploadableProperties** представляет элемент, загружаемый при [создании сеанса загрузки.](../api/driveitem-createuploadsession.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип                              | Описание                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|description   |String                             | Предоставляет видимое пользователю описание элемента. Чтение и запись. Только на OneDrive Personal.             |
|driveItemSource| [driveItemSource](driveItemSource.md)              | Сведения об источнике элемента диска. Чтение и запись. Только на OneDrive для бизнеса и SharePoint.  |
|fileSize      |Int64                              | Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой. Только на OneDrive Personal. |
|fileSystemInfo|[fileSystemInfo](filesysteminfo.md)| Сведения о файловой системе на клиенте. Чтение и запись.                                                      |
|mediaSource  | [mediaSource](mediaSource.md)                    | Сведения о источниках мультимедиа. Чтение и запись. Только на OneDrive для бизнеса и SharePoint.                 |
|name          |String                             | Имя элемента (имя и расширение файла). Чтение и запись.                                          |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.driveItemUploadableProperties",
  "baseType": null
}-->

```json
{
  "description": "String",
  "fileSize": 1024,
  "fileSystemInfo": {"@odata.type": "microsoft.graph.fileSystemInfo"},
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

