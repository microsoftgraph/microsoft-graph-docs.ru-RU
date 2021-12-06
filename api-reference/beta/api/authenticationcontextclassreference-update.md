---
title: Обновление проверки подлинностиContextClassReference
description: Обновление свойств объекта authenticationContextClassReference.
ms.localizationpriority: medium
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0fee669405322945ef0d4552b9e98fd63f2a39c8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982350"
---
# <a name="update-authenticationcontextclassreference"></a>Обновление проверки подлинностиContextClassReference

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)                    |
|:--------------------------------------|:---------------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Policy.ReadWrite.ConditionalAccess |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Policy.ReadWrite.ConditionalAccess |

> [!NOTE]
> Этот API имеет [известные проблемы, связанные](/graph/known-issues#permissions) с разрешениями.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/authenticationContextClassReferences/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание      |
|:--------------|:-----------------|
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса укажи значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

Список свойств см. в списке [authenticationContextClassReference.](../resources/authenticationContextClassReference.md)

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authenticationcontextclassreference"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
Content-type: application/json

{
   "value": 
    [
      {
         "displayName": "Contoso trusted locations",
        "description": "Access is only allowed from trusted locations",
        "isAvailable": true
      }
    ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-authenticationcontextclassreference-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
