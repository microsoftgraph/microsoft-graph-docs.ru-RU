---
title: Список АкцессревиевинстанцедеЦисионитем
description: Получение объектов АкцессревиевинстанцедеЦисионитем.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 65f74fc94af433d0ecd545a33cef4e0022c387d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214375"
---
# <a name="list-accessreviewinstancedecisionitem"></a>Список АкцессревиевинстанцедеЦисионитем

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объектов [акцессревиевинстанцедеЦисионитем](../resources/accessreviewinstancedecisionitem.md) для определенного [акцессревиевинстанце](../resources/accessreviewinstance.md). Возвращается список из нуля или более объектов АкцессревиевинстанцедеЦисионитем, включая все вложенные свойства.

>[!NOTE]
>Если возвращается множество **акцессревиевинстанцедеЦисионитемс** , чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на страницы, включив в него как параметр запроса $Top, который содержит не более 100, и параметр запроса $Skip = 0 в запросе. Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с помощью свойства @odata. nextLink в ответе, который содержит URL-адрес следующей страницы результатов. При наличии этого свойства Продолжайте делать дополнительные запросы с URL-адресом @odata. nextLink в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе разбиение данных Microsoft Graph в приложении.
>
>Если не указано ни одного параметра запроса и число результатов превышает 100, Microsoft Graph автоматически разбивать результаты на страницы 100 на каждой странице.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL  |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение                            | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL |

 Вошедшего в систему пользователя также должен находиться в роли каталога, который позволяет им читать проверку доступа.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```
## <a name="request-headers"></a>Заголовки запросов
Нет.

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиевинстанцедеЦисионитем](../resources/accessreviewinstance.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос
В приведенном ниже примере показан запрос на получение всех решений для экземпляра проверки доступа.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
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

---


---

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
    "@odata.count": 4,
    "value": [
        {
            "id": "77a61af9-3bef-4bbf-b00b-04734d6d5eae",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
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
                "userId": "3736c87b-dc21-4290-8802-d6fef5fa3a08",
                "userDisplayName": "Irvin Sayers",
                "userPrincipalName": "IrvinS@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "f30b68ef-b843-4479-86b8-0a3a2f4bb209",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:08.377Z",
            "decision": "Approve",
            "justification": "This employee needs access for reason X",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "ecd78419-3f1e-4f07-9bd9-7c77137af4f1",
                "userDisplayName": "Bianca Pisani",
                "userPrincipalName": "BiancaP@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "037b737f-e8ca-4507-b126-5a0620ba2c18",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:28.473Z",
            "decision": "Deny",
            "justification": "This employee changed roles and no longer needs access",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "5f16b75b-031c-4944-9691-070f03273079",
                "userDisplayName": "Delia Dennis",
                "userPrincipalName": "DeliaD@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "7032f455-10a3-4d04-bf02-66fb65d26d10",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:44.38Z",
            "decision": "DontKnow",
            "justification": "I do not know what this employee needs",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "4169762e-895f-4350-a13d-e5b09b1efcfa",
                "userDisplayName": "Isaiah Langer",
                "userPrincipalName": "IsaiahL@M365x471116.OnMicrosoft.com"
            }
        }
    ]
}
```

## <a name="see-also"></a>См. также

- [Получение Акцессревиевсчедуледефинитион](accessreviewscheduledefinition-get.md)
- [Получение Акцессревиевинстанце](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
