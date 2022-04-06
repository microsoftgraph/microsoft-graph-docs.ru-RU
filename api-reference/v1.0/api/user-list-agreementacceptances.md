---
title: Перечисление agreementAcceptances
description: Извлечение списка объектов agreementAcceptance пользователя.
ms.localizationpriority: medium
author: raprakasMSFT
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c9ba2f97837742b87e664bb3f3e450065729d022
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516005"
---
# <a name="list-agreementacceptances"></a>Перечисление agreementAcceptances

Пространство имен: microsoft.graph

Извлечение объектов пользовательского [соглашения, подписанных пользователем](../resources/agreementacceptance.md) .
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AgreementAcceptance.Read |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/agreementAcceptances

# where the id or userPrincipalName is the signed-in user's

GET /users/{id | userPrincipalName}/agreementAcceptances
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `200 OK` отклика и коллекцию [объектов agreementAcceptance](../resources/agreementacceptance.md) в тексте ответа.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/agreementAcceptances
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-agreementacceptances-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-agreementacceptances-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#agreementAcceptances",
    "value": [
        {
            "id": "94410bbf-3d3e-4683-8149-f034e55c39dd_d4bb5206-77bf-4d5c-96b4-cf7b0ed3be98",
            "agreementId": "94410bbf-3d3e-4683-8149-f034e55c39dd",
            "userId": "d4bb5206-77bf-4d5c-96b4-cf7b0ed3be98",
            "deviceId": "00000000-0000-0000-0000-000000000000",
            "deviceDisplayName": null,
            "deviceOSType": null,
            "deviceOSVersion": null,
            "agreementFileId": "08033369-8972-42a3-8533-90bbd2757a01",
            "userDisplayName": "Megan Bowen",
            "userPrincipalName": "MeganB@M365x43961174.OnMicrosoft.com",
            "userEmail": "MeganB@M365x43961174.OnMicrosoft.com",
            "recordedDateTime": "2022-03-04T14:11:22.6658376Z",
            "expirationDateTime": null,
            "state": "accepted"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
