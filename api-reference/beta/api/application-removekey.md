---
title: 'Приложение: Ремовекэй'
description: Удаление ключевых учетных данных из приложения
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 868cacc6aae55d5779f974cff4bef4171aae9623
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961869"
---
# <a name="application-removekey"></a>Приложение: Ремовекэй

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление ключевых учетных данных из [приложения](../resources/application.md). Этот метод вместе с [аддкэй](application-addkey.md) может использоваться приложением для автоматизации пошаговых ключей истечения срока действия.

> [!NOTE]
> [Создание servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [обновление операций servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления ключевых учетных данных для любого приложения с приложением или контекстом пользователя.

В рамках проверки запроса для этого метода проверяется наличие проверки на наличие существующего ключа перед выполнением действия.

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
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите следующие обязательные свойства.

| Свойство  | Тип | Описание|
|:----------|:-----|:-----------|
| Него значение KeyID     | GUID | Уникальный идентификатор пароля.|
| совмещен | String | Самозаверяющий маркер JWT, используемый в качестве подтверждения наличия существующих ключей. Маркер JWT должен быть подписан с использованием закрытого ключа одного из существующих действительных сертификатов приложения. Маркер должен содержать следующие утверждения:<ul><li>`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</li><li>`iss` — издателем должен быть __идентификатор__  приложения, выполняющего вызов.</li><li>`nbf` — вовремя.</li><li>`exp` — сроком действия должно быть значение "nbf" + 10 минут.</li></ul><br>Ниже приведен [Пример](/graph/application-rollkey-prooftoken) кода, который можно использовать для создания этого маркера для проверки подлинности.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No content`.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removekey-java-snippets.md)]
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
  "description": "application: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


