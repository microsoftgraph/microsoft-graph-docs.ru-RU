---
title: Тип ресурса Воркбуккоммент
description: Представляет комментарий в книге.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a7a3427512962bd38c90faa710c501380e353f22
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775897"
---
# <a name="workbookcomment-resource-type"></a>Тип ресурса Воркбуккоммент

Представляет комментарий в книге.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Воркбуккомментс](../api/workbook-list-comments.md) | Коллекция [воркбуккоммент](workbookComment.md) | Получение коллекции объектов **воркбуккоммент** . |
| [Получение Воркбуккоммент](../api/workbookcomment-get.md) | [воркбуккоммент](workbookcomment.md) | Чтение свойств и связей объекта **воркбуккоммент** . |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|content|String|Содержимое комментария.|
|contentType|String|Указывает тип комментария.|
|id|Строка| Представляет идентификатор примечания. Только для чтения.|

## <a name="relationships"></a>Отношения

| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|replies|Коллекция [воркбуккомментрепли](workbookcommentreply.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
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
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
