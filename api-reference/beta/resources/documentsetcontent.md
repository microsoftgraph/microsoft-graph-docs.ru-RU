---
author: swapnil1993
title: тип ресурса documentSetContent
description: Ресурс documentSetContent содержит метаданные о файле, присутствуют в расположении контента по умолчанию.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8597dfb8a762d2166a9253fb4e806b9c2fcf5223
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447402"
---
# <a name="documentsetcontent-resource-type"></a>тип ресурса documentSetContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Содержит метаданные о файле, присутствуют в расположении контента по умолчанию типа контента.

## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание
|:---------------|:--------|:--------------------------------------------------
| contentType    | microsoft.graph.contentTypeInfo | Сведения о типе контента файла. 
| fileName      | string  | Имя файла в папке ресурсов, которое должно быть добавлено в качестве контента по умолчанию или шаблона в наборе документов  
| folderName         | string  | Имя папки, в которой будет размещен файл при создания нового набора документов в библиотеке.

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса **documentSetContent.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```