---
title: Тип ресурса Воркбуккоммент
description: Определение типа ресурса Воркбуккоммент
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3a238ab9b033cd1906842f61d9f2d72b6d642335
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533384"
---
# <a name="workbookcomment-resource-type"></a>Тип ресурса Воркбуккоммент

Пространство имен: microsoft.graph

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

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|отвечать|Коллекция [воркбуккомментрепли](workbookcommentreply.md)| Только для чтения. Допускается значение null.|

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
