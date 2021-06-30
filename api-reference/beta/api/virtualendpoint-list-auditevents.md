---
title: Перечисление объектов auditEvent
description: Получите список объектов cloudPcAuditEvent и их свойств.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 9c775798982d558347b4431f80056a8f7f5d40ea
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211380"
---
# <a name="list-auditevents"></a><span data-ttu-id="49260-103">Перечисление объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="49260-103">List auditEvents</span></span>

<span data-ttu-id="49260-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49260-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49260-105">Список всех [объектов cloudPcAuditEvent](../resources/cloudpcauditevent.md) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49260-105">List all the [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects for the tenant.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="49260-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49260-106">Permissions</span></span>

<span data-ttu-id="49260-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49260-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49260-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49260-109">Permission type</span></span>|<span data-ttu-id="49260-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49260-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49260-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49260-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49260-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49260-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="49260-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49260-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49260-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49260-114">Not supported.</span></span>|
|<span data-ttu-id="49260-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="49260-115">Application</span></span>|<span data-ttu-id="49260-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49260-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49260-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49260-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49260-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49260-118">Optional query parameters</span></span>

<span data-ttu-id="49260-119">Этот метод поддерживает `$skiptoken` и `$top` `$filter` параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49260-119">This method supports `$skiptoken`, `$top` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="49260-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="49260-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="49260-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49260-121">Request headers</span></span>

| <span data-ttu-id="49260-122">Имя</span><span class="sxs-lookup"><span data-stu-id="49260-122">Name</span></span>          | <span data-ttu-id="49260-123">Описание</span><span class="sxs-lookup"><span data-stu-id="49260-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="49260-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49260-124">Authorization</span></span> | <span data-ttu-id="49260-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49260-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49260-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49260-127">Request body</span></span>

<span data-ttu-id="49260-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49260-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49260-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="49260-129">Response</span></span>

<span data-ttu-id="49260-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPcAuditEvent](../resources/cloudpcauditevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49260-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49260-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="49260-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49260-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="49260-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_cloudpcauditevent"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents
```

### <a name="response"></a><span data-ttu-id="49260-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="49260-133">Response</span></span>

><span data-ttu-id="49260-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49260-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```
