---
title: Создание appManagementPolicy
description: Создание политики управления приложениями.
localization_priority: Normal
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9553accf83925e1ab33c36f353a7ca74da6ad623
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262411"
---
# <a name="create-appmanagementpolicy"></a>Создание appManagementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание [объекта appManagementPolicy.](../resources/appManagementPolicy.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                |
| :------------------------------------- | :--------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Policy.ReadWrite.ApplicationConfiguration |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                             |
| Приложение                            | Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /policies/appManagementPolicies
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса укажи JSON представление [appManagementPolicy.](../resources/appManagementPolicy.md)

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа с новым объектом `201 Created` [appManagementPolicy ](../resources/appmanagementpolicy.md) в полезной нагрузке ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса. В этом запросе создана политика управления приложениями со следующими настройками:

- Включает политику.
- Блокирует создание новых паролей для приложений и директоров служб после 2019-10-19 в 10:37 по времени UTC.
- Ограничивает секреты паролей для приложений и главных служб, созданных после 2019-10-19 в 10:37 по времени UTC, менее чем за 20 дней.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_appManagementPolicy"
}-->

```http
POST https://graph.microsoft.com/beta/policies/appManagementPolicies

{
    "displayName": "Credential management policy",
    "description": "Cred policy sample",
    "isEnabled": true,
    "restrictions": {
        "passwordCredentials": [
            {
                "restrictionType": "passwordAddition",
                "maxLifetime": null,
                "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z"
            },
            {
                "restrictionType": "passwordLifetime",
                "maxLifetime": "P4DT12H30M5S",
                "restrictForAppsCreatedAfterDateTime": "2018-10-19T10:37:00Z"
            }
        ]
    }
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-appmanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-appmanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-appmanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-appmanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/appManagementPolicies/$entity",
    "id": "a4ab1ed9-46bb-4bef-88d4-86fd6398dd5d",
    "displayName": "credential management policy",
    "description": "Lorem ipsum",
    "isEnabled": true,
    "restrictions": {
        "passwordCredentials": [
            {
                "restrictionType": "passwordAddition",
                "maxLifetime": null,
                "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z"
            },
            {
                "restrictionType": "passwordLifetime",
                "maxLifetime": "P4DT12H30M5S",
                "restrictForAppsCreatedAfterDateTime": "2018-10-19T10:37:00Z"
            }
        ]
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "create appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
