---
title: Get unifiedRoleAssignmentScheduleRequest
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f03d053979f8821296a9a3e59e6c7fdd0372735f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299773"
---
# <a name="get-unifiedroleassignmentschedulerequest"></a><span data-ttu-id="53b65-103">Get unifiedRoleAssignmentScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="53b65-103">Get unifiedRoleAssignmentScheduleRequest</span></span>
<span data-ttu-id="53b65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53b65-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="53b65-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53b65-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53b65-106">Permissions</span></span>
<span data-ttu-id="53b65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b65-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53b65-109">Permission type</span></span>|<span data-ttu-id="53b65-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53b65-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b65-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53b65-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53b65-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="53b65-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="53b65-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53b65-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b65-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="53b65-114">Not supported</span></span>|
|<span data-ttu-id="53b65-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53b65-115">Application</span></span>|<span data-ttu-id="53b65-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="53b65-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b65-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b65-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53b65-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53b65-118">Optional query parameters</span></span>
<span data-ttu-id="53b65-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="53b65-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="53b65-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="53b65-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="53b65-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53b65-121">Request headers</span></span>
|<span data-ttu-id="53b65-122">Имя</span><span class="sxs-lookup"><span data-stu-id="53b65-122">Name</span></span>|<span data-ttu-id="53b65-123">Описание</span><span class="sxs-lookup"><span data-stu-id="53b65-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53b65-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53b65-124">Authorization</span></span>|<span data-ttu-id="53b65-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b65-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b65-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53b65-127">Request body</span></span>
<span data-ttu-id="53b65-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53b65-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53b65-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b65-129">Response</span></span>

<span data-ttu-id="53b65-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="53b65-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53b65-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="53b65-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53b65-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="53b65-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```


### <a name="response"></a><span data-ttu-id="53b65-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b65-133">Response</span></span>
<span data-ttu-id="53b65-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="53b65-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
    "action": "String",
    "principalId": "String",
    "roleDefinitionId": "String",
    "directoryScopeId": "String",
    "appScopeId": "String",
    "isValidationOnly": "Boolean",
    "targetScheduleId": "String",
    "justification": "String",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "ticketInfo": {
      "@odata.type": "microsoft.graph.ticketInfo"
    }
  }
}
```

