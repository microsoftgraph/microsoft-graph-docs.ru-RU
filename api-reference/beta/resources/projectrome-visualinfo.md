---
title: Тип ресурса visualInfo
description: Сложный тип для представления свойство **visualElements** в объекте активности.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 56d3822c89de074847aeab6c8a0a742ecd7f006f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514924"
---
# <a name="visualinfo-resource-type"></a>Тип ресурса visualInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип для представления свойство **visualElements** в объекте [активности](../resources/projectrome-activity.md) .

Каждое действие пользователя отображаются на шкале как адаптивный карточки. Разработчики приложений, рекомендуется для предоставления настраиваемых карточку, которая записывает только операции, которая выполнялась в вашем приложении. Это можно сделать с указанием настраиваемых карточки JSON в свойстве контента.

В дополнение к visual метаданных с адаптивный карточки приложение может указать контента метаданных — данные, которые являются используются для формирования вывод на действие пользователя, чтобы предлагать новые действия для оказания будущих повторно. Это можно сделать с помощью свойства contentInfo действия для предоставления объект JSON, который использует свойства schema.org для описания содержимого.

Если этот параметр не указан настраиваемых карточки простой карточки будут создаваться с использованием отображаемый текст и описание свойств. Настраиваемые карточки, рекомендуется использовать для демонстрации наиболее содержимого из в вашем приложении.

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:------|:-----------|
|отображаемый текст | String | Обязательный. Короткая текстовое описание уникальное действие пользователя (например, имя документа в тех случаях, где действие относится к создания документов)|
|description | String | Необязательный параметр. Больше текстовое описание уникальный активности пользователя (пример: документа имя, первое предложение и/или метаданные)|
|BackgroundColor | String | Необязательный параметр. Цвет фона, используемого для отображения активности в пользовательском Интерфейсе - торговая марка цвет для исходного приложения действия. Должен быть допустимый шестнадцатеричный цвет|
|content | Объектный JSON | Необязательный параметр. Настраиваемые части данных — объект JSON, используется для предоставления пользовательского контента для отображения активности в пользовательском Интерфейсе командной консоли Windows|
|атрибуты | [imageInfo](../resources/projectrome-imageinfo.md) | Необязательный параметр. Объект JSON, используемый для представления значок, представляющий приложение, используемый для создания операции|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@data.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@data.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-visualinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
