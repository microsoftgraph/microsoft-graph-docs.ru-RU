---
title: 'servicePrincipal: Ремовекэй'
description: Удаление ключа учетных данных из servicePrincipal
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29e1c9589717797f6e4a6354d4b19d2bc5d924a8
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291092"
---
# <a name="serviceprincipal-removekey"></a>servicePrincipal: Ремовекэй

Пространство имен: microsoft.graph

Удаление ключевых учетных данных из [servicePrincipal](../resources/serviceprincipal.md). Этот метод вместе с [аддкэй](serviceprincipal-addkey.md) можно использовать в servicePrincipal для автоматизации изкрутки ключей истечения срока действия.

> [!NOTE]
> [Создание servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) и [обновление операций servicePrincipal](../api/serviceprincipal-update.md) можно продолжать использовать для добавления и обновления ключевых учетных данных для любых servicePrincipal с контекстом пользователя или без него.

В рамках проверки запроса для этого метода проверяется наличие проверки на наличие существующего ключа перед выполнением действия.

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
POST /serviceprincipals/{id}/removeKey
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание                |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса

В тексте запроса укажите следующие обязательные свойства.

| Свойство  | Тип | Описание|
|:----------|:-----|:-----------|
| Него значение KeyID     | Идентификатор GUID | Уникальный идентификатор пароля.|
| совмещен | String | Самозаверяющий маркер JWT, используемый в качестве подтверждения наличия существующих ключей. Этот маркер JWT должен быть подписан с помощью закрытого ключа одного из существующих действительных сертификатов servicePrincipal. Маркер должен содержать следующие утверждения:<ul><li>`aud`Необходимо указать аудиторию `00000002-0000-0000-c000-000000000000` .</li><li>`iss`-Issuer должен быть __идентификатором__ servicePrincipal, осуществляющим вызов.</li><li>`nbf`— Не до времени.</li><li>`exp`— Срок действия должен быть "NBF" + 10 минут.</li></ul><br>Ниже приведен [Пример](/graph/application-rollkey-prooftoken) кода, который можно использовать для создания этого маркера для проверки подлинности.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No content`.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/v1.0/serviceprincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```

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