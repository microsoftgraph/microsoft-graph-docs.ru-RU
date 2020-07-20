---
title: пендингоператионс
description: Ресурс Пендингоператионс указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 381ecd3bf302a1e7d323211cac071e360340b5c6
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863686"
---
# <a name="pendingoperations-resource-type"></a>Тип ресурса Пендингоператионс

Пространство имен: microsoft.graph

Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem** , ожидают завершения.

## <a name="properties"></a>Свойства

| Свойство                | Тип        | Описание |
|:------------------------|:------------|:------------|
|**пендингконтентупдате** |[пендингконтентупдате](pendingcontentupdate.md)|Свойство, указывающее на то, что операция, которая может обновить двоичный контент файла, ожидает завершения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingOperations",
  "baseType": null
}-->

```json
{
  "pendingContentUpdate": {"@odata.type": "microsoft.graph.pendingContentUpdate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingOperations resource indicates that an operation that may affect the state of the DriveItem is pending completion.",
  "keywords": "pendingoperations,pendingoperations,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
