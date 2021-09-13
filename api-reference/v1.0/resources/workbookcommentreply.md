---
title: тип ресурса workbookCommentReply
description: Определение типа ресурса workbookCommentReply
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 44ca6d6038aba3a12e9d96a63202aad3a5d0d59a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139459"
---
# <a name="workbookcommentreply-resource-type"></a>тип ресурса workbookCommentReply

Пространство имен: microsoft.graph

Представляет ответ на Excel комментарий.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список книгCommentReplies](../api/workbookcomment-list-replies.md) | [коллекция workbookCommentReply](workbookcommentreply.md) | Извлечение списка объектов workbookcommentreply. |
| [Get workbookCommentReply](../api/workbookcommentreply-get.md) | [workbookCommentReply](workbookcommentreply.md) | Чтение свойств и связей объекта workbookCommentReply. |
| [Создание книгиCommentReply](../api/workbookcomment-post-replies.md) | [workbookCommentReply](workbookcommentreply.md) | Создание новой книгиCommentReply. |
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

