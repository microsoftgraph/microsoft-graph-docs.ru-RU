---
title: Получить linkedResource
description: Чтение свойств и связей объекта linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e13fc32575c2b5aeccd55491f0f66ee6be923812
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872487"
---
# <a name="get-linkedresource"></a><span data-ttu-id="f65bf-103">Получить linkedResource</span><span class="sxs-lookup"><span data-stu-id="f65bf-103">Get linkedResource</span></span>
<span data-ttu-id="f65bf-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="f65bf-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="f65bf-105">Чтение свойств и связей объекта [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="f65bf-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f65bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f65bf-106">Permissions</span></span>
<span data-ttu-id="f65bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f65bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f65bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f65bf-109">Permission type</span></span>|<span data-ttu-id="f65bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f65bf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f65bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f65bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f65bf-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f65bf-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f65bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f65bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f65bf-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f65bf-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f65bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f65bf-115">Application</span></span>|<span data-ttu-id="f65bf-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f65bf-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f65bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f65bf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="f65bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f65bf-118">Request headers</span></span>
|<span data-ttu-id="f65bf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f65bf-119">Name</span></span>|<span data-ttu-id="f65bf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f65bf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f65bf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f65bf-121">Authorization</span></span>|<span data-ttu-id="f65bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f65bf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f65bf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f65bf-124">Request body</span></span>
<span data-ttu-id="f65bf-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f65bf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f65bf-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f65bf-126">Response</span></span>

<span data-ttu-id="f65bf-127">В случае успеха этот метод возвращает код отклика и объект `200 OK` [linkedResource](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f65bf-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f65bf-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f65bf-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f65bf-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f65bf-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f65bf-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f65bf-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="f65bf-131">C#</span><span class="sxs-lookup"><span data-stu-id="f65bf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f65bf-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f65bf-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f65bf-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f65bf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f65bf-134">Java</span><span class="sxs-lookup"><span data-stu-id="f65bf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f65bf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f65bf-135">Response</span></span>
<span data-ttu-id="f65bf-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f65bf-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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


