---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3798c86812452daeaa1332fd6de5c4cf3229497f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082926"
---
# <a name="patchcontentcommand-resource-type"></a>Тип ресурса Патчконтенткомманд

Пространство имен: microsoft.graph

Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [Patch Pages/{ID} '](../api/page-update.md) .

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|action|оненотепатчактионтипе|Действие, которое необходимо выполнить для целевого элемента. Возможные значения: `replace` , `append` , `delete` , `insert` , или `prepend` .|
|content|String|Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если содержимое содержит двоичные данные, необходимо отправить запрос, используя `multipart/form-data` тип контента с частью "Commands". |
|position|оненотепатчинсертпоситион|Место для добавления предоставленного контента относительно целевого элемента. Возможные значения: `after` (по умолчанию) или `before` .|
|target|Строка|Обновляемый элемент. Должен быть `#<data-id>` либо сгенерированным `<id>` элементом, либо `body` `title` ключевым словом or.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

