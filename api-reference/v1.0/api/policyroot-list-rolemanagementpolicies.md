---
title: Перечисление roleManagementPolicies
description: Получение политик управления ролами и их сведений.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 894eba495c2535a0af32227b83afe3ce1a3021bb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315553"
---
# <a name="list-rolemanagementpolicies"></a>Перечисление roleManagementPolicies
Пространство имен: microsoft.graph

Получение политик управления ролами и их сведений.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies?$filter=scopeId eq 'scopeId' and scopeType eq 'scopeType'
```

## <a name="query-parameters"></a>Параметры запроса
Для этого метода требуется параметр `$filter` запроса (`eq`) для области запроса **scopeId** и **scopeType**. Для настройки ответа можно также `$select` `$expand` использовать параметры запроса oData и OData. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-retrieve-the-role-management-policies-that-apply-to-azure-ad-roles"></a>Пример 1. Получение политик управления ролями, которые применяются к Azure AD ролей

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicies?$filter=scopeId eq '/' and scopeType eq 'DirectoryRole'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies",
    "value": [
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        },
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_23b16f1a-1f8d-4891-93b1-21244cdf6115",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        }
    ]
}
```

### <a name="example-2-retrieve-the-role-management-policies-that-apply-to-the-directory-and-expand-the-associated-rules"></a>Пример 2. Получение политик управления ролем, применяемых к каталогу, и развертывание связанных правил

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy_expand_rules"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicies?$filter=scopeId eq '/' and scopeType eq 'Directory'&$expand=rules
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-expand-rules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-expand-rules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-expand-rules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-expand-rules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicy-expand-rules-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies(rules())",
    "value": [
        {
            "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "displayName": "Directory",
            "description": "Directory",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "Directory",
            "lastModifiedDateTime": "2022-04-20T16:12:29.553Z",
            "lastModifiedBy": {
                "displayName": "MOD Administrator",
                "id": null
            },
            "rules@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies('Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448')/rules",
            "rules": [
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                    "id": "Expiration_Admin_Eligibility",
                    "isExpirationRequired": false,
                    "maximumDuration": "P365D",
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Admin_Admin_Eligibility",
                    "notificationType": "Email",
                    "recipientType": "Admin",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Requestor_Admin_Eligibility",
                    "notificationType": "Email",
                    "recipientType": "Requestor",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Approver_Admin_Eligibility",
                    "notificationType": "Email",
                    "recipientType": "Approver",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                    "id": "Enablement_Admin_Eligibility",
                    "enabledRules": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Eligibility",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                    "id": "Expiration_Admin_Assignment",
                    "isExpirationRequired": false,
                    "maximumDuration": "P180D",
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                    "id": "Enablement_Admin_Assignment",
                    "enabledRules": [
                        "Justification"
                    ],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Admin_Admin_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Admin",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Requestor_Admin_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Requestor",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Approver_Admin_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Approver",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "Admin",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                    "id": "Expiration_EndUser_Assignment",
                    "isExpirationRequired": true,
                    "maximumDuration": "PT8H",
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                    "id": "Enablement_EndUser_Assignment",
                    "enabledRules": [
                        "MultiFactorAuthentication",
                        "Justification"
                    ],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
                    "id": "Approval_EndUser_Assignment",
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    },
                    "setting": {
                        "isApprovalRequired": false,
                        "isApprovalRequiredForExtension": false,
                        "isRequestorJustificationRequired": true,
                        "approvalMode": "SingleStage",
                        "approvalStages": [
                            {
                                "approvalStageTimeOutInDays": 1,
                                "isApproverJustificationRequired": true,
                                "escalationTimeInMinutes": 0,
                                "isEscalationEnabled": false,
                                "primaryApprovers": [],
                                "escalationApprovers": []
                            }
                        ]
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
                    "id": "AuthenticationContext_EndUser_Assignment",
                    "isEnabled": false,
                    "claimValue": null,
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Admin_EndUser_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Admin",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Requestor_EndUser_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Requestor",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                },
                {
                    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                    "id": "Notification_Approver_EndUser_Assignment",
                    "notificationType": "Email",
                    "recipientType": "Approver",
                    "notificationLevel": "All",
                    "isDefaultRecipientsEnabled": true,
                    "notificationRecipients": [],
                    "target": {
                        "caller": "EndUser",
                        "operations": [
                            "all"
                        ],
                        "level": "Assignment",
                        "inheritableSettings": [],
                        "enforcedSettings": []
                    }
                }
            ]
        }
    ]
}
```
