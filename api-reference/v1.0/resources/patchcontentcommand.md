---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0a6ea27f1dd6206a97b6ad60daf783b3092b69a4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807026"
---
# <a name="patchcontentcommand-resource-type"></a>Тип ресурса Патчконтенткомманд

Пространство имен: microsoft.graph

Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.

## <a name="json-representation"></a>Представление в формате JSON

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
|target|String|Обновляемый элемент. Должен быть `#<data-id>` либо сгенерированным `<id>` элементом, либо `body` `title` ключевым словом or.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
