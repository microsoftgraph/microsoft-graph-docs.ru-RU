---
title: Get unifiedRoleEligibilitySchedule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleEligibilitySchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 22f90942b141cca787ea583debb718b8a05c41d8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679948"
---
# <a name="get-unifiedroleeligibilityschedule"></a><span data-ttu-id="d11f0-103">Get unifiedRoleEligibilitySchedule</span><span class="sxs-lookup"><span data-stu-id="d11f0-103">Get unifiedRoleEligibilitySchedule</span></span>
<span data-ttu-id="d11f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d11f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d11f0-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilitySchedule.](../resources/unifiedroleeligibilityschedule.md)</span><span class="sxs-lookup"><span data-stu-id="d11f0-105">Read the properties and relationships of an [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d11f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d11f0-106">Permissions</span></span>
<span data-ttu-id="d11f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d11f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d11f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d11f0-109">Permission type</span></span>|<span data-ttu-id="d11f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d11f0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d11f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d11f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d11f0-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="d11f0-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="d11f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d11f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d11f0-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d11f0-114">Not supported</span></span>|
|<span data-ttu-id="d11f0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d11f0-115">Application</span></span>|<span data-ttu-id="d11f0-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="d11f0-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="d11f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d11f0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules/{unifiedRoleEligibilitySchedulesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d11f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d11f0-118">Optional query parameters</span></span>
<span data-ttu-id="d11f0-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="d11f0-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d11f0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d11f0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d11f0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d11f0-121">Request headers</span></span>
|<span data-ttu-id="d11f0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d11f0-122">Name</span></span>|<span data-ttu-id="d11f0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d11f0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d11f0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d11f0-124">Authorization</span></span>|<span data-ttu-id="d11f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d11f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d11f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d11f0-127">Request body</span></span>
<span data-ttu-id="d11f0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d11f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d11f0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11f0-129">Response</span></span>

<span data-ttu-id="d11f0-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d11f0-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d11f0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d11f0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d11f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d11f0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d11f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d11f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules/5cfd7709-7709-5cfd-0977-fd5c0977fd5c
```
# <a name="c"></a>[<span data-ttu-id="d11f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="d11f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleeligibilityschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d11f0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d11f0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleeligibilityschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d11f0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d11f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleeligibilityschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d11f0-137">Java</span><span class="sxs-lookup"><span data-stu-id="d11f0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleeligibilityschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d11f0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11f0-138">Response</span></span>
<span data-ttu-id="d11f0-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d11f0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "createdUsing": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "createdDateTime": "2020-09-09T21:35:27.91Z",
    "modifiedDateTime": "2020-09-09T21:35:27.91Z",
    "status": "Provisioned",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "memberType": "direct"
  }
}
```

