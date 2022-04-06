---
title: 'servicePrincipal: addKey'
description: Добавление учетных данных ключа объекту servicePrincipal.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0fbeb8479463fd52c2cbbf041ba24470ae2d7307
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63671666"
---
# <a name="serviceprincipal-addkey"></a>servicePrincipal: addKey

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавляет ключевые учетные данные в [службуPrincipal](../resources/serviceprincipal.md). Этот метод наряду с [removeKey](serviceprincipal-removekey.md) может использоваться службойPrincipal для автоматизации проката истекающих ключей.

> [!NOTE]
> [Создание службыPrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [Update servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления учетных данных для любой службыPrincipal с контекстом пользователя или без него.

В рамках проверки запроса для этого метода проверяется доказательство на наличие существующего ключа перед выполнением действия. 

ServicePrincipals, у которых нет существующих действительных сертификатов (например, еще не добавлены сертификаты или истек срок действия всех сертификатов), не смогут использовать это действие службы. Для выполнения обновления можно использовать службу [UpdatePrincipal](../api/serviceprincipal-update.md).

## <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All, Directory.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Нет.    |
|Приложение | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |


## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addKey
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
| keyCredential | [keyCredential](../resources/keycredential.md) | Добавлены новые учетные данные ключа servicePrincipal. Тип __,__ __использование и__ __ключ__ необходимые свойства для этого использования. Поддерживаемые ключевые типы:<br><ul><li>`AsymmetricX509Cert`: Использование должно быть `Verify`.</li><li>`X509CertAndPassword`: Использование должно быть `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Требуется __установить только secretText__ , который должен содержать пароль для ключа. Это свойство требуется только для ключей типа `X509CertAndPassword`. Установите его в противном `null` случае.|
| доказательство | Строка | Самозаверяемый маркер JWT, используемый в качестве доказательства владения существующими ключами. Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов службыPrincipal. Маркер должен содержать следующие утверждения:<ul><li>`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - Эмитент должен быть __id__  службыPrincipal, которая делает вызов.</li><li>`nbf` — вовремя.</li><li>`exp` - Срок действия должен быть `nbf` + 10 минут.</li></ul><br>Действия по созданию этого маркера владения см. в журнале [Generating proof of possession tokens for rolling keys](/graph/application-rollkey-prooftoken).|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` отклика и новый [объект keyCredential](../resources/keycredential.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a>Пример 1. Добавление новых учетных данных ключа в службуPrincipal

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_1"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-1-javascript-snippets.md)]
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

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a>Пример 2. Добавление учетных данных ключа и связанного пароля для ключа

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey_2"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/addKey
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-2-javascript-snippets.md)]
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
  "description": "servicePrincipal: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



