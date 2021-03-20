---
title: Получить linkedResource
description: Ознакомьтесь с свойствами и отношениями объекта linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b353e6ca577bd27608e79674b53d6b34864c4155
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949843"
---
# <a name="get-linkedresource"></a><span data-ttu-id="e737a-103">Получить linkedResource</span><span class="sxs-lookup"><span data-stu-id="e737a-103">Get linkedResource</span></span>
<span data-ttu-id="e737a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e737a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e737a-105">Ознакомьтесь с свойствами и отношениями объекта [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="e737a-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e737a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e737a-106">Permissions</span></span>
<span data-ttu-id="e737a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e737a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e737a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e737a-109">Permission type</span></span>|<span data-ttu-id="e737a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e737a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e737a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e737a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e737a-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e737a-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e737a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e737a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e737a-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e737a-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e737a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e737a-115">Application</span></span>|<span data-ttu-id="e737a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e737a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e737a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e737a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="e737a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e737a-118">Request headers</span></span>
|<span data-ttu-id="e737a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e737a-119">Name</span></span>|<span data-ttu-id="e737a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e737a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e737a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e737a-121">Authorization</span></span>|<span data-ttu-id="e737a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e737a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e737a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e737a-124">Request body</span></span>
<span data-ttu-id="e737a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e737a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e737a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e737a-126">Response</span></span>

<span data-ttu-id="e737a-127">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект linkedResource](../resources/linkedresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e737a-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e737a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e737a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e737a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e737a-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e737a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e737a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="e737a-131">C#</span><span class="sxs-lookup"><span data-stu-id="e737a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e737a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e737a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e737a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e737a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e737a-134">Java</span><span class="sxs-lookup"><span data-stu-id="e737a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e737a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e737a-135">Response</span></span>
<span data-ttu-id="e737a-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e737a-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
     "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
  }
}
```


