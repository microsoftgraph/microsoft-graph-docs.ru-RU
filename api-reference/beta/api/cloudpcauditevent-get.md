---
title: Get cloudPcAuditEvent
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcAuditEvent.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1848aa35f9c4b1f31159d950e946e898ff84ad1c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211322"
---
# <a name="get-cloudpcauditevent"></a><span data-ttu-id="0ff7a-103">Get cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="0ff7a-103">Get cloudPcAuditEvent</span></span>

<span data-ttu-id="0ff7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ff7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ff7a-105">Ознакомьтесь с свойствами и отношениями объекта [cloudPcAuditEvent.](../resources/cloudpcauditevent.md)</span><span class="sxs-lookup"><span data-stu-id="0ff7a-105">Read the properties and relationships of a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="0ff7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ff7a-106">Permissions</span></span>

<span data-ttu-id="0ff7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ff7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ff7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ff7a-109">Permission type</span></span>| <span data-ttu-id="0ff7a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ff7a-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="0ff7a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ff7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ff7a-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff7a-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="0ff7a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ff7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ff7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ff7a-114">Not supported.</span></span>|
|<span data-ttu-id="0ff7a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ff7a-115">Application</span></span>|<span data-ttu-id="0ff7a-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ff7a-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ff7a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ff7a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ff7a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ff7a-118">Request headers</span></span>

| <span data-ttu-id="0ff7a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ff7a-119">Name</span></span>          | <span data-ttu-id="0ff7a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ff7a-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0ff7a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ff7a-121">Authorization</span></span> | <span data-ttu-id="0ff7a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ff7a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ff7a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ff7a-124">Request body</span></span>

<span data-ttu-id="0ff7a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ff7a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ff7a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ff7a-126">Response</span></span>

<span data-ttu-id="0ff7a-127">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект cloudPcAuditEvent](../resources/cloudpcauditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ff7a-127">If successful, this method returns a `200 OK` response code and a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ff7a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ff7a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ff7a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ff7a-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_cloudpcauditevent"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/{id}
```

### <a name="response"></a><span data-ttu-id="0ff7a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ff7a-130">Response</span></span>

><span data-ttu-id="0ff7a-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ff7a-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcAuditEvent"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
      "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
      "id": "250473f5-029f-4037-813d-ba4768201d61",
      "displayName": "Display Name value",
      "componentName": "Component Name value",  
      "activity": "Activity value",  
      "activityDateTime": "2021-02-14T13:10:51.814636+08:00",  
      "activityType": " Activity Type value",  
      "activityOperationType": "Activity Operation Type value",  
      "activityResult": "Activity Result value",  
      "correlationId": "a5c71cc6-2271-4d5c-9bfe-d94781e83fe6",  
      "category": "Category value",
      "actor": {
          "@odata.type": "microsoft.graph.cloudPcAuditActor",
          "type": "Type value",
          "userPermissions": [
              "User Permissions value"
          ],
          "applicationId": "Application Id value",
          "applicationDisplayName": "Application Display Name value",
          "userPrincipalName": "User Principal Name value",
          "servicePrincipalName": "Service Principal Name value",
          "ipAddress": "Ip Address value",
          "userId": "User Id value",
          "userRoleScopeTags": [
              {
                  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
                  "displayName": "Display Name value",
                  "roleScopeTagId": "Role Scope Tag Id value"
              }
          ],
          "remoteTenantId": "Remote Tenant Id value",
          "remoteUserId": "Remote User Id value"
      },
      "resources": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.cloudPcAuditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
  }
}
```
