---
title: Тип ресурса workbookComment
description: Определение типа ресурса workbookComment
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 24cce9a392f9d5b9cfcdfc35e0c87ade16d760d7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158053"
---
# <a name="workbookcomment-resource-type"></a>Тип ресурса workbookComment

Пространство имен: microsoft.graph

Представляет комментарий в книге.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список workbookComments](../api/workbook-list-comments.md) | [коллекция workbookComment](workbookComment.md) | Получите **коллекцию объектов workbookComment.** |
| [Get workbookComment](../api/workbookcomment-get.md) | [workbookComment](workbookcomment.md) | Чтение свойств и связей объекта **workbookComment.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|content|String|Содержимое комментария.|
|contentType|String|Указывает тип комментария.|
|id|String| Представляет идентификатор примечания. Только для чтения.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|replies|[Коллекция workbookCommentReply](workbookcommentreply.md)| Только для чтения. Допускается значение null.|

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

