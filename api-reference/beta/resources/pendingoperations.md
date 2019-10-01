---
title: пендингоператионс
description: Ресурс Пендингоператионс указывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d83a68bf555fa5cc239fb38b147d12754f223e13
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333432"
---
# <a name="pendingoperations-resource-type"></a>Тип ресурса Пендингоператионс

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
