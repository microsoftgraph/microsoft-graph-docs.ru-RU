---
title: тип ресурса educationFileResource
description: Подкласс educationResource, который представляет объект файла, связанный с назначением или отправкой.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c91b33734ea421c34e3627c76b7dd410ab8d251f262c509b15865d5c8db60814
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146918"
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


