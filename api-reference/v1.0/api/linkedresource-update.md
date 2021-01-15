---
title: Обновление linkedResource
description: Обновление свойств объекта linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b41e4d3948ccca6f58c1ab701367f4432b489551
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873810"
---
# <a name="update-linkedresource"></a><span data-ttu-id="bb604-103">Обновление linkedResource</span><span class="sxs-lookup"><span data-stu-id="bb604-103">Update linkedResource</span></span>
<span data-ttu-id="bb604-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb604-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb604-105">Обновление свойств объекта [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="bb604-105">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb604-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb604-106">Permissions</span></span>
<span data-ttu-id="bb604-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb604-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb604-109">Permission type</span></span>|<span data-ttu-id="bb604-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb604-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb604-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb604-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb604-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb604-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="bb604-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb604-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb604-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb604-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="bb604-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb604-115">Application</span></span>|<span data-ttu-id="bb604-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="bb604-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb604-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb604-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="bb604-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb604-118">Request headers</span></span>
|<span data-ttu-id="bb604-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bb604-119">Name</span></span>|<span data-ttu-id="bb604-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bb604-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bb604-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb604-121">Authorization</span></span>|<span data-ttu-id="bb604-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb604-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bb604-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb604-124">Content-Type</span></span>|<span data-ttu-id="bb604-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb604-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb604-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb604-127">Request body</span></span>
<span data-ttu-id="bb604-128">В теле запроса укажу представление объекта [linkedResource](../resources/linkedresource.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="bb604-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="bb604-129">В следующей таблице показаны свойства, необходимые при обновлении [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="bb604-129">The following table shows the properties that are required when you update the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="bb604-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb604-130">Property</span></span>|<span data-ttu-id="bb604-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bb604-131">Type</span></span>|<span data-ttu-id="bb604-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb604-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb604-133">id</span><span class="sxs-lookup"><span data-stu-id="bb604-133">id</span></span>|<span data-ttu-id="bb604-134">String</span><span class="sxs-lookup"><span data-stu-id="bb604-134">String</span></span>|<span data-ttu-id="bb604-135">Созданный сервером ИД для связанного объекта Inherited from [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="bb604-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="response"></a><span data-ttu-id="bb604-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb604-136">Response</span></span>

<span data-ttu-id="bb604-137">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [linkedResource](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb604-137">If successful, this method returns a `200 OK` response code and an updated [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb604-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="bb604-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb604-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb604-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bb604-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb604-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "update_linkedresource"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft"
}
```
# <a name="c"></a>[<span data-ttu-id="bb604-141">C#</span><span class="sxs-lookup"><span data-stu-id="bb604-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb604-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb604-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb604-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb604-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb604-144">Java</span><span class="sxs-lookup"><span data-stu-id="bb604-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bb604-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb604-145">Response</span></span>
<span data-ttu-id="bb604-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb604-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```


