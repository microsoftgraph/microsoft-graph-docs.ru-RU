---
title: Приемки списков
description: Сведения о записях приемки для определенного соглашения.
author: raprakasMSFT
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0b5748c3b46ac3411be9f528251897fc0bbc0ca4
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516205"
---
# <a name="list-acceptances"></a>Приемки списков
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о записях приемки для определенного соглашения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AgreementAcceptance.Read, AgreementAcceptance.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/termsOfUse/agreements/{agreementsId}/acceptances
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод позволяет `$select` настроить параметры `$filter` запроса OData и OData. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` отклика и коллекцию [объектов agreementAcceptance](../resources/agreementacceptance.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_agreementacceptance"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/acceptances
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-agreementacceptance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-agreementacceptance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-agreementacceptance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-agreementacceptance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-agreementacceptance-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.agreementAcceptance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#agreementAcceptances",
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
            "userPrincipalName": "MeganB@Contoso.com",
            "userEmail": "MeganB@Contoso.com",
            "recordedDateTime": "2022-03-04T14:11:22.6658376Z",
            "expirationDateTime": null,
            "state": "accepted"
        }
    ]
}
```

