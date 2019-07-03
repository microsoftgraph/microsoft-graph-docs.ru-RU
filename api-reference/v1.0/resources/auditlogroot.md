---
title: Тип ресурса Аудитлогрут
description: Содержит различные типы журналов аудита. Эти ресурсы возвращают одноэлементный ресурс Аудитлог. Он не содержит пригодных для использования свойств.
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c43367465ac89116fcdca2460deb832d2cfbe746
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444024"
---
# <a name="auditlogroot-resource-type"></a>Тип ресурса Аудитлогрут

Содержит различные типы журналов аудита. Эти ресурсы возвращают одноэлементный ресурс Аудитлог. Он не содержит пригодных для использования свойств.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Перечисление элементов аудита каталога в коллекции и их свойства.|
|[Получение directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Получение определенного элемента аудита каталога и его свойств.|
|[Перечисление signIn](../api/signin-list.md) | [signIn](signin.md) |Чтение свойств и связей объектов signIn.|
|[Получение объекта signIn](../api/signin-get.md) | [signIn](signin.md) |Чтение свойств и связей объекта signIn.|

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Отношения

| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|Директоряудитс|Коллекция [директоряудит](directoryaudit.md)| Только для чтения. Допускается значение null.|
|Сигнинс|Коллекция [SignIn](signin.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a>Пример


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
} -->
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
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
