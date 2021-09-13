---
title: 'servicePrincipal: removeKey'
description: Удаление учетных данных ключа из службыPrincipal
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f6311481eddade52d6f3f2e2898037d4fe493a1c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026062"
---
# <a name="serviceprincipal-removekey"></a>servicePrincipal: removeKey

Пространство имен: microsoft.graph

Удаление учетных данных ключей [из службыPrincipal.](../resources/serviceprincipal.md) Этот метод вместе с [addKey](serviceprincipal-addkey.md) можно использовать службойPrincipal для автоматизации проката истекающих ключей.

> [!NOTE]
> [Создание службыPrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [Update servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления учетных данных для любой службыPrincipal с контекстом пользователя или без него.

В рамках проверки запроса для этого метода проверяется доказательство на наличие существующего ключа перед выполнением действия.

## <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All, Application.ReadWrite.All, Directory.ReadWrite.All   |
|Делегированные (личная учетная запись Майкрософт) | Нет.    |
|Приложение | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removeKey
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажи следующие необходимые свойства.

| Свойство  | Тип | Описание|
|:----------|:-----|:-----------|
| keyId     | GUID | Уникальный идентификатор пароля.|
| доказательство | Строка | Самозаверяемый маркер JWT, используемый в качестве доказательства владения существующими ключами. Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов службыPrincipal. Маркер должен содержать следующие утверждения:<ul><li>`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - Эмитент должен быть __id__  службыPrincipal, которая делает вызов.</li><li>`nbf` — вовремя.</li><li>`exp` — сроком действия должно быть значение "nbf" + 10 минут.</li></ul><br>Вот пример [кода,](/graph/application-rollkey-prooftoken) который можно использовать для создания этого доказательства маркера владения.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No content`.

## <a name="examples"></a>Примеры

В следующем примере показано, как вызвать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-removekey-java-snippets.md)]
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
  "description": "servicePrincipal: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

