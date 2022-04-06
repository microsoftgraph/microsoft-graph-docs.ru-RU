---
author: swapnil1993
title: тип ресурса documentSetContent
description: Ресурс documentSetContent содержит метаданные о файле, присутствуют в расположении контента по умолчанию.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 0ec71779247f143c0f43f1695c75049af15d453f
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722984"
---
# <a name="documentsetcontent-resource-type"></a>тип ресурса documentSetContent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Содержит метаданные о файле, присутствуют в расположении контента по умолчанию типа контента.

## <a name="properties"></a>Свойства

| Свойство    | Тип                            | Описание                                                                                                     |
| :---------- | :------------------------------ | :-------------------------------------------------------------------------------------------------------------- |
| contentType | microsoft.graph.contentTypeInfo | Сведения о типе контента файла.                                                                           |
| fileName    | строка                          | Имя файла в папке ресурсов, которое должно быть добавлено в качестве контента по умолчанию или шаблона в наборе документов |
| folderName  | строка                          | Имя папки, в которой будет размещен файл при создания нового набора документов в библиотеке.                 |

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса **documentSetContent** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```
