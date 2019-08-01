---
title: Тип ресурса "безопасность"
description: Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 87bd321a3c5e66cdc5d4fdc7fcb1407d02fbca1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034456"
---
# <a name="security-resource-type"></a>Тип ресурса "безопасность"

Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление оповещений](../api/alert-list.md) | Коллекция [alert](alert.md) | Получение коллекции объектов Alert. |
| [получение оповещений](../api/alert-get.md) | Коллекция [alert](alert.md) | Получение объекта Alert. |
| [Обновление оповещений](../api/alert-update.md) | Коллекция [alert](alert.md) | Получение объекта Alert. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|alerts|Коллекция [alert](alert.md)| Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>Пример

Ресурс **безопасности** доступен в корне графа.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
