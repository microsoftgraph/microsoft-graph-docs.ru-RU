---
title: Тип ресурса Воркбуккомментрепли
description: Определение типа ресурса Воркбуккомментрепли
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5d080f283401d9486de53095d3ad25029edbb14b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519241"
---
# <a name="workbookcommentreply-resource-type"></a>Тип ресурса Воркбуккомментрепли

Пространство имен: microsoft.graph

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
