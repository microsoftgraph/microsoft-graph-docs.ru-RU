---
title: пендингоператионс
description: Ресурс Пендингоператионс указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b7b5d162bfcc9cccdfc7a2ea769e4ea39272e2d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998097"
---
# <a name="pendingoperations-resource-type"></a>Тип ресурса Пендингоператионс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, что одна или несколько операций, которые могут повлиять на состояние **driveItem** , ожидают завершения.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|пендингконтентупдате|[пендингконтентупдате](pendingcontentupdate.md)|Свойство, указывающее на то, что операция, которая может обновить двоичный контент файла, ожидает завершения.|

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


