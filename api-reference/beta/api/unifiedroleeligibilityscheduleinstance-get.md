---
title: Get unifiedRoleEligibilityScheduleInstance
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleEligibilityScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adf95e156e4750add6f0763be17b122a3ebaf489
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299520"
---
# <a name="get-unifiedroleeligibilityscheduleinstance"></a><span data-ttu-id="4d2e1-103">Get unifiedRoleEligibilityScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="4d2e1-103">Get unifiedRoleEligibilityScheduleInstance</span></span>
<span data-ttu-id="4d2e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d2e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d2e1-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilityScheduleInstance.](../resources/unifiedroleeligibilityscheduleinstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d2e1-105">Read the properties and relationships of an [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d2e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2e1-106">Permissions</span></span>
<span data-ttu-id="4d2e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d2e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d2e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2e1-109">Permission type</span></span>|<span data-ttu-id="4d2e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d2e1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d2e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d2e1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d2e1-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4d2e1-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="4d2e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d2e1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d2e1-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4d2e1-114">Not supported</span></span>|
|<span data-ttu-id="4d2e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d2e1-115">Application</span></span>|<span data-ttu-id="4d2e1-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4d2e1-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d2e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d2e1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances/{unifiedRoleEligibilityScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d2e1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d2e1-118">Optional query parameters</span></span>
<span data-ttu-id="4d2e1-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="4d2e1-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4d2e1-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4d2e1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d2e1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d2e1-121">Request headers</span></span>
|<span data-ttu-id="4d2e1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4d2e1-122">Name</span></span>|<span data-ttu-id="4d2e1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2e1-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4d2e1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d2e1-124">Authorization</span></span>|<span data-ttu-id="4d2e1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d2e1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d2e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d2e1-127">Request body</span></span>
<span data-ttu-id="4d2e1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d2e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d2e1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2e1-129">Response</span></span>

<span data-ttu-id="4d2e1-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4d2e1-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d2e1-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4d2e1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d2e1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d2e1-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances/5cfd7709-7709-5cfd-0977-fd5c0977fd5c
```


### <a name="response"></a><span data-ttu-id="4d2e1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2e1-133">Response</span></span>
<span data-ttu-id="4d2e1-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4d2e1-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
    "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "startDateTime": "2020-09-09T21:35:27.91Z",
    "endDateTime": "2020-09-09T21:35:27.91Z",
    "memberType": "direct",
    "roleEligibilityScheduleId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c"
  }
}
```

