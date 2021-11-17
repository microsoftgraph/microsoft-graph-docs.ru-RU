---
title: Обновление appManagementPolicy
description: Обновление политики управления приложениями.
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b19a09e4bd752c04938c20181c6a55924ae029fb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995650"
---
# <a name="update-appmanagementpolicy"></a>Обновление appManagementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление [объекта appManagementPolicy.](../resources/appManagementPolicy.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                |
| :------------------------------------- | :--------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Policy.ReadWrite.ApplicationConfiguration |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                             |
| Для приложений                            | Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/appManagementPolicies/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса укажи значения для соответствующих полей из [appManagementPolicy,](../resources/appManagementPolicy.md) которые должны быть обновлены.
Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.
Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство                | Тип                                                                        | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|:------------------------|:----------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName  | Строка                                                      | Отображает имя политики. Унаследованный от [policyBase](../resources/policybase.md).                                        |
| description  | Строка                                                      | Описание политики. Унаследованный от [policyBase](../resources/policybase.md).                                         |
| isEnabled    | Boolean                                                     | Обозначает, включена ли политика.                                      |
| ограничения | [appManagementConfiguration](../resources/appManagementConfiguration.md) | Ограничения, которые применяются к основному объекту приложения или службы. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_appManagementPolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}

{
    "isEnabled": false
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-appmanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-appmanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-appmanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-appmanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-appmanagementpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "update appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
