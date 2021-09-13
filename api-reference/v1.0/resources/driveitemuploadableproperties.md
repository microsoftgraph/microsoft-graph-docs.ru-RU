---
title: тип ресурса driveItemUploadableProperties
description: Ресурс driveItemUploadableProperties представляет элемент, загружаемый при создании сеанса загрузки.
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: bedbdbd67010352c3bc69a743e355efaf0514409
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067467"
---
# <a name="driveitemuploadableproperties-resource-type"></a>тип ресурса driveItemUploadableProperties

Пространство имен: microsoft.graph

Представляет элемент, загружаемый при [создании сеанса загрузки.](../api/driveitem-createuploadsession.md)

## <a name="json-representation"></a>Представление в формате JSON

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

