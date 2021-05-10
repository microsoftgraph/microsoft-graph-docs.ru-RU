---
title: Get unifiedRoleEligibilityScheduleRequest
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ea5ed510740770b6103275d89d03c01c65e77f6
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299737"
---
# <a name="get-unifiedroleeligibilityschedulerequest"></a><span data-ttu-id="33b08-103">Get unifiedRoleEligibilityScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="33b08-103">Get unifiedRoleEligibilityScheduleRequest</span></span>
<span data-ttu-id="33b08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33b08-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="33b08-105">Read the properties and relationships of an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="33b08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33b08-106">Permissions</span></span>
<span data-ttu-id="33b08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33b08-109">Permission type</span></span>|<span data-ttu-id="33b08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33b08-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33b08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33b08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="33b08-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="33b08-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="33b08-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33b08-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33b08-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="33b08-114">Not supported</span></span>|
|<span data-ttu-id="33b08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33b08-115">Application</span></span>|<span data-ttu-id="33b08-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="33b08-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="33b08-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33b08-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33b08-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="33b08-118">Optional query parameters</span></span>
<span data-ttu-id="33b08-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="33b08-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="33b08-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="33b08-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="33b08-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33b08-121">Request headers</span></span>
|<span data-ttu-id="33b08-122">Имя</span><span class="sxs-lookup"><span data-stu-id="33b08-122">Name</span></span>|<span data-ttu-id="33b08-123">Описание</span><span class="sxs-lookup"><span data-stu-id="33b08-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="33b08-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33b08-124">Authorization</span></span>|<span data-ttu-id="33b08-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33b08-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33b08-127">Request body</span></span>
<span data-ttu-id="33b08-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33b08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33b08-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b08-129">Response</span></span>

<span data-ttu-id="33b08-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="33b08-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33b08-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="33b08-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33b08-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="33b08-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```


### <a name="response"></a><span data-ttu-id="33b08-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b08-133">Response</span></span>
<span data-ttu-id="33b08-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="33b08-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
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

