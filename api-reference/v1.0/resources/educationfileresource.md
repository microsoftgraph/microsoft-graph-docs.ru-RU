---
title: тип ресурса educationFileResource
description: Подкласс educationResource, который представляет объект файла, связанный с назначением или отправкой.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e0e101e1d21bd8e5aa205875a9f444678aeee218
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036643"
---
# <a name="educationfileresource-resource-type"></a>тип ресурса educationFileResource

Пространство имен: microsoft.graph

Подкласс [educationResource,](educationresource.md) который представляет объект файла, связанный с назначением или отправкой.

В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), а является файлом, который не имеет специальной обработки в системе. Файловый ресурс должен храниться в **ресурсеFolder,** связанном с назначением или отправкой этого ресурса.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|Строка|Расположение на диске файлового ресурса.|

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


