---
title: Создание Активитибаседтимеаутполици
description: Создание нового Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f061510c17cbd4a6ac1c41017a52f0e0d3160fa
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475446"
---
# <a name="create-activitybasedtimeoutpolicy"></a>Создание Активитибаседтимеаутполици

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy. ReadWrite. Аппликатионконфигуратион |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Policy. ReadWrite. Аппликатионконфигуратион |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса

В тексте запроса добавьте представление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
