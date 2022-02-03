---
title: 'синхронизация: секреты'
description: Предоставление учетных данных для установления подключения к целевой системе.
ms.localizationpriority: medium
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 955dc53dcefb499fd3fe8e75e30dc1509d396629
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348778"
---
# <a name="synchronization-secrets"></a>синхронизация: секреты

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставление учетных данных для установления подключения к целевой системе.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     |Directory.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |Не поддерживается. |
|Приложение                            |Application.ReadWrite.OwnedBy, Directory.ReadWrite.All | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/secrets
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|учетные данные|[синхронизацияSecretKeyStringValuePair](../resources/synchronization-synchronizationsecretkeystringvaluepair.md) коллекция|Учетные данные для проверки. Игнорируется при **использовании параметра UseSavedCredentials** `true`.|

## <a name="response"></a>Отклик
Если секреты успешно сохранены, этот метод возвращает код `204 No Content` ответа. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronization_secrets"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/secrets
Content-type: application/json

{
    "value": [
        {
            "key": "BaseAddress",
            "value": "user@domain.com"
        },
        {
            "key": "SecretToken",
            "value": "password-value"
        },
        {
            "key": "SyncNotificationSettings",
            "value": "{\"Enabled\":false,\"DeleteThresholdEnabled\":false}"
        },
        {
            "key": "SyncAll",
            "value": "false"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-secrets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-secrets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-secrets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример ответа. 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronization: secrets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
