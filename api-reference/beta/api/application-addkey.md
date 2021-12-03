---
title: 'приложение: addKey'
description: Добавление учетных данных ключа в приложение.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7e8b39733b208a84246dc2ae4f706d86434b1510
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285043"
---
# <a name="application-addkey"></a>приложение: addKey

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавление учетных данных ключа в [приложение.](../resources/application.md) Этот метод, наряду с [removeKey,](application-removekey.md)может использоваться приложением для автоматизации проката истекающих ключей.

> [!NOTE]
> Вы можете продолжать использовать операции приложения [Create и](../api/application-post-applications.md) [Update](../api/application-update.md) для добавления и обновления учетных данных для любого приложения с контекстом пользователя или без него. 

В рамках проверки запроса для этого метода проверяется доказательство на наличие существующего ключа перед выполнением действия. 

Приложения, у которых нет существующих действительных сертификатов (еще не добавлены сертификаты или истек срок действия всех сертификатов), не смогут использовать это действие службы. Чтобы вместо этого выполнить обновление, вы можете использовать операцию [обновления приложения](../api/application-update.md).

## <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Нет.  |
|Делегированные (личная учетная запись Майкрософт) | Нет.    |
|Приложение | Нет. |

> [!NOTE]
> Приложение не нуждается в специальном разрешении для сверки собственных ключей. 

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажи следующие необходимые свойства.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| keyCredential | [keyCredential](../resources/keycredential.md) | Добавлены новые учетные данные ключа приложения. __Тип,__ __использование и__ __ключ__ необходимые свойства для этого использования. Поддерживаемые ключевые типы:<br><ul><li>`AsymmetricX509Cert`: Использование должно быть `Verify` .</li><li>`X509CertAndPassword`: Использование должно быть `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Требуется __установить только secretText,__ который должен содержать пароль для ключа. Это свойство требуется только для ключей типа `X509CertAndPassword` . Установите его в `null` противном случае.|
| доказательство | Строка | Самозаверяемый маркер JWT, используемый в качестве доказательства владения существующими ключами. Маркер JWT должен быть подписан с использованием закрытого ключа одного из существующих действительных сертификатов приложения. Маркер должен содержать следующие утверждения:<ul><li>`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</li><li>`iss` — издателем должен быть __идентификатор__  приложения, выполняющего вызов.</li><li>`nbf` — вовремя.</li><li>`exp` - Срок действия должен `nbf` быть + 10 минут.</li></ul><br>О действиях по созданию этого доказательства маркера владения см. в журнале [Generating proof of possession tokens for rolling keys.](/graph/application-rollkey-prooftoken) Дополнительные сведения о типах утверждений см. в дополнительных сведениях [о полезной нагрузке Claims.](/azure/active-directory/develop/active-directory-certificate-credentials)|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и новый `200 OK` [объект keyCredential](../resources/keycredential.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-add-a-new-key-credential-to-an-application"></a>Пример 1. Добавление новых учетных данных ключей в приложение

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey_1"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "AsymmetricX509Cert",
        "usage": "Verify",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": null,
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/application-addkey-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a>Пример 2. Добавление учетных данных ключа и связанного пароля для ключа

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey_2"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "X509CertAndPassword",
        "usage": "Sign",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": {
        "secretText": "MKTr0w1..."
    },
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/application-addkey-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



