---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3c8aab8770304f8616025d0d5ac2e70ad41a1340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534074"
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
|action|оненотепатчактионтипе|Действие, которое необходимо выполнить для целевого элемента. Возможные значения: `replace`, `append`, `delete`, `insert`, или. `prepend`|
|content|String|Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если содержимое содержит двоичные данные, необходимо отправить запрос, используя тип `multipart/form-data` контента с частью "Commands". |
|position|оненотепатчинсертпоситион|Место для добавления предоставленного контента относительно целевого элемента. Возможные значения: `after` (по умолчанию) или `before`.|
|target|String|Обновляемый элемент. Должен быть `#<data-id>` либо сгенерированным `<id>` элементом, либо ключевым словом `body` or. `title`|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
