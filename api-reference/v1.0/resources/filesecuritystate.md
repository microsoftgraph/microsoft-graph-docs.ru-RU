---
title: Тип ресурса fileSecurityState
description: Содержит сведения о файле (не процессе), связанном с оповещением.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 00a8f3ce61c185969fab0adaf99483a8d03c906c
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971072"
---
# <a name="filesecuritystate-resource-type"></a>Тип ресурса fileSecurityState

Пространство имен: microsoft.graph

Содержит сведения о файле (не процессе), связанном с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий хэши файлов (криптографические и с учетом расположения).|
|name|String|Имя файла (без пути).|
|path|String|Полный путь к файлу или imageFile.|
|riskScore|Строка|Созданная поставщиком или вычисляемая оценка риска для файла оповещений. Рекомендуемый диапазон значений — 0–1, что соответствует проценту.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

