---
title: Обновление unifiedRoleManagementPolicyRule
description: Обновление правила, определенного для политики управления ролем.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a32f562a86ed72d8da728973ca6c5b5a5db7fcbb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204425"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a>Обновление unifiedRoleManagementPolicyRule
Пространство имен: microsoft.graph

Обновление правила, определенного для политики управления ролем. Правило может быть одним из следующих типов, производных от объекта [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) :
+ [unifiedRoleManagementPolicyApprovalRule](../resources/unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](../resources/unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](../resources/unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](../resources/unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](../resources/unifiedrolemanagementpolicynotificationrule.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|claimValue|Строка|Значение утверждения контекста проверки подлинности. <br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyAuthenticationContextRule** .|
|enabledRules|Коллекция строк|Коллекция правил, включенных для этого правила политики. Например, `MultiFactorAuthentication`и `Ticketing``Justification`.<br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyEnablementRule** .|
|isDefaultRecipientsEnabled|Логическое|Указывает, будет ли получатель по умолчанию получать уведомление по электронной почте.<br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyNotificationRule** .|
|isEnabled|Boolean| Указывает, включено ли это правило. <br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyAuthenticationContextRule** .|
|isExpirationRequired|Логическое|Указывает, требуется ли срок действия, является ли это постоянно активным назначением или допустимостью. <br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyExpirationRule** .|
|maximumDuration|Длительность| Максимальная длительность, допустимая для допустимости или назначения, которая не является постоянной. Требуется, если **isExpirationRequired** имеет значение `true`. <br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyExpirationRule** . |
|notificationLevel|Строка|Уровень уведомления. Возможные значения: `None`, `Critical`. `All`<br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyNotificationRule** .|
|notificationRecipients|Коллекция String|Список получателей уведомлений по электронной почте.<br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyNotificationRule** .|
|notificationType|Строка|Тип уведомления. Поддерживается `Email` только.<br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyNotificationRule** .|
|recipientType|String|Тип получателя уведомления. Возможные значения: `Requestor`, `Approver`. `Admin`<br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyNotificationRule** .|
|setting|[approvalSettings](../resources/approvalsettings.md)|Параметры для утверждения назначения роли. <br/><br/>Может быть обновлен для типа **правила unifiedRoleManagementPolicyApprovalRule** .|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения об области, предназначенной для правила политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. <br/><br/> Может быть обновлен для всех типов правил.|

>**Примечание:** Свойство `@odata.type` со значением определенного типа правила должно быть включено в текст. Например, `"@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule"`.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

В следующем примере обновляется правило политики управления ролами типа **unifiedRoleManagementPolicyExpirationRule** и с идентификатором `Expiration_EndUser_Assignment`.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedrolemanagementpolicyrule"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/policies/roleManagementPolicies/DirectoryRole_84841066-274d-4ec0-a5c1-276be684bdd3_200ec19a-09e7-4e7a-9515-cf1ee64b96f9/rules/Expiration_EndUser_Assignment
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
    "id": "Expiration_EndUser_Assignment",
    "isExpirationRequired": true,
    "maximumDuration": "PT1H45M",
    "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
        "caller": "EndUser",
        "operations": [
            "All"
        ],
        "level": "Assignment",
        "inheritableSettings": [],
        "enforcedSettings": []
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedrolemanagementpolicyrule-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

