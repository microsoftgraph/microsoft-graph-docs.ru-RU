---
title: Get unifiedRoleAssignmentScheduleInstance
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9659c6630aa310b240bd102d7ff76765d8fab3d
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351148"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a><span data-ttu-id="81d3f-103">Get unifiedRoleAssignmentScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="81d3f-103">Get unifiedRoleAssignmentScheduleInstance</span></span>
<span data-ttu-id="81d3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81d3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81d3f-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)</span><span class="sxs-lookup"><span data-stu-id="81d3f-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81d3f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81d3f-106">Permissions</span></span>
<span data-ttu-id="81d3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81d3f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81d3f-109">Permission type</span></span>|<span data-ttu-id="81d3f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81d3f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81d3f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81d3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81d3f-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81d3f-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="81d3f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81d3f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81d3f-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="81d3f-114">Not supported</span></span>|
|<span data-ttu-id="81d3f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81d3f-115">Application</span></span>|<span data-ttu-id="81d3f-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81d3f-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="81d3f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81d3f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81d3f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81d3f-118">Optional query parameters</span></span>
<span data-ttu-id="81d3f-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="81d3f-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="81d3f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="81d3f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="81d3f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81d3f-121">Request headers</span></span>
|<span data-ttu-id="81d3f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="81d3f-122">Name</span></span>|<span data-ttu-id="81d3f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="81d3f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81d3f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81d3f-124">Authorization</span></span>|<span data-ttu-id="81d3f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81d3f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81d3f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81d3f-127">Request body</span></span>
<span data-ttu-id="81d3f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81d3f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81d3f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="81d3f-129">Response</span></span>

<span data-ttu-id="81d3f-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="81d3f-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81d3f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="81d3f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81d3f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="81d3f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb
```


### <a name="response"></a><span data-ttu-id="81d3f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="81d3f-133">Response</span></span>
<span data-ttu-id="81d3f-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="81d3f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "principalId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleDefinitionId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "directoryScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "appScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "startDateTime": "2020-09-09T21:35:27.91Z",
    "endDateTime": "2020-09-09T21:35:27.91Z",
    "assignmentType": "eligible",
    "memberType": "direct",
    "roleAssignmentOriginId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleAssignmentScheduleId": "eb18c026-c026-eb18-26c0-18eb26c018eb"
  }
}
```

