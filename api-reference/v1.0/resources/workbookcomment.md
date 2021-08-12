---
title: тип ресурса workbookComment
description: Определение типа ресурса workbookComment
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8a81ac565e9dd65dfccfdef4eeb7eca86786eee4c225a8a1c91c4333e1c34573
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235235"
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

