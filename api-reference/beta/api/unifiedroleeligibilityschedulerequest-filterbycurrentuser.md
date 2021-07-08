---
title: 'unifiedRoleEligibilityScheduleRequest: filterByCurrentUser'
description: Получите список объектов unifiedRoleEligibilityScheduleRequest и их свойств, отфильтрованных определенным пользователем
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8ad251e390eae9f328b425c1083f189d5c6989a5
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334677"
---
# <a name="unifiedroleeligibilityschedulerequest-filterbycurrentuser"></a><span data-ttu-id="6f6ba-103">unifiedRoleEligibilityScheduleRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="6f6ba-103">unifiedRoleEligibilityScheduleRequest: filterByCurrentUser</span></span>
<span data-ttu-id="6f6ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f6ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f6ba-105">Получите список объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) и их свойств, связанных с определенным основным объектом.</span><span class="sxs-lookup"><span data-stu-id="6f6ba-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f6ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6ba-106">Permissions</span></span>
<span data-ttu-id="6f6ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6ba-109">Permission type</span></span>|<span data-ttu-id="6f6ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f6ba-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f6ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f6ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f6ba-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6f6ba-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="6f6ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f6ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f6ba-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6f6ba-114">Not supported</span></span>|
|<span data-ttu-id="6f6ba-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f6ba-115">Application</span></span>|<span data-ttu-id="6f6ba-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6f6ba-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f6ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f6ba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="6f6ba-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6f6ba-118">Function parameters</span></span>
<span data-ttu-id="6f6ba-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="6f6ba-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6f6ba-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="6f6ba-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6f6ba-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="6f6ba-121">Parameter</span></span>|<span data-ttu-id="6f6ba-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6f6ba-122">Type</span></span>|<span data-ttu-id="6f6ba-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6f6ba-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f6ba-124">on</span><span class="sxs-lookup"><span data-stu-id="6f6ba-124">on</span></span>|<span data-ttu-id="6f6ba-125">RoleEligibilityScheduleRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="6f6ba-125">RoleEligibilityScheduleRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="6f6ba-126">ID основного объекта</span><span class="sxs-lookup"><span data-stu-id="6f6ba-126">ID of the principal object</span></span>|


## <a name="request-headers"></a><span data-ttu-id="6f6ba-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f6ba-127">Request headers</span></span>
|<span data-ttu-id="6f6ba-128">Имя</span><span class="sxs-lookup"><span data-stu-id="6f6ba-128">Name</span></span>|<span data-ttu-id="6f6ba-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6f6ba-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f6ba-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f6ba-130">Authorization</span></span>|<span data-ttu-id="6f6ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f6ba-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6ba-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f6ba-133">Request body</span></span>
<span data-ttu-id="6f6ba-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f6ba-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f6ba-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f6ba-135">Response</span></span>

<span data-ttu-id="6f6ba-136">В случае успешной работы эта функция возвращает код ответа и коллекцию `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6f6ba-136">If successful, this function returns a `200 OK` response code and a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f6ba-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="6f6ba-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f6ba-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f6ba-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedRoleEligibilityScheduleRequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser(on='parameterValue')
```


### <a name="response"></a><span data-ttu-id="6f6ba-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f6ba-139">Response</span></span>
<span data-ttu-id="6f6ba-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6f6ba-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "String (identifier)",
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
  ]
}
```

