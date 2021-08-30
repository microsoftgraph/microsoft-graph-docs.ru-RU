---
author: swapnil1993
title: тип ресурса documentSetContent
description: Ресурс documentSetContent содержит метаданные о файле, присутствуют в расположении контента по умолчанию.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5926e80c6c507591942009ae00ea199fdccfdca0
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696834"
---
# <a name="documentsetcontent-resource-type"></a>тип ресурса documentSetContent

Пространство имен: microsoft.graph

Представляет содержимое документа по умолчанию, установленного в SharePoint.
## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание|
|:---------------|:--------|:--------------------------------------------------|
| contentType    | microsoft.graph.contentTypeInfo | Сведения о типе контента файла. |
| fileName      | string  | Имя файла в папке ресурсов, который должен быть добавлен в качестве контента по умолчанию или шаблона в наборе документов.|
| folderName         | string  | Имя папки, в которой будет размещен файл при создания нового набора документов в библиотеке.|

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