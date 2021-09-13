---
title: Удаление permissionGrantConditionSet из исключения коллекции разрешенийGrantPolicy
description: Удаляет исключенный набор условий из политики предоставления разрешений.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 48cd558f6a02067834b258838b7641a55b9bec8e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072794"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a>Удаление permissionGrantConditionSet из исключения коллекции разрешенийGrantPolicy

Пространство имен: microsoft.graph

Удаляет [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) из  исключенной коллекции [permissionGrantPolicy.](../resources/permissiongrantpolicy.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | PermissionGrantPolicy.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
| Для приложений | PermissionGrantPolicy.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-excludes-java-snippets.md)]
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
