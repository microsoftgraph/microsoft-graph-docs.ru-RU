---
title: Get unifiedRoleAssignmentSchedule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentSchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 939ae40260ed127fe36089db5874c7c880b8f8d4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351022"
---
# <a name="get-unifiedroleassignmentschedule"></a><span data-ttu-id="f3566-103">Get unifiedRoleAssignmentSchedule</span><span class="sxs-lookup"><span data-stu-id="f3566-103">Get unifiedRoleAssignmentSchedule</span></span>
<span data-ttu-id="f3566-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3566-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3566-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f3566-105">Read the properties and relationships of an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3566-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3566-106">Permissions</span></span>
<span data-ttu-id="f3566-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3566-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3566-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3566-109">Permission type</span></span>|<span data-ttu-id="f3566-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3566-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3566-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3566-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3566-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f3566-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span></span>|
|<span data-ttu-id="f3566-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3566-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3566-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f3566-114">Not supported</span></span>|
|<span data-ttu-id="f3566-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3566-115">Application</span></span>|<span data-ttu-id="f3566-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f3566-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3566-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3566-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentSchedulesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3566-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3566-118">Optional query parameters</span></span>
<span data-ttu-id="f3566-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="f3566-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f3566-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f3566-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3566-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3566-121">Request headers</span></span>
|<span data-ttu-id="f3566-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f3566-122">Name</span></span>|<span data-ttu-id="f3566-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f3566-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f3566-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3566-124">Authorization</span></span>|<span data-ttu-id="f3566-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3566-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3566-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3566-127">Request body</span></span>
<span data-ttu-id="f3566-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3566-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3566-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3566-129">Response</span></span>

<span data-ttu-id="f3566-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3566-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3566-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f3566-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3566-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3566-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413
```


### <a name="response"></a><span data-ttu-id="f3566-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3566-133">Response</span></span>
<span data-ttu-id="f3566-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f3566-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdUsing": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdDateTime": "2020-09-09T21:35:27.91Z",
    "modifiedDateTime": "2020-09-09T21:35:27.91Z",
    "status": "Provisioned",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "assignmentType": "Eligible",
    "memberType": "direct"
  }
}
```

