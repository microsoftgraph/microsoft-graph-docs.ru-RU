---
title: тип ресурса educationFileResource
description: Подкласс educationResource, который представляет объект файла, связанный с назначением или отправкой.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 814ea6119210184356c561ac4f6a3dee5d3eac10
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912617"
---
# <a name="educationfileresource-resource-type"></a>тип ресурса educationFileResource

Пространство имен: microsoft.graph

Подкласс [educationResource,](educationresource.md) который представляет объект файла, связанный с назначением или отправкой.

В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), а является файлом, который не имеет специальной обработки в системе. Файловый ресурс должен храниться в **ресурсеFolder,** связанном с назначением или отправкой этого ресурса.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|String|Расположение на диске файлового ресурса.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


