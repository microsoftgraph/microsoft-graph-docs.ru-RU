---
title: pendingContentUpdate
description: Ресурс pendingContentUpdate указывает, что операция, которая может повлиять на двоичное содержимое driveItem, ожидает завершения.
ms.localizationpriority: medium
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: ec44c2c1d75bc11276d99dad1815c0d999b4f0e1
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176341"
---
# <a name="pendingcontentupdate-resource-type"></a>Тип ресурса pendingContentUpdate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, что операция, которая может повлиять на двоичное содержимое **driveItem** , ожидает завершения.

## <a name="properties"></a>Свойства

| Свойство     | Тип         | Описание |
|:-------------|:-------------|:------------|
|queuedDateTime|DateTimeOffset|Дата и время, когда ожидающая двоичная операция была поставлена в очередь в формате UTC. Только для чтения.|

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


