---
title: тип ресурса visualInfo
description: Сложный тип для представления **свойства visualElements** в объекте действия.
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 3c71a3613c51c1b7494fd44550108d8cd63645ff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019190"
---
# <a name="visualinfo-resource-type"></a>тип ресурса visualInfo

Пространство имен: microsoft.graph

Сложный тип для представления **свойства visualElements** в [объекте действия.](../resources/projectrome-activity.md)

Каждое действие пользователя будет показано в Timeline в качестве адаптивной карты. Разработчикам приложений рекомендуется предоставить настраиваемую карточку, которая отражает суть действий, которые произошли в вашем приложении. Это возможно, предоставив настраиваемую JSON-карту в свойстве контента.

Помимо визуальных метаданных с адаптивной картой приложение может указывать метаданные контента — данные, которые используются для создания выводов о деятельности пользователя, чтобы предложить новые действия для дальнейшего повторного взаимодействия. Это возможно с помощью свойства contentInfo для предоставления объекта JSON, который использует schema.org свойств для описания контента.

Если не предоставлена настраиваемая карта, с помощью свойств displayText и описания создается простая карта. Пользовательские карты рекомендуется для демонстрации наилучшего контента из приложения.

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:------|:-----------|
|displayText | Строка | Обязательный. Краткое текстовое описание уникальной активности пользователя (например, имя документа в случаях, когда действие относится к созданию документа)|
|description | String | Необязательный параметр. Более подробное текстовое описание уникальной активности пользователя (пример: имя документа, первое предложение и/или метаданные)|
|backgroundColor | String | Необязательный параметр. Фоновый цвет, используемый для отображения действия в пользовательском интерфейсе — цвета бренда для источника приложения. Должен быть допустимым цветом гекса|
|содержимое | Нетипизированный объект JSON | Необязательно. Настраиваемый фрагмент данных — объект JSON, используемый для предоставления настраиваемого контента для отрисовки активности в пользовательском интерфейсе Windows Shell|
|атрибуция | [imageInfo](../resources/projectrome-imageinfo.md) | Необязательно. Объект JSON, используемый для представления значка, который представляет приложение, используемую для создания действия|

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
    "@odata.type": "microsoft.graph.visualInfo",
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
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

