---
title: Тип ресурса объекта filesecuritystate
description: Содержит сведения о файле (не процессу), связанном с предупреждением.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564794"
---
# <a name="filesecuritystate-resource-type"></a>Тип ресурса объекта filesecuritystate

Содержит сведения о файле (не процессу), связанном с предупреждением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).|
|name|String|Имя файла (без пути).|
|path|String|Полный путь к файлу или файлу imageFile.|
|riskScore|String|Созданный поставщиком/вычисляемый показатель риска для файла оповещений. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|

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
