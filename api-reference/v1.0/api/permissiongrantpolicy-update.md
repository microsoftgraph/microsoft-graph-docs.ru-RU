---
title: Обновление Пермиссионгрантполици
description: Обновление объекта Пермиссионгрантполици.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 403968aa3ee4cde189c5b58331cd4dc90dd3cabd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524089"
---
# <a name="update-permissiongrantpolicy"></a>Обновление Пермиссионгрантполици

Пространство имен: microsoft.graph

Обновление свойств объекта  [пермиссионгрантполици](../resources/permissiongrantpolicy.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Policy. ReadWrite. Пермиссионгрант |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | Policy. ReadWrite. Пермиссионгрант |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип |Описание|
|:---------------|:--------|:----------|
| displayName | String |Отображаемое имя политики предоставления разрешений.|
| description |String| Описание политики предоставления разрешений.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и не возвращает ничего в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permissiongrantpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy
Content-Type: application/json

{
  "displayName": "Custom permission grant policy"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 204 No Content
```
