---
title: 'managementActionTenantDeploymentStatus: changeDeploymentStatus'
description: Изменение состояния развертывания уровня клиента для действия управления. Эти сведения используются для получения сведений о том, какие действия управления находятся в определенном состоянии. В качестве примера может быть план применения многофакторной проверки подлинности для администраторов, поэтому было бы идеально изменить состояние на запланированное, чтобы отразить соответствующий статус.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 01c7efcbea39f9360e9c1356103db89e7021df1e
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60947282"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a>managementActionTenantDeploymentStatus: changeDeploymentStatus
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изменение состояния развертывания уровня клиента для действия управления. Эти сведения используются для получения сведений о том, какие действия управления находятся в определенном состоянии. В качестве примера может быть план применения многофакторной проверки подлинности для администраторов, поэтому было бы идеально изменить состояние на запланированное, чтобы отразить соответствующий статус.

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
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
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
|tenantGroupId|String|Идентификатор группы клиента.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)|
|managementActionId|String|Идентификатор для действия [управления](../resources/managedtenants-managementaction.md).|
|managementTemplateId|String|Идентификатор шаблона [управления.](../resources/managedtenants-managementtemplate.md)|
|status|String|Новый статус развертывания клиента [действия](../resources/managedtenants-managementaction.md) управления.|

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код ответа и `200 OK` [управлениеActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managementactiontenantdeploymentstatus_changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
Content-Type: application/json

{
  "tenantGroupId": "String",
  "tenantId": "String",
  "managementActionId": "String",
  "managementTemplateId": "String",
  "status": "String"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementactiontenantdeploymentstatus-changedeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementactiontenantdeploymentstatus-changedeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementactiontenantdeploymentstatus-changedeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementactiontenantdeploymentstatus-changedeploymentstatus-java-snippets.md)]
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
  "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
  "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
  "status": "planned",
  "workloadActionDeploymentStatuses": []
}
```
