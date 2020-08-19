---
title: Тип ресурса Имажеинфо
description: Сложный тип для представления свойства " **атрибуты** " в части висуалинфо объекта Activity.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: a57155a880e9ba4e00dd9a4d17ddae3742bbaa8e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807484"
---
# <a name="imageinfo-resource-type"></a>Тип ресурса Имажеинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип для представления свойства " **атрибуты** " в части [висуалинфо](../resources/projectrome-visualinfo.md) объекта [Activity](../resources/projectrome-activity.md) .

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|iconUrl | String | Необязательно URI, указывающий на значок, представляющий приложение, используемое для создания действия.|
|алтернатетекст | String | Необязательно доступное для изображения содержимое с замещающим текстом|
|аддимажекуери | Логический | Необязательно параметр, указывающий на то, что сервер может динамически отображать изображение в ответ на параметризация. Например, изображение с высокой контрастностью|

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
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
