---
title: Тип ресурса fileHash
description: Содержит конфиденциальную информацию о хеше файла (криптографии и конфиденциальном расположении).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 98b2e9ed0ba4ca6a7af23d1fe6cf7acb278975ccf36f45983c58aeb5d721e744
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218718"
---
# <a name="filehash-resource-type"></a>Тип ресурса fileHash

Пространство имен: microsoft.graph

Содержит конфиденциальную информацию о хеше файла (криптографии и конфиденциальном расположении).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hashType|fileHashType|Тип hash файла. Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.|
|hashValue|String|Значение hash файла.|

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

