---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7ae624f4bc02c257f2b7947a10a65634580e5f1e
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681132"
---
# <a name="create-grouplifecyclepolicy"></a>Создание groupLifecyclePolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается |
|Приложение |  Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса
В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.
##### <a name="response"></a>Отклик

Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


