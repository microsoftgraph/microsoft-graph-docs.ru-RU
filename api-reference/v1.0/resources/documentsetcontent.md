---
author: swapnil1993
title: тип ресурса documentSetContent
description: Ресурс documentSetContent содержит метаданные о файле, присутствуют в расположении контента по умолчанию.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 741047ab90badd16e4f7dea61c92ca8d952ee978
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072542"
---
# <a name="documentsetcontent-resource-type"></a>тип ресурса documentSetContent

Пространство имен: microsoft.graph

Представляет содержимое документа по умолчанию, установленного в SharePoint.
## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание|
|:---------------|:--------|:--------------------------------------------------|
| contentType    | microsoft.graph.contentTypeInfo | Сведения о типе контента файла. |
| fileName      | string  | Имя файла в папке ресурсов, который должен быть добавлен в качестве контента по умолчанию или шаблона в наборе документов.|
| folderName         | строка  | Имя папки, в которой будет размещен файл при создания нового набора документов в библиотеке.|

## <a name="json-representation"></a>Представление в формате JSON

Вот представление JSON ресурса **documentSetContent.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSetContent" } -->

```json
{
  "contentType": { "@type": "microsoft.graph.contentTypeInfo" },
  "fileName": "string",
  "folderName": "string"
}
```
