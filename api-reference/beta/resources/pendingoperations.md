---
title: pendingOperations
description: Ресурс pendingOperations указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
ms.localizationpriority: medium
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 6cf3903a99405dbcbdf83f26da053030e46dbb9e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176538"
---
# <a name="pendingoperations-resource-type"></a>Тип ресурса pendingOperations

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem** , ожидают завершения.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|pendingContentUpdate|[pendingContentUpdate](pendingcontentupdate.md)|Свойство, указывающее, что операция, которая может обновить двоичное содержимое файла, ожидает завершения.|

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


