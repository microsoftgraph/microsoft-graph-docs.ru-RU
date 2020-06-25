---
title: пендингконтентупдате
description: Ресурс Пендингконтентупдате указывает на то, что операция, которая может повлиять на двоичный контент driveItem, ожидает завершения.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: b1a197ae60dc8bb60533d567c6472a65988c3962
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863805"
---
# <a name="pendingcontentupdate-resource-type"></a>Тип ресурса Пендингконтентупдате

Пространство имен: microsoft.graph

Указывает, что операция, которая может повлиять на двоичное содержимое **driveItem** , ожидает завершения.

## <a name="properties"></a>Свойства

| Свойство     | Тип         | Описание |
|:-------------|:-------------|:------------|
|**куеуеддатетиме**|DateTimeOffset|Дата и время, когда отложенная двоичная операция была поставлена в очередь в течение времени в формате UTC. Только для чтения.|

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
