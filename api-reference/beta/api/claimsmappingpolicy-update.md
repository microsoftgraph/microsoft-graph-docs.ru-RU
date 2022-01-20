---
title: Update claimsmappingpolicy
description: Обновление свойств объекта claimsMappingPolicy.
ms.localizationpriority: medium
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e91c87a66052a878ca81b2cd554f30ab3ec5f203
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135617"
---
# <a name="update-claimsmappingpolicy"></a>Update claimsmappingpolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [claimsMappingPolicy.](../resources/claimsmappingpolicy.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy.ReadWrite.ApplicationConfiguration |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|определение|Коллекция строк| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками этой политики.  Обязательный.|
|description|Строка| Описание этой политики.|
|displayName|Строка| Отображение имени для этой политики. Обязательное.|
|isOrganizationDefault|Логическое|Если заданной для true, активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию является ложным.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
Content-type: application/json

{
    "displayName": "UpdateClaimsPolicy"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-claimsmappingpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-claimsmappingpolicy-powershell-snippets.md)]
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
  "description": "Update claimsmappingpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


