---
title: тип ресурса fileSecurityState
description: Содержит сведения о файле (не процессе), связанных с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ac694c40e2f8a0a126d7849cf0131f4955af27d9e96aab73c30ead2d20ad42e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218725"
---
# <a name="filesecuritystate-resource-type"></a>тип ресурса fileSecurityState

Пространство имен: microsoft.graph

Содержит сведения о файле (не процессе), связанных с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий хеши файлов (криптографические и чувствительные к расположению).|
|name|String|Имя файла (без пути).|
|path|String|Полный путь файла файла/imageFile.|
|riskScore|String|Оценка риска поставщика, генерируемого или рассчитанного в файле оповещения. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|

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

