---
title: Тип ресурса fileHash
description: Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).
localization_priority: Normal
ms.openlocfilehash: 9d72812d1ad43999ea3ed5b28251d629b9380d47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564773"
---
# <a name="filehash-resource-type"></a>Тип ресурса fileHash

Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Хаштипе|fileHashType|Тип хэша файла. Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.|
|Хашвалуе|String|Значение хэша файла.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
