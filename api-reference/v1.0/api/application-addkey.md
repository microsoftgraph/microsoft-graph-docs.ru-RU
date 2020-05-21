---
title: 'Приложение: Аддкэй'
description: Добавление в приложение учетных данных ключа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1ea747f50138304a497acacdea188d5beb2d2a98
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336598"
---
# <a name="application-addkey"></a>Приложение: Аддкэй

Пространство имен: microsoft.graph

Добавление в [приложение](../resources/application.md)учетных данных ключа. Этот метод вместе с [ремовекэй](application-removekey.md) может использоваться приложением для автоматизации изсрочки ключей истечения срока действия.

> [!NOTE]
> С помощью команды " [создать приложение](../api/application-post-applications.md) и [Обновление приложений](../api/application-update.md) " можно продолжать использовать для добавления и обновления ключевых учетных данных для любого приложения с контекстом пользователя или без него.

В рамках проверки запроса для этого метода проверяется наличие проверки на наличие существующего ключа перед выполнением действия. 

Приложения, у которых нет существующих действительных сертификатов (сертификаты не были добавлены до тех пор, или у всех сертификатов истек срок действия), не удастся использовать это действие службы. Вместо этого можно использовать операцию [обновления приложения](../api/application-update.md) для выполнения обновления.

## <a name="permissions"></a>Permissions

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Отсутствуют.  |
|Делегированные (личная учетная запись Майкрософт) | Нет.    |
|Приложение | Отсутствуют. |

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

## <a name="request-body"></a>Основной текст запроса

В тексте запроса укажите следующие обязательные свойства.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| кэйкредентиал | [кэйкредентиал](../resources/keycredential.md) | Новые учетные данные ключа приложения, которые требуется добавить. Для этого использования требуются свойства __Type__, __Usage__ и __Key__ . Поддерживаются следующие типы ключей:<br><ul><li>`AsymmetricX509Cert`: Использование должно быть `Verify` .</li><li>`X509CertAndPassword`: Использование должно быть`Sign`</li></ul>|
| passwordCredential | [passwordCredential](../resources/passwordcredential.md) | Необходимо задать только __секреттекст__ , который должен содержать пароль для ключа. Это свойство является обязательным только для ключей типа `X509CertAndPassword` . Задайте для него значение `null` другой.|
| совмещен | String | Самозаверяющий маркер JWT, используемый в качестве подтверждения наличия существующих ключей. Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов приложения. Маркер должен содержать следующие утверждения:<ul><li>`aud`Необходимо указать аудиторию `00000002-0000-0000-c000-000000000000` .</li><li>`iss`-Issuer должен быть __идентификатором__ приложения, осуществляющего вызов.</li><li>`nbf`— Не до времени.</li><li>`exp`— Срок действия должен быть "NBF" + 10 минут.</li></ul><br>Ниже приведен [Пример](/graph/application-rollkey-prooftoken) кода, который можно использовать для создания этого маркера для проверки подлинности.|

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
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
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
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
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
