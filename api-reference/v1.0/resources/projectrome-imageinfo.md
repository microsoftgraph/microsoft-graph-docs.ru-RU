---
title: тип ресурса imageInfo
description: Сложный тип для представления свойства **атрибуции** в visualInfo части объекта действия.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 1f8f4a69304412296030eb50a907bdf9ca6f6c000b16e295688c836585fbb775
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229005"
---
# <a name="imageinfo-resource-type"></a>тип ресурса imageInfo

Пространство имен: microsoft.graph

Сложный тип для представления свойства **атрибуции** в [visualInfo](../resources/projectrome-visualinfo.md) части [объекта действия.](../resources/projectrome-activity.md)

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|iconUrl | String | Необязательный; URI, который указывает на значок, который представляет приложение, используемую для создания действия|
|alternateText | String | Необязательный; alt-text accessible content for the image|
|addImageQuery | Логическое | Необязательный; параметр, используемый для того, чтобы указать, что сервер может динамически отрисовки изображения в ответ на параметризацию. Например— изображение с высоким контрастом|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

