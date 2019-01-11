---
title: Тип ресурса fileSecurityState
description: Содержит сведения о файле (не процесса), связанные с оповещение.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894098"
---
# <a name="filesecuritystate-resource-type"></a>Тип ресурса fileSecurityState

Содержит сведения о файле (не процесса), связанные с оповещение.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).|
|name|Строка|Имя файла (без пути).|
|path|String|Полный путь к файлу файл/файл изображения.|
|riskScore|Строка|Поставщик создан/вычисляется риск показатель файл оповещений. Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|

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
