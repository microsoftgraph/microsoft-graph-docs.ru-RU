---
title: Get unifiedRoleAssignmentScheduleInstance
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6eeba1d6971e51357a52ce78cf56c2e00caa3d77
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680320"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a><span data-ttu-id="f0b6c-103">Get unifiedRoleAssignmentScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="f0b6c-103">Get unifiedRoleAssignmentScheduleInstance</span></span>
<span data-ttu-id="f0b6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0b6c-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)</span><span class="sxs-lookup"><span data-stu-id="f0b6c-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0b6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b6c-106">Permissions</span></span>
<span data-ttu-id="f0b6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0b6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0b6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b6c-109">Permission type</span></span>|<span data-ttu-id="f0b6c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0b6c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0b6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0b6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0b6c-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f0b6c-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="f0b6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0b6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0b6c-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f0b6c-114">Not supported</span></span>|
|<span data-ttu-id="f0b6c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0b6c-115">Application</span></span>|<span data-ttu-id="f0b6c-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f0b6c-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0b6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0b6c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0b6c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0b6c-118">Optional query parameters</span></span>
<span data-ttu-id="f0b6c-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="f0b6c-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f0b6c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f0b6c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0b6c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0b6c-121">Request headers</span></span>
|<span data-ttu-id="f0b6c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f0b6c-122">Name</span></span>|<span data-ttu-id="f0b6c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f0b6c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f0b6c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0b6c-124">Authorization</span></span>|<span data-ttu-id="f0b6c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0b6c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0b6c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0b6c-127">Request body</span></span>
<span data-ttu-id="f0b6c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0b6c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0b6c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b6c-129">Response</span></span>

<span data-ttu-id="f0b6c-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f0b6c-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0b6c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f0b6c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0b6c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0b6c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/unifiedRoleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb
```


### <a name="response"></a><span data-ttu-id="f0b6c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b6c-133">Response</span></span>
<span data-ttu-id="f0b6c-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f0b6c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

