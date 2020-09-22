---
title: пендингконтентупдате
description: Ресурс Пендингконтентупдате указывает на то, что операция, которая может повлиять на двоичный контент driveItem, ожидает завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5e7291ac4591ba63bec96108dd46bf9561358bb4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998096"
---
# <a name="pendingcontentupdate-resource-type"></a>Тип ресурса Пендингконтентупдате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, что операция, которая может повлиять на двоичное содержимое **driveItem** , ожидает завершения.

## <a name="properties"></a>Свойства

| Свойство     | Тип         | Описание |
|:-------------|:-------------|:------------|
|куеуеддатетиме|DateTimeOffset|Дата и время, когда отложенная двоичная операция была поставлена в очередь в течение времени в формате UTC. Только для чтения.|

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


