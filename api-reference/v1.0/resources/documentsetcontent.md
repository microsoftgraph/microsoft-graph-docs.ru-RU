---
author: swapnil1993
title: тип ресурса documentSetContent
description: Ресурс documentSetContent содержит метаданные о файле, присутствуют в расположении контента по умолчанию.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5894c31c990f2cd55d5646c44e569c310d599e39
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757642"
---
# <a name="documentsetcontent-resource-type"></a>тип ресурса documentSetContent

Пространство имен: microsoft.graph

Представляет содержимое документа по умолчанию, установленного в SharePoint.
## <a name="properties"></a>Свойства

| Свойство  | Тип    | Описание|
|:---------------|:--------|:--------------------------------------------------|
| contentType    | microsoft.graph.contentTypeInfo | Сведения о типе контента файла. |
| fileName      | String  | Имя файла в папке ресурсов, который должен быть добавлен в качестве контента по умолчанию или шаблона в наборе документов.|
| folderName         | String  | Имя папки, в которой будет размещен файл при создания нового набора документов в библиотеке.|

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
