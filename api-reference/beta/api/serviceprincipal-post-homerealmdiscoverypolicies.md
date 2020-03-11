---
title: Назначение типа ресурса homeRealmDiscoveryPolicy
description: Назначьте Хомереалмдисковериполици участнику службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 49483db94f77151364932869c4ae58861530ce2f
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590246"
---
# <a name="assign-homerealmdiscoverypolicy"></a>Назначение типа ресурса homeRealmDiscoveryPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Назначьте [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) для [servicePrincipal](../resources/servicePrincipal.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL  |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Authorization | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите идентификатор объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) (с помощью `@odata.id` свойства), который должен быть назначен субъекту-службе.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
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
  "description": "Assign homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
