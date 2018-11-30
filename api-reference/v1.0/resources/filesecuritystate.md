---
title: Тип ресурса fileSecurityState
description: Содержит сведения о файле (не процесса), связанные с оповещение.
ms.openlocfilehash: d1358d7fe0d5565845201781e32b3da14a89f412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028183"
---
# <a name="filesecuritystate-resource-type"></a>Тип ресурса fileSecurityState

Содержит сведения о файле (не процесса), связанные с оповещение.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Description|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).|
|name|String|Имя файла (без пути).|
|path|String|Полный путь к файлу файл/файл изображения.|
|riskScore|String|Поставщик создан/вычисляется риск показатель файл оповещений. Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|

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