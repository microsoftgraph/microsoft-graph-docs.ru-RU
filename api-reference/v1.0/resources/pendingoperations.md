---
title: pendingOperations
description: Ресурс pendingOperations указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, находятся в ожидании завершения.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 8fac755c6bcce65af03a96b1c13d6186ae3c1f86e975cf9577d0a5e568ebe62a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178123"
---
# <a name="pendingoperations-resource-type"></a>тип ресурса pendingOperations

Пространство имен: microsoft.graph

Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem,** ожидают завершения.

## <a name="properties"></a>Свойства

| Свойство                | Тип        | Описание |
|:------------------------|:------------|:------------|
|**pendingContentUpdate** |[pendingContentUpdate](pendingcontentupdate.md)|Свойство, которое указывает, что операция, которая может обновить двоичное содержимое файла, находится в стадии завершения.|

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

