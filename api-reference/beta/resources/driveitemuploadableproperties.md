---
title: Тип ресурса Дривеитемуплоадаблепропертиес
description: Ресурс Дривеитемуплоадаблепропертиес представляет элемент, который отправляется при создании сеанса отправки.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9505de9fd67a5f8cf8d7e89e964d98d758a22bde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067386"
---
# <a name="driveitemuploadableproperties-resource-type"></a>Тип ресурса Дривеитемуплоадаблепропертиес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **дривеитемуплоадаблепропертиес** представляет элемент, который отправляется при [создании сеанса отправки](../api/driveitem-createuploadsession.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип                              | Описание                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|description   |String                             | Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в OneDrive персональный.             |
|филесизе      |Int64                              | Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой. Только в OneDrive персональный. |
|fileSystemInfo|[fileSystemInfo](filesysteminfo.md)| Сведения о файловой системе на клиенте. Чтение и запись.                                                      |
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

