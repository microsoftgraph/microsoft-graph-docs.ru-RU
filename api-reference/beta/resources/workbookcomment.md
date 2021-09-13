---
title: тип ресурса workbookComment
description: Представляет комментарий в книге.
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3ff1508bb17ad584d11c1b14ebe95c32ab0c9f55
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59119837"
---
# <a name="workbookcomment-resource-type"></a>тип ресурса workbookComment

Пространство имен: microsoft.graph

Представляет комментарий в книге.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список книгКомменты](../api/workbook-list-comments.md) | [коллекция workbookComment](workbookComment.md) | Получите **коллекцию объектов workbookComment.** |
| [Get workbookComment](../api/workbookcomment-get.md) | [workbookComment](workbookcomment.md) | Ознакомьтесь с свойствами и отношениями объекта **workbookComment.** |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|content|String|Содержимое комментария.|
|contentType|String|Указывает тип комментария.|
|id|String| Представляет идентификатор примечания. Только для чтения.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|ответы|[коллекция workbookCommentReply](workbookcommentreply.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
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
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


