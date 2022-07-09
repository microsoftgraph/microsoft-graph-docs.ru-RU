---
title: Список решений
description: Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fc510b9537c42d5afef3620ad7f019f364e26e5d
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696610"
---
# <a name="list-decisions"></a>Список решений
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) для определенного [объекта accessReviewInstance](../resources/accessreviewinstance.md). Возвращается список из нуля или более объектов accessReviewInstanceDecisionItem, включая все их вложенные свойства.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает `$select`параметры `$filter`запроса , `$orderBy`, и `$skip``$top` OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

Размер страницы по умолчанию для этого API — 100 **объектов accessReviewInstance** . Чтобы повысить эффективность и избежать времени ожидания из-за больших результирующих наборов, примените разбиение на страницы с помощью `$skip` `$top` параметров запроса и параметров запроса. Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и коллекцию объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-all-decisions-for-an-instance-of-an-access-review"></a>Пример 1. Получение всех решений для экземпляра проверки доступа

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "userDisplayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "displayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            }
        },
        {
            "id": "4bde8d40-9224-4aa3-936b-08d73e1baf47",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/11feb738-0039-4a6c-a045-dcb91a47969a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "userDisplayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "displayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            }
        }
    ]
}
```


### <a name="example-2-retrieve-all-decision-items-for-which-youre-a-reviewer-and-expand-the-definitions"></a>Пример 2. Получение всех элементов принятия решений, для которых вы являетесь рецензентом, и развертывание определений

#### <a name="request"></a>Запрос
В следующем примере показан запрос на получение всех решений по каждому экземпляру и определение, для которого вызывающий пользователь является рецензентом.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_expand"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')?$expand=instance($expand=definition)
```
# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewinstancedecisionitem-expand-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-accessreviewinstancedecisionitem-expand-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessReviewInstanceDecisionItems",
    "@odata.count": 10,
    "value": [
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "Adele Vance",
                    "userPrincipalName": "adele@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "b4cbd87c-0ee2-4647-a7e3-41b580ea6fed",
                "displayName": "Priviliged Role Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "Adele Vance",
                    "userPrincipalName": "adele@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "f1edce7a-edad-49fb-83eb-b7f1eda48dd2",
                "displayName": "Global Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "John Doe",
                    "userPrincipalName": "johndoe@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "f1edce7a-edad-49fb-83eb-b7f1eda48dd2",
                "displayName": "Global Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "2e8e717b-a857-49f0-918a-013cf0415456",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "John Doe 1",
                    "userPrincipalName": "johndoe1@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "20a97808-56dd-490a-97a9-73bf2344cce7",
                "displayName": "Hello world",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        }
    ]
}
```
