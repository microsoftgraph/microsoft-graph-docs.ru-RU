---
title: Тип ресурса educationMediaResource
description: Представляет ресурс файла мультимедиа для объекта educationAssignment. Наследует от educationResource
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 98b645b33e2109cc187f5b895175defeb1c90d4f
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684503"
---
# <a name="educationmediaresource-resource-type"></a>Тип ресурса educationMediaResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс файла мультимедиа для [объекта educationAssignment](educationassignment.md). Наследуется от [educationResource](educationresource.md).

Upload эти файлы в **каталог fileResource**, связанный с назначением или отправкой.

Следующие типы файлов являются ресурсами мультимедиа: `webm`, `mkv`, `avi`, , `wmv`, `m4v``mp4`, `mpg`, `mpeg`, `m2v`, `jpg`, `png``gif`, `bmp`, , `heic`, , , `jpeg`и `m4a``psd``mp3` .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fileUrl|String|Расположение файла в общей папке точек. Обязательный|
|createdBy|String|Отображаемое имя пользователя, создавшего этот ресурс.|
|createdDateTime|DateTimeOffset|Дата, когда была добавлена повторная ошибка.|
|displayName|string|Отображаемое имя пользователя, который добавил ресурс.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменяет ресурс|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения ресурса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

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
  "fileUrl": "String",
  "createdBy": "String (User)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": "String (User)",
  "lastModifiedDateTime": "String (timestamp)"
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


