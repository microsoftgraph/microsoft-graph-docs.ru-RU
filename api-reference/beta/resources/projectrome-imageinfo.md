---
title: Тип ресурса imageInfo
description: Сложный тип для представления свойство **атрибуты** в части visualInfo объекта активности.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 347e07b70e8bad6dce8571dd1fbac5cd00d9abdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978692"
---
# <a name="imageinfo-resource-type"></a>Тип ресурса imageInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сложный тип для представления свойство **атрибуты** в части [visualInfo](../resources/projectrome-visualinfo.md) объекта [активности](../resources/projectrome-activity.md) .

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|iconUrl | Строка | Необязательный; URI, указывающий на значок, представляющий приложение, используемый для создания операции|
|alternateText | Строка | Необязательный; Замещающий текст доступного содержимого для образа|
|addImageQuery | Логический | Необязательный; параметр служит для указания сервера может отобразить изображение динамически в ответ на параметризации. Для примера — изображение высокой контрастности|

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
