---
title: 'Приложение: Аддкэй'
description: Добавление учетных данных ключа в приложение.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 498e848d2adb8d3ccf14df2744c1ed5ec05be692
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962304"
---
# <a name="application-addkey"></a>Приложение: Аддкэй

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавление в [приложение](../resources/application.md)учетных данных ключа. Этот метод вместе с [ремовекэй](application-removekey.md)может использоваться приложением для автоматизации изкрутки ключей истечения срока действия.

> [!NOTE]
> Вы можете продолжить использовать операции " [создать приложение](../api/application-post-applications.md) " и " [Обновление приложения приложения](../api/application-update.md) " для добавления и обновления ключевых учетных данных для любого приложения с контекстом пользователя или без него. 

В рамках проверки запроса для этого метода проверяется наличие проверки на наличие существующего ключа перед выполнением действия. 

Приложения, у которых нет существующих действительных сертификатов (сертификаты не были добавлены до тех пор, или у всех сертификатов истек срок действия), не удастся использовать это действие службы. Чтобы вместо этого выполнить обновление, вы можете использовать операцию [обновления приложения](../api/application-update.md).

## <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Нет.  |
|Делегированные (личная учетная запись Майкрософт) | Нет.    |
|Приложение | Нет. |

> [!NOTE]
> Приложению не требуется определенное разрешение для развертывания собственных ключей. 

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите следующие обязательные свойства.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| keyCredential | [keyCredential](../resources/keycredential.md) | Новые учетные данные ключа приложения, которые требуется добавить. Для этого использования требуются свойства __Type__ , __Usage__ и __Key__ . Поддерживаются следующие типы ключей:<br><ul><li>`AsymmetricX509Cert`: Использование должно быть `Verify` .</li><li>`X509CertAndPassword`: Использование должно быть `Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Необходимо задать только __секреттекст__ , который должен содержать пароль для ключа. Это свойство является обязательным только для ключей типа `X509CertAndPassword` . Задайте для него значение `null` другой.|
| совмещен | String | Самозаверяющий маркер JWT, используемый в качестве подтверждения наличия существующих ключей. Маркер JWT должен быть подписан с использованием закрытого ключа одного из существующих действительных сертификатов приложения. Маркер должен содержать следующие утверждения:<ul><li>`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</li><li>`iss` — издателем должен быть __идентификатор__  приложения, выполняющего вызов.</li><li>`nbf` — вовремя.</li><li>`exp` — сроком действия должно быть значение "nbf" + 10 минут.</li></ul><br>Ниже приведен [Пример](/graph/application-rollkey-prooftoken) кода, который можно использовать для создания этого маркера для проверки подлинности.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [кэйкредентиал](../resources/keycredential.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-add-a-new-key-credential-to-an-application"></a>Пример 1: Добавление новых учетных данных ключа в приложение

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey"
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
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-java-snippets.md)]
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

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a>Пример 2: Добавление учетных данных ключа и соответствующего пароля для ключа

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "application_addkey"
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
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->


