---
title: Тип ресурса Дривеитемуплоадаблепропертиес
description: Ресурс Дривеитемуплоадаблепропертиес представляет элемент, который отправляется при создании сеанса отправки.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f8511bba850c1d165fe9b7082b7df51900b17962
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333436"
---
# <a name="driveitemuploadableproperties-resource-type"></a>Тип ресурса Дривеитемуплоадаблепропертиес

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