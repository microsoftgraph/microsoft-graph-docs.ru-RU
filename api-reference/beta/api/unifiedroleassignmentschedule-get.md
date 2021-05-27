---
title: Get unifiedRoleAssignmentSchedule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentSchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d4e608946dea3314359b90c3c8b6b859c0a62566
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680399"
---
# <a name="get-unifiedroleassignmentschedule"></a><span data-ttu-id="6e5b4-103">Get unifiedRoleAssignmentSchedule</span><span class="sxs-lookup"><span data-stu-id="6e5b4-103">Get unifiedRoleAssignmentSchedule</span></span>
<span data-ttu-id="6e5b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e5b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e5b4-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)</span><span class="sxs-lookup"><span data-stu-id="6e5b4-105">Read the properties and relationships of an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e5b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e5b4-106">Permissions</span></span>
<span data-ttu-id="6e5b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e5b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e5b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e5b4-109">Permission type</span></span>|<span data-ttu-id="6e5b4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e5b4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e5b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e5b4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e5b4-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6e5b4-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="6e5b4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e5b4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e5b4-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e5b4-114">Not supported</span></span>|
|<span data-ttu-id="6e5b4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e5b4-115">Application</span></span>|<span data-ttu-id="6e5b4-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6e5b4-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e5b4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e5b4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentSchedulesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e5b4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6e5b4-118">Optional query parameters</span></span>
<span data-ttu-id="6e5b4-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="6e5b4-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6e5b4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6e5b4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e5b4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e5b4-121">Request headers</span></span>
|<span data-ttu-id="6e5b4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6e5b4-122">Name</span></span>|<span data-ttu-id="6e5b4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6e5b4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6e5b4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e5b4-124">Authorization</span></span>|<span data-ttu-id="6e5b4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e5b4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e5b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e5b4-127">Request body</span></span>
<span data-ttu-id="6e5b4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e5b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e5b4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e5b4-129">Response</span></span>

<span data-ttu-id="6e5b4-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6e5b4-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e5b4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e5b4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e5b4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e5b4-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413
```


### <a name="response"></a><span data-ttu-id="6e5b4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e5b4-133">Response</span></span>
<span data-ttu-id="6e5b4-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6e5b4-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

