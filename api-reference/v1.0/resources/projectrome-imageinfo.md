---
title: тип ресурса imageInfo
description: Сложный тип для представления свойства **атрибуции** в visualInfo части объекта действия.
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: cf76bd7e81f913f9641568bbd20c62a1c3ed16a8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019197"
---
# <a name="imageinfo-resource-type"></a>тип ресурса imageInfo

Пространство имен: microsoft.graph

Сложный тип для представления свойства **атрибуции** в [visualInfo](../resources/projectrome-visualinfo.md) части [объекта действия.](../resources/projectrome-activity.md)

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|iconUrl | Строка | Необязательный; URI, который указывает на значок, который представляет приложение, используемую для создания действия|
|alternateText | Строка | Необязательный; alt-text accessible content for the image|
|addImageQuery | Логический | Необязательный; параметр, используемый для того, чтобы указать, что сервер может динамически отрисовки изображения в ответ на параметризацию. Например— изображение с высоким контрастом|

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

