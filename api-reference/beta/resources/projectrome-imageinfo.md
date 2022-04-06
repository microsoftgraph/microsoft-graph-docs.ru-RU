---
title: тип ресурса imageInfo
description: Сложный тип для представления свойства **атрибуции** в visualInfo части объекта действия.
ms.localizationpriority: medium
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: a123ea442fe4309ea96962b4155e0f36909fee7b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723772"
---
# <a name="imageinfo-resource-type"></a>тип ресурса imageInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип для представления свойства **атрибуции** в [visualInfo](../resources/projectrome-visualinfo.md) части [объекта действия](../resources/projectrome-activity.md) .

## <a name="properties"></a>Свойства

| Свойство      | Тип    | Описание                                                                                                                                              |
| :------------ | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------- |
| iconUrl       | String  | Необязательный; URI, который указывает на значок, который представляет приложение, используемую для создания действия                                                      |
| alternateText | String  | Необязательный; alt-text accessible content for the image                                                                                                      |
| addImageQuery | Boolean | Необязательный; параметр, используемый для того, чтобы указать, что сервер может динамически отрисовки изображения в ответ на параметризацию. Например— изображение с высоким контрастом |

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
