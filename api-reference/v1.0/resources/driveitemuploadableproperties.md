---
title: тип ресурса driveItemUploadableProperties
description: Ресурс driveItemUploadableProperties представляет элемент, загружаемый при создании сеанса загрузки.
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 39a1b68f4584e6c583213a08b203f1e3d5a7a5453b8eb1ad8708c06ef953c0c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182562"
---
# <a name="driveitemuploadableproperties-resource-type"></a>тип ресурса driveItemUploadableProperties

Пространство имен: microsoft.graph

Представляет элемент, загружаемый при [создании сеанса загрузки.](../api/driveitem-createuploadsession.md)

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

## <a name="properties"></a>Свойства

| Свойство     | Тип                              | Описание                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|**description**   |String                             | Предоставляет видимое пользователю описание элемента. Чтение и запись. Только на OneDrive Personal.             |
|**fileSize**      |Int64                              | Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой. Только на OneDrive Personal. |
|**fileSystemInfo**|[fileSystemInfo](filesysteminfo.md)| Сведения о файловой системе на клиенте. Чтение и запись.                                                      |
|**name**          |String                             | Имя элемента (имя и расширение файла). Чтение и запись.                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

