---
title: 'servicePrincipal: removeKey'
description: Удаление учетных данных ключа из службыPrincipal
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e834455f015966e59b2a668461ca6054eb21b03b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63331962"
---
# <a name="serviceprincipal-removekey"></a>servicePrincipal: removeKey

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление учетных данных ключей из [службыPrincipal](../resources/serviceprincipal.md). Этот метод вместе с [addKey](serviceprincipal-addkey.md) можно использовать службойPrincipal для автоматизации проката истекающих ключей.

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
POST /serviceprincipals/{id}/removeKey
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажи следующие необходимые свойства.

| Свойство  | Тип | Описание|
|:----------|:-----|:-----------|
| keyId     | Guid | Уникальный идентификатор пароля.|
| доказательство | String | Самозаверяемый маркер JWT, используемый в качестве доказательства владения существующими ключами. Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов службыPrincipal. Маркер должен содержать следующие утверждения:<ul><li>`aud` — требуется использовать аудиторию `00000002-0000-0000-c000-000000000000`.</li><li>`iss` - Эмитент должен быть __id__  службыPrincipal, которая делает вызов.</li><li>`nbf` — вовремя.</li><li>`exp` - Срок действия должен быть `nbf` + 10 минут.</li></ul><br>Действия по созданию этого маркера владения см. в журнале [Generating proof of possession tokens for rolling keys](/graph/application-rollkey-prooftoken).|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No content`.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removekey-javascript-snippets.md)]
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



