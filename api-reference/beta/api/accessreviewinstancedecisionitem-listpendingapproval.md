---
title: Список ожидающих утверждения АкцессревиевинстанцедеЦисионитем
description: Получение объектов АкцессревиевинстанцедеЦисионитем, ожидающих утверждения вызывающим пользователем.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e245d58966b1fa6e206dff1c7a29f38a3146ac21
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000987"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval"></a>Список ожидающих утверждения АкцессревиевинстанцедеЦисионитемс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объектов [акцессревиевинстанцедеЦисионитем](../resources/accessreviewinstance.md) для определенных [акцессревиевинстанце](../resources/accessreviewscheduledefinition.md) , ожидающих утверждения вызывающим пользователем. Возвращается список из нуля или более объектов АкцессревиевинстанцедеЦисионитем, включая все вложенные свойства.

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

Кроме того, вошедшего в систему пользователя будут отображаться только те решения, которым назначен проверяющий в инстанце'с Акцессревиевсчедуледефинитион.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```
## <a name="request-headers"></a>Заголовки запросов
Нет.

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиевинстанцедеЦисионитем](../resources/accessreviewinstance.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос
В приведенном ниже примере показан запрос на получение всех решений для экземпляра проверки доступа, ожидающей утверждения вызывающего пользователя.

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```

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
    "@odata.count": 2,
    "value": [
        {
            "id": "654b34e7-b48f-4772-a2d4-08f1d0dd014c",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
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
                "userId": "7eae986b-d425-48b2-adf2-3c777f6256f3",
                "userDisplayName": "Adele Vance",
                "userPrincipalName": "AdeleV@microsoft.com"
            }
        },
        {
            "id": "0311dba4-c60c-412e-ac77-14e1da23daf1",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
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
                "userId": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "userDisplayName": "MOD Administrator",
                "userPrincipalName": "admin@microsoft.com"
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
  "description": "List accessReviewInstanceDecisionItem pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
