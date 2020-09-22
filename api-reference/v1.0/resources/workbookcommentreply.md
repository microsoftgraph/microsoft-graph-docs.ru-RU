---
title: Тип ресурса Воркбуккомментрепли
description: Определение типа ресурса Воркбуккомментрепли
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 26c1862a05431f02149cb4ddbef9a8ab57449d37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015157"
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
|content|String|Содержимое ответа на комментарий.|
|contentType|String|Указывает тип ответа на комментарий.|
|id|String|Представляет идентификатор примечания. Только для чтения.|


## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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

