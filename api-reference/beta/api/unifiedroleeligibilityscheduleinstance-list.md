---
title: Список unifiedRoleEligibilityScheduleInstances
description: Получите список объектов unifiedRoleEligibilityScheduleInstance и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ca95171cb9b174e4686f4228274679ec09b72e5
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299514"
---
# <a name="list-unifiedroleeligibilityscheduleinstances"></a><span data-ttu-id="da1d7-103">Список unifiedRoleEligibilityScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="da1d7-103">List unifiedRoleEligibilityScheduleInstances</span></span>
<span data-ttu-id="da1d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da1d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da1d7-105">Получите список объектов [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="da1d7-105">Get a list of the [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="da1d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da1d7-106">Permissions</span></span>
<span data-ttu-id="da1d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da1d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da1d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da1d7-109">Permission type</span></span>|<span data-ttu-id="da1d7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da1d7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da1d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da1d7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da1d7-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="da1d7-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="da1d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da1d7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da1d7-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="da1d7-114">Not supported</span></span>|
|<span data-ttu-id="da1d7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da1d7-115">Application</span></span>|<span data-ttu-id="da1d7-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="da1d7-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="da1d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da1d7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da1d7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da1d7-118">Optional query parameters</span></span>
<span data-ttu-id="da1d7-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="da1d7-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="da1d7-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="da1d7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="da1d7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da1d7-121">Request headers</span></span>
|<span data-ttu-id="da1d7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="da1d7-122">Name</span></span>|<span data-ttu-id="da1d7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="da1d7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da1d7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da1d7-124">Authorization</span></span>|<span data-ttu-id="da1d7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da1d7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da1d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da1d7-127">Request body</span></span>
<span data-ttu-id="da1d7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da1d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da1d7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="da1d7-129">Response</span></span>

<span data-ttu-id="da1d7-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="da1d7-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da1d7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="da1d7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da1d7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="da1d7-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances
```


### <a name="response"></a><span data-ttu-id="da1d7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="da1d7-133">Response</span></span>
<span data-ttu-id="da1d7-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da1d7-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "principalId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "roleDefinitionId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "directoryScopeId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "appScopeId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "memberType": "direct",
      "roleEligibilityScheduleId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1"
    }
  ]
}
```

