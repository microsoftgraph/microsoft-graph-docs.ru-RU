---
title: Тип ресурса "безопасность"
description: Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579214"
---
# <a name="security-resource-type"></a>Тип ресурса "безопасность"

Ресурс Security — точка входа для объектной модели безопасности. Он возвращает одноэлементный ресурс безопасности. Он не содержит пригодных для использования свойств.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [перечисление оповещений](../api/alert-list.md); | [](alert.md) коллекция Alerts | Получение коллекции объектов Alert. |
| [получение оповещений](../api/alert-get.md) | [](alert.md) коллекция Alerts | Получение объекта Alert. |
| [Обновление оповещений](../api/alert-update.md) | [](alert.md) коллекция Alerts | Получение объекта Alert. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|alerts|[](alert.md) коллекция Alerts| Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON
Ниже показано представление ресурса в формате JSON.

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
