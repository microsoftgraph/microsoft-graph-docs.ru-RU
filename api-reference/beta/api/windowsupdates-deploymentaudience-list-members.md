---
title: Участники аудитории развертывания списка
description: Список ресурсов updatableAsset, которые являются участниками развертыванияAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 9b7c448596c4da96fbc9109bf92436154d4191ca
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351134"
---
# <a name="list-deployment-audience-members"></a><span data-ttu-id="553f3-103">Участники аудитории развертывания списка</span><span class="sxs-lookup"><span data-stu-id="553f3-103">List deployment audience members</span></span>

<span data-ttu-id="553f3-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="553f3-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="553f3-105">Список [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов, которые являются членами [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="553f3-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are members of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

> [!NOTE]
> <span data-ttu-id="553f3-106">Этот API имеет [известные проблемы, связанные](/Graph/known-issues#accessing-and-updating-deployment-audiences) с развертываниями, созданными через Intune.</span><span class="sxs-lookup"><span data-stu-id="553f3-106">This API has a [known issue](/Graph/known-issues#accessing-and-updating-deployment-audiences) related to deployments created via Intune.</span></span>

## <a name="permissions"></a><span data-ttu-id="553f3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="553f3-107">Permissions</span></span>
<span data-ttu-id="553f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="553f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553f3-110">Permission type</span></span>|<span data-ttu-id="553f3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="553f3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="553f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="553f3-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="553f3-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="553f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="553f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553f3-115">Not supported.</span></span>|
|<span data-ttu-id="553f3-116">Application</span><span class="sxs-lookup"><span data-stu-id="553f3-116">Application</span></span>|<span data-ttu-id="553f3-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="553f3-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="553f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553f3-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="553f3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="553f3-119">Optional query parameters</span></span>
<span data-ttu-id="553f3-120">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="553f3-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="553f3-121">Чтобы использовать параметр запроса для свойства, которое не унаследовано от [updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса для свойства.</span><span class="sxs-lookup"><span data-stu-id="553f3-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="553f3-122">Например, чтобы выбрать [azureADDevice,](../resources/windowsupdates-azureaddevice.md) `errors` используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="553f3-122">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="553f3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553f3-123">Request headers</span></span>
|<span data-ttu-id="553f3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="553f3-124">Name</span></span>|<span data-ttu-id="553f3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="553f3-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="553f3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="553f3-126">Authorization</span></span>|<span data-ttu-id="553f3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="553f3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="553f3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="553f3-129">Request body</span></span>
<span data-ttu-id="553f3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="553f3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="553f3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="553f3-131">Response</span></span>

<span data-ttu-id="553f3-132">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="553f3-132">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="553f3-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="553f3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="553f3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="553f3-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="553f3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="553f3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/members
```
# <a name="c"></a>[<span data-ttu-id="553f3-136">C#</span><span class="sxs-lookup"><span data-stu-id="553f3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="553f3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="553f3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="553f3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="553f3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="553f3-139">Java</span><span class="sxs-lookup"><span data-stu-id="553f3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="553f3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="553f3-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "fb95f07d-9e73-411d-99ab-7eca3a5122b1",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
        }
      ]
    },
  ]
}
```

