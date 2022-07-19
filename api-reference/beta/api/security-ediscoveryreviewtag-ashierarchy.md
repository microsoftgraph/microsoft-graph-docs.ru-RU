---
title: 'ediscoveryReviewTag: asHierarchy'
description: Перечисление тега как иерархии*
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 55ad928218c08ab742cdc44bce565a9df04779b7
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838047"
---
# <a name="ediscoveryreviewtag-ashierarchy"></a>ediscoveryReviewTag: asHierarchy
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Выводит список тегов проверки обнаружения](../resources/security-ediscoveryreviewtag.md) электронных данных с показанной иерархией тегов.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags/asHierarchy
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения `200 OK` эта функция возвращает код отклика и коллекцию [microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewtagthis.ashierarchy"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/asHierarchy
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoveryreviewtagthisashierarchy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoveryreviewtagthisashierarchy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoveryreviewtagthisashierarchy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoveryreviewtagthisashierarchy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/ediscoveryreviewtagthisashierarchy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryReviewTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(ediscoveryReviewTag)",
    "@odata.count": 5,
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "My tag API 2",
            "description": "Use Graph API to create tags (updated)",
            "lastModifiedDateTime": "2022-05-30T00:27:41.6407249Z",
            "childSelectability": "Many",
            "id": "062de822f17a4a2e9b833aa3f6c37108",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "Responsive",
            "description": "",
            "lastModifiedDateTime": "2022-05-23T19:41:24.4237284Z",
            "childSelectability": "One",
            "id": "d3d99dc704a74801b792b3e1e722aa0d",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "Not responsive",
            "lastModifiedDateTime": "2022-05-23T19:41:31.3381716Z",
            "childSelectability": "One",
            "id": "ced26633616a434abd83762d49a25a6c",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "Processing",
            "description": "Determine whether to outsource processing",
            "lastModifiedDateTime": "2022-05-23T19:46:03.8746996Z",
            "childSelectability": "Many",
            "id": "d8580989505c4fb3a25b845013697cf7",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "childTags": []
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
            "displayName": "My tag API",
            "description": "Use Graph API to create tags",
            "lastModifiedDateTime": "2022-05-23T19:58:26.1573076Z",
            "childSelectability": "Many",
            "id": "7c6cc351-fb90-431f-8562-1b607a3144a4",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                },
                "application": {
                    "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                    "displayName": "Graph Explorer"
                }
            },
            "childTags": []
        }
    ]
}
```

