---
title: 'unifiedRoleAssignmentScheduleRequest: filterByCurrentUser'
description: Получить список объектов unifiedRoleAssignmentScheduleRequest и их свойств, отфильтрованных определенным пользователем
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 182ffc04a0c86838eea976c3c77496cba8a92f86
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53333977"
---
# <a name="unifiedroleassignmentschedulerequest-filterbycurrentuser"></a><span data-ttu-id="65d87-103">unifiedRoleAssignmentScheduleRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="65d87-103">unifiedRoleAssignmentScheduleRequest: filterByCurrentUser</span></span>
<span data-ttu-id="65d87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="65d87-105">Получите список объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств, связанных с определенным основным объектом.</span><span class="sxs-lookup"><span data-stu-id="65d87-105">Get a list of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65d87-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65d87-106">Permissions</span></span>
<span data-ttu-id="65d87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65d87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65d87-109">Permission type</span></span>|<span data-ttu-id="65d87-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65d87-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65d87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65d87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65d87-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="65d87-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="65d87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65d87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65d87-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="65d87-114">Not supported</span></span>|
|<span data-ttu-id="65d87-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="65d87-115">Application</span></span>|<span data-ttu-id="65d87-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="65d87-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="65d87-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65d87-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="65d87-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="65d87-118">Query parameters</span></span>
<span data-ttu-id="65d87-119">В следующей таблице показаны параметры запроса, которые можно использовать с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="65d87-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="65d87-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="65d87-120">Parameter</span></span>|<span data-ttu-id="65d87-121">Тип</span><span class="sxs-lookup"><span data-stu-id="65d87-121">Type</span></span>|<span data-ttu-id="65d87-122">Описание</span><span class="sxs-lookup"><span data-stu-id="65d87-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65d87-123">on</span><span class="sxs-lookup"><span data-stu-id="65d87-123">on</span></span>|<span data-ttu-id="65d87-124">RoleAssignmentScheduleRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="65d87-124">RoleAssignmentScheduleRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="65d87-125">Id основного объекта.</span><span class="sxs-lookup"><span data-stu-id="65d87-125">Id of the principal object.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="65d87-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65d87-126">Request headers</span></span>
|<span data-ttu-id="65d87-127">Имя</span><span class="sxs-lookup"><span data-stu-id="65d87-127">Name</span></span>|<span data-ttu-id="65d87-128">Описание</span><span class="sxs-lookup"><span data-stu-id="65d87-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65d87-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65d87-129">Authorization</span></span>|<span data-ttu-id="65d87-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65d87-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65d87-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65d87-132">Request body</span></span>
<span data-ttu-id="65d87-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65d87-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65d87-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="65d87-134">Response</span></span>

<span data-ttu-id="65d87-135">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [унифицированную коллекциюRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="65d87-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65d87-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="65d87-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65d87-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="65d87-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleAssignmentScheduleRequests/filterByCurrentUser(on='d6e4112f-112f-d6e4-2f11-e4d62f11e4d6')
```


### <a name="response"></a><span data-ttu-id="65d87-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="65d87-138">Response</span></span>
<span data-ttu-id="65d87-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="65d87-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "action": "AdminAssign",
      "principalId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "roleDefinitionId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "directoryScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "appScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "isValidationOnly": false,
      "targetScheduleId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "justification": "this is a justification",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "ticketInfo": {
        "@odata.type": "microsoft.graph.ticketInfo"
      }
    }
  ]
}
```

