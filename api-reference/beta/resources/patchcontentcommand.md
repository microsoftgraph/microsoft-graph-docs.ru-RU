---
title: Тип ресурса patchContentCommand
description: Изменения, внося в OneNote в запросе PATCH.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.technology: microsoft-graph
author: jewan-microsoft
ms.openlocfilehash: 11155779f5765e098a566589b522f9e987d6a68d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176778"
---
# <a name="patchcontentcommand-resource-type"></a>Тип ресурса patchContentCommand

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изменения, внося в OneNote в запросе PATCH.

## <a name="json-representation"></a>Представление JSON

Ниже приведено представление ресурса в формате JSON, которое отправляется в тексте запроса [PATCH pages/{id}](../api/page-update.md) .

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
|action|Строка|Действие, выполняемые с целевым элементом. Возможные значения: `replace`, `append`, `delete`, `insert` и `prepend`.|
|content|String|Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если содержимое содержит двоичные данные, запрос `multipart/form-data` должен быть отправлен с использованием типа контента с частью "Команды". |
|position|Строка|Место для добавления предоставленного контента относительно целевого элемента. Возможные значения: ( `after` по умолчанию) или `before`.|
|target|Строка|Обновляемый элемент. Должен быть либо `#<data-id>` созданным `{id}` элементом, либо ключевым словом `body` `title` .|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


