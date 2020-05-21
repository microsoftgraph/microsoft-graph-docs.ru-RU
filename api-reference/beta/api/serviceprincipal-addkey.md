---
title: 'servicePrincipal: Аддкэй'
description: Добавление ключевых учетных данных в servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fccde0dac4e447f0e8558e65d375bb475e652f62
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333984"
---
# <a name="serviceprincipal-addkey"></a>servicePrincipal: Аддкэй

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавление ключевых учетных данных в [servicePrincipal](../resources/serviceprincipal.md). Этот метод вместе с [ремовекэй](serviceprincipal-removekey.md) можно использовать в servicePrincipal для автоматизации изкрутки ключей истечения срока действия.

> [!NOTE]
> [Создание servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [обновление операций servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления ключевых учетных данных для любых servicePrincipal с контекстом пользователя или без него.

В рамках проверки запроса для этого метода проверяется наличие проверки на наличие существующего ключа перед выполнением действия. 

СервицепринЦипалс, у которых нет существующих действительных сертификатов (например, не было добавлено ни одного сертификата, или у всех сертификатов истек срок действия), не сможете использовать это действие службы. [Обновление servicePrincipal](../api/serviceprincipal-update.md) можно использовать для выполнения обновления.

## <a name="permissions"></a>Permissions

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Отсутствуют.  |
|Делегированные (личная учетная запись Майкрософт) | Нет.    |
|Приложение | Отсутствуют. |

> [!NOTE]
> ServicePrincipal не требует каких – либо специальных разрешений для развертывания собственных ключей.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/addKey
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса

В тексте запроса укажите следующие обязательные свойства.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| кэйкредентиал | [кэйкредентиал](../resources/keycredential.md) | Новые учетные данные ключа servicePrincipal для добавления. Для этого использования требуются свойства __Type__, __Usage__ и __Key__ . Поддерживаются следующие типы ключей:<br><ul><li>`AsymmetricX509Cert`: Использование должно быть `Verify` .</li><li>`X509CertAndPassword`: Использование должно быть`Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Необходимо задать только __секреттекст__ , который должен содержать пароль для ключа. Это свойство является обязательным только для ключей типа `X509CertAndPassword` . Задайте для него значение `null` другой.|
| совмещен | String | Самозаверяющий маркер JWT, используемый в качестве подтверждения наличия существующих ключей. Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов servicePrincipal. Маркер должен содержать следующие утверждения:<ul><li>`aud`Необходимо указать аудиторию `00000002-0000-0000-c000-000000000000` .</li><li>`iss`-Issuer должен быть __идентификатором__ servicePrincipal, осуществляющим вызов.</li><li>`nbf`— Не до времени.</li><li>`exp`— Срок действия должен быть "NBF" + 10 минут.</li></ul><br>Ниже приведен [Пример](/graph/application-rollkey-prooftoken) кода, который можно использовать для создания этого маркера для проверки подлинности.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [кэйкредентиал](../resources/keycredential.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a>Пример 1: Добавление новых учетных данных ключа в объект servicePrincipal

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/addKey
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
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

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

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a>Пример 2: Добавление учетных данных ключа и соответствующего пароля для ключа

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/addKey
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

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
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
    "Error: serviceprincipal_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
