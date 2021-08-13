---
title: pendingContentUpdate
description: Ресурс pendingContentUpdate указывает, что операция, которая может повлиять на двоичное содержимое driveItem, находится в стадии завершения.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 917a952ba9694178c17b3ef6ccb89780790528860f227a3a5f02f5cb5f44cf5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178138"
---
# <a name="pendingcontentupdate-resource-type"></a>тип ресурсов pendingContentUpdate

Пространство имен: microsoft.graph

Указывает, что операция, которая может повлиять на двоичное содержимое **driveItem,** находится в стадии завершения.

## <a name="properties"></a>Свойства

| Свойство     | Тип         | Описание |
|:-------------|:-------------|:------------|
|**queuedDateTime**|DateTimeOffset|Дата и время ожидания двоичной операции в очереди во время UTC. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->

