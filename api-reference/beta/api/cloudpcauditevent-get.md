---
title: Get cloudPcAuditEvent
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcAuditEvent.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 9dc44e92d4e332a2e682c25f525d72faa7a62847
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316891"
---
# <a name="get-cloudpcauditevent"></a><span data-ttu-id="f392b-103">Get cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="f392b-103">Get cloudPcAuditEvent</span></span>

<span data-ttu-id="f392b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f392b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f392b-105">Ознакомьтесь с свойствами и отношениями объекта [cloudPcAuditEvent.](../resources/cloudpcauditevent.md)</span><span class="sxs-lookup"><span data-stu-id="f392b-105">Read the properties and relationships of a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="f392b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f392b-106">Permissions</span></span>

<span data-ttu-id="f392b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f392b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f392b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f392b-109">Permission type</span></span>| <span data-ttu-id="f392b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f392b-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="f392b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f392b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f392b-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f392b-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f392b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f392b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f392b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f392b-114">Not supported.</span></span>|
|<span data-ttu-id="f392b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f392b-115">Application</span></span>|<span data-ttu-id="f392b-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f392b-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f392b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f392b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f392b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f392b-118">Request headers</span></span>

| <span data-ttu-id="f392b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f392b-119">Name</span></span>          | <span data-ttu-id="f392b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f392b-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f392b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f392b-121">Authorization</span></span> | <span data-ttu-id="f392b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f392b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f392b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f392b-124">Request body</span></span>

<span data-ttu-id="f392b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f392b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f392b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f392b-126">Response</span></span>

<span data-ttu-id="f392b-127">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект cloudPcAuditEvent](../resources/cloudpcauditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f392b-127">If successful, this method returns a `200 OK` response code and a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f392b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f392b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f392b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f392b-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f392b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f392b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcauditevent"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/{id}
```
# <a name="c"></a>[<span data-ttu-id="f392b-131">C#</span><span class="sxs-lookup"><span data-stu-id="f392b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcauditevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f392b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f392b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcauditevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f392b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f392b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcauditevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f392b-134">Java</span><span class="sxs-lookup"><span data-stu-id="f392b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcauditevent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f392b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f392b-135">Response</span></span>

><span data-ttu-id="f392b-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f392b-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
