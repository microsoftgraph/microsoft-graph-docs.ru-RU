---
title: 'accessPackage: getApplicablePolicyRequirements'
description: Разрешить звонителям находить требования для запроса назначения для определенного accessPackage.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 14491683e302c89b41d5b01b3ea627e41999e0c1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340729"
---
# <a name="accesspackage-getapplicablepolicyrequirements"></a>accessPackage: getApplicablePolicyRequirements
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](../resources/entitlementmanagement-overview.md) это действие извлекает список объектов [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) , которые в настоящее время пользователь может использовать для создания [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).  Каждый объект требования соответствует политике назначения пакетов доступа, для которых подписанное в настоящее время пользователь может запрашивать назначение.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/getApplicablePolicyRequirements
```

## <a name="function-parameters"></a>Параметры функции

Нет.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не поставляем тело запроса для этого метода, если вы хотите получить список требований пакета доступа, как в примере 1. Если вы хотите получить требования политики для области пользователей, как в примере 2, необходимо предоставить тело запроса.

## <a name="response"></a>Отклик
`200 OK` В случае успешного выполнения этот метод возвращает код ответа и коллекцию [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) в тексте отклика, по одному объекту для каждой политики, для которой пользователь является **разрешеннымRequestor**. Если политика не имеет требований, то будут иметься и значения **accessPackageAssignmentRequestRequirements** `false` `null` . Если нет политик, в которых пользователь является **разрешеннымRequestor**, вместо него будет возвращена пустая коллекция.

## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-a-list-of-access-package-requirements-to-create-an-access-package"></a>Пример 1. Извлечение списка требований пакета доступа для создания пакета доступа

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackage_getapplicablepolicyrequirements"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/fb449cf8-3a59-4d86-bdfd-a1b7299681de/getApplicablePolicyRequirements
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackage-getapplicablepolicyrequirements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackage-getapplicablepolicyrequirements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackage-getapplicablepolicyrequirements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackage-getapplicablepolicyrequirements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackage-getapplicablepolicyrequirements-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/accesspackage-getapplicablepolicyrequirements-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequestRequirements)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "policyId": "d6322c23-04d6-eb11-b22b-c8d9d21f4e9a",
            "policyDisplayName": "Initial Policy",
            "policyDescription": "Initial Policy",
            "isApprovalRequired": false,
            "isApprovalRequiredForExtension": false,
            "isRequestorJustificationRequired": false,
            "questions": [
                {
                    "@odata.type": "#microsoft.graph.textInputQuestion",
                    "id": "0fd349e2-a3a7-4712-af08-660f29c12b90",
                    "isRequired": true,
                    "isAnswerEditable": null,
                    "sequence": 0,
                    "isSingleLineQuestion": true,
                    "text": {
                        "defaultText": "What is your display name",
                        "localizedTexts": []
                    }
                }
            ],
            "existingAnswers": [],
            "schedule": []
        }
    ]
}
``` 

### <a name="example-2-get-policy-requirements-for-a-given-user-scope"></a>Пример 2. Получить требования к политике для данной области пользователей

#### <a name="request"></a>Запрос

<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/accessPackages(‘b15419bb-5ffc-ea11-b207-c8d9d21f4e9a’)/getApplicablePolicyRequirements

{
        "subject": {
            "objectId": "5acd375c-8acb-45de-a958-fa0dd89259ad"
        }
    }
```



#### <a name="response"></a>Отклик

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "policyId": "d6322c23-04d6-eb11-b22b-c8d9d21f4e9a",
            "policyDisplayName": "Initial Policy",
            "policyDescription": "Initial Policy",
            "isApprovalRequired": false,
            "isApprovalRequiredForExtension": false,
            "isRequestorJustificationRequired": false,
            "questions": [
                {
                    "@odata.type": "#microsoft.graph.textInputQuestion",
                    "id": "5a7f2a8f-b802-4438-bec6-09599bc43e13",
                    "isRequired": false,
                    "isAnswerEditable": true,
                    "sequence": 0,
                    "isSingleLineQuestion": true,
                    "text": {
                        "defaultText": "Enter your mail",
                        "localizedTexts": []
                    }
                }
            ],
            "existingAnswers": [
                {
                    "@odata.type": "#microsoft.graph.answerString",
                    "displayValue": "admin@contoso.com",
                    "value": "admin@contoso.com",
                    "answeredQuestion": {
                        "@odata.type": "#microsoft.graph.textInputQuestion",
                        "id": "5a7f2a8f-b802-4438-bec6-09599bc43e13",
                        "isRequired": false,
                        "isAnswerEditable": true,
                        "sequence": 0,
                        "isSingleLineQuestion": true,
                        "text": {
                            "defaultText": "Enter your mail",
                            "localizedTexts": []
                        }
                    }
                }
            ],
            "schedule": []
        }
    ]
}
```
