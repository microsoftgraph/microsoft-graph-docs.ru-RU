---
title: тип ресурсов безопасности
description: Ресурс безопасности является точкой входа для объектной модели безопасности. Он возвращает ресурс безопасности singleton. Он не содержит никаких полезных свойств.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 14c0aa4a239b143df79d873e127c3e70dc7900fe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139606"
---
# <a name="security-resource-type"></a>тип ресурсов безопасности

Пространство имен: microsoft.graph

Ресурс безопасности является точкой входа для объектной модели безопасности. Он возвращает ресурс безопасности singleton. Он не содержит никаких полезных свойств.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление оповещений](../api/alert-list.md) | Коллекция [alert](alert.md) | Получите коллекцию объектов оповещения. |
| [получения оповещений](../api/alert-get.md) | Коллекция [alert](alert.md) | Получите объект оповещений. |
| [Обновление оповещений](../api/alert-update.md) | Коллекция [alert](alert.md) | Получите объект оповещений. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|оповещения|Коллекция [alert](alert.md)| Только для чтения. Допускается значение null.|


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
```http
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

