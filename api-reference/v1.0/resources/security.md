---
title: Тип ресурса безопасности
description: Безопасность ресурсов — это точка входа для объектной модели безопасности. Возвращает ресурсов безопасности одного. Он не содержит какие-либо можно использовать свойства.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983256"
---
# <a name="security-resource-type"></a>Тип ресурса безопасности

Безопасность ресурсов — это точка входа для объектной модели безопасности. Возвращает ресурсов безопасности одного. Он не содержит какие-либо можно использовать свойства.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [перечисление оповещений](../api/alert-list.md); | [оповещение о](alert.md) семейства сайтов | Получите коллекцию объекта оповещения. |
| [Получение оповещений](../api/alert-get.md) | [оповещение о](alert.md) семейства сайтов | Получите объект оповещения. |
| [Обновление оповещений](../api/alert-update.md) | [оповещение о](alert.md) семейства сайтов | Получите объект оповещения. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|alerts|[оповещение о](alert.md) семейства сайтов| Только для чтения. Допускается значение null.|


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

**Безопасность** ресурсов доступна в корне диаграммы.

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
