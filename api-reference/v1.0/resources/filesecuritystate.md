---
title: тип ресурса fileSecurityState
description: Содержит сведения о файле (не процессе), связанных с оповещением.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2db9d028c6a1550886a956bbfaad3bb3141f3141
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078863"
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
|riskScore|Строка|Оценка риска поставщика, генерируемого или рассчитанного в файле оповещения. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|

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

