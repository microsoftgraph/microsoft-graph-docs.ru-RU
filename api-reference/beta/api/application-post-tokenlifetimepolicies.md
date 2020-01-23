---
title: Назначение типа ресурса tokenLifetimePolicy
description: Назначьте Токенлифетимеполици для приложения или участника службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fca668417d52914194ef087a32b28478101a32d7
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475623"
---
# <a name="assign-tokenlifetimepolicy"></a>Назначение типа ресурса tokenLifetimePolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Назначьте [токенлифетимеполици](../resources/tokenlifetimepolicy.md) [приложению](../resources/application.md) или [servicePrincipal](../resources/servicePrincipal.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy. Read. ALL и Application. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите идентификатор объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) (с помощью `@odata.id` свойства), который должен быть назначен для приложения или участника-службы.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
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
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
