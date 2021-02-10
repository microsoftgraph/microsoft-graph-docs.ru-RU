---
title: Тип ресурса workbookCommentReply
description: Определение типа ресурса workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7c47a6eb7abf8bf675dd8be35db6a96e511dbbcf
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158039"
---
# <a name="workbookcommentreply-resource-type"></a>Тип ресурса workbookCommentReply

Пространство имен: microsoft.graph

Представляет ответ на комментарий Excel.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список workbookCommentReplies](../api/workbookcomment-list-replies.md) | [Коллекция workbookCommentReply](workbookcommentreply.md) | Получить список объектов workbookcommentreply. |
| [Get workbookCommentReply](../api/workbookcommentreply-get.md) | [workbookCommentReply](workbookcommentreply.md) | Чтение свойств и связей объекта workbookCommentReply. |
| [Создание workbookCommentReply](../api/workbookcomment-post-replies.md) | [workbookCommentReply](workbookcommentreply.md) | Создайте новую книгуCommentReply. |
## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|content|String|Содержимое ответа на комментарий.|
|contentType|String|Указывает тип ответа на комментарий.|
|id|String|Представляет идентификатор примечания. Только для чтения.|


## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "keyProperty": "id"
}-->

```json
{
  "content": "String",
  "contentType": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

