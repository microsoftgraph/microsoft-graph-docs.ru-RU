---
title: Тип ресурса Воркбуккомментрепли
description: Определение типа ресурса Воркбуккомментрепли
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0a4dfc215eec435c67f1259a85e899db4dfb2b63
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775904"
---
# <a name="workbookcommentreply-resource-type"></a>Тип ресурса Воркбуккомментрепли

Представляет ответ на комментарий Excel.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Воркбуккомментреплиес](../api/workbookcomment-list-replies.md) | Коллекция [воркбуккомментрепли](workbookcommentreply.md) | Получение списка объектов воркбуккомментрепли. |
| [Получение Воркбуккомментрепли](../api/workbookcommentreply-get.md) | [воркбуккомментрепли](workbookcommentreply.md) | Чтение свойств и связей объекта Воркбуккомментрепли. |
| [Создание Воркбуккомментрепли](../api/workbookcomment-post-replies.md) | [воркбуккомментрепли](workbookcommentreply.md) | Создание нового Воркбуккомментрепли. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|content|String|Содержимое комментария, на который дан ответ.|
|contentType|String|Указывает тип комментария для ответа.|
|id|Строка|Представляет идентификатор примечания. Только для чтения.|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "baseType": "",
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
