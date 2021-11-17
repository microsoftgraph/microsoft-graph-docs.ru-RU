---
title: 'managementAction: применить'
description: Применяет действие управления к определенному управляемому клиенту. При выполнении этой операции будут созданы соответствующие конфигурации и созданы политики. В качестве примера при применении требуемой многофакторной проверки подлинности для действий управления администраторами создается политика условного доступа Azure Active Directory, которая требует многофакторной проверки подлинности для всех пользователей, на которых назначена роль административного каталога.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 25b60d217a312a28210106b62f609c07384de904
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980960"
---
# <a name="managementaction-apply"></a>managementAction: применить
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Применяет действие управления к определенному управляемому клиенту. При выполнении этой операции будут созданы соответствующие конфигурации и созданы политики. В качестве примера при применении требуемой многофакторной проверки подлинности для действий управления администраторами создается политика условного доступа Azure Active Directory, которая требует многофакторной проверки подлинности для всех пользователей, на которых назначена роль административного каталога.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)|
|tenantGroupId|Строка|Идентификатор группы клиента.|
|managementTemplateId|String|Идентификатор шаблона [управления](../resources/managedtenants-managementtemplate.md).|

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код ответа и `200 OK` [управлениеActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managementaction_apply"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
Content-Type: application/json

{
  "tenantId": "String",
  "tenantGroupId": "String",
  "managementTemplateId": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementaction-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementaction-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementaction-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementaction-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/managementaction-apply-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.managedTenants.ManagementActionDeploymentStatus",
  "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
  "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9",
  "status": "completed",
  "workloadActionDeploymentStatuses": [
    {
      "actionId": "46b80b42-06c7-45b4-b6fb-aa0aecace87b",
      "status": "completed",
      "deployedPolicyId": null,
      "lastDeploymentDateTime": "2021-07-11T19:35:10.4463799Z",
      "error": null
    }
  ]
}
```
