---
title: 'unifiedRoleAssignmentScheduleInstance: filterByCurrentUser'
description: Получите список объектов unifiedRoleAssignmentScheduleInstance и их свойств, отфильтрованных определенным пользователем
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cd84a9e617f582eb01afe31cad28114f22e03432
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680327"
---
# <a name="unifiedroleassignmentscheduleinstance-filterbycurrentuser"></a><span data-ttu-id="0056a-103">unifiedRoleAssignmentScheduleInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="0056a-103">unifiedRoleAssignmentScheduleInstance: filterByCurrentUser</span></span>
<span data-ttu-id="0056a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0056a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0056a-105">Получите список объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) и их свойств, связанных с определенным основным объектом.</span><span class="sxs-lookup"><span data-stu-id="0056a-105">Get a list of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0056a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0056a-106">Permissions</span></span>
<span data-ttu-id="0056a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0056a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0056a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0056a-109">Permission type</span></span>|<span data-ttu-id="0056a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0056a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0056a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0056a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0056a-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0056a-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="0056a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0056a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0056a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0056a-114">Not supported</span></span>|
|<span data-ttu-id="0056a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0056a-115">Application</span></span>|<span data-ttu-id="0056a-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0056a-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="0056a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0056a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="0056a-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="0056a-118">Query parameters</span></span>
<span data-ttu-id="0056a-119">В следующей таблице показаны параметры, которые можно использовать с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="0056a-119">The following table shows the parameters that can be used with this method.</span></span>

|<span data-ttu-id="0056a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="0056a-120">Parameter</span></span>|<span data-ttu-id="0056a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0056a-121">Type</span></span>|<span data-ttu-id="0056a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0056a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0056a-123">on</span><span class="sxs-lookup"><span data-stu-id="0056a-123">on</span></span>|<span data-ttu-id="0056a-124">roleAssignmentScheduleInstanceFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="0056a-124">roleAssignmentScheduleInstanceFilterByCurrentUserOptions</span></span>|<span data-ttu-id="0056a-125">Id текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="0056a-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="0056a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0056a-126">Request headers</span></span>
|<span data-ttu-id="0056a-127">Имя</span><span class="sxs-lookup"><span data-stu-id="0056a-127">Name</span></span>|<span data-ttu-id="0056a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0056a-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0056a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0056a-129">Authorization</span></span>|<span data-ttu-id="0056a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0056a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0056a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0056a-132">Request body</span></span>
<span data-ttu-id="0056a-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0056a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0056a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0056a-134">Response</span></span>

<span data-ttu-id="0056a-135">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [унифицированную коллекциюRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0056a-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0056a-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="0056a-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0056a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0056a-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentscheduleinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/unifiedRoleAssignmentScheduleInstances/filterByCurrentUser(on='dce468b2-68b2-dce4-b268-e4dcb268e4dc')
```


### <a name="response"></a><span data-ttu-id="0056a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0056a-138">Response</span></span>
<span data-ttu-id="0056a-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0056a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "assignmentType": "eligible",
      "memberType": "direct",
      "roleAssignmentOriginId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "roleAssignmentScheduleId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc"
    }
  ]
}
```

