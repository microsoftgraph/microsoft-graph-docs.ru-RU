---
title: тип ресурса educationMediaResource
description: Представляет ресурс файлов мультимедиа для educationAssignment. Наследует от educationResource
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d89835234ff1e388b5da9c618322ebad0c8a101e
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220806"
---
# <a name="educationmediaresource-resource-type"></a>тип ресурса educationMediaResource

Пространство имен: microsoft.graph

Представляет ресурс файлов мультимедиа для [educationAssignment](educationassignment.md). Наследует [от educationResource](educationresource.md).

Upload эти файлы в **каталог fileResource,** связанный с назначением или отправкой.

Следующие типы файлов — это медиа-ресурсы: `webm` , , , , `mkv` `avi` , `wmv` `mp4` и `m4v` `mpg` `mpeg` `m2v` `jpg` `png` `gif` `bmp` `heic` `jpeg` `psd` `mp3` `m4a` .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|String|Расположение файла в общей папке точеки. Обязательная|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationMediaResource"
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
  "description": "educationMediaResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


