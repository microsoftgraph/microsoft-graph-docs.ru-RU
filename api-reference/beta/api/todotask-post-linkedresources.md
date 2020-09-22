---
title: Создание Линкедресаурцес
description: Создание нового объекта Линкедресаурцес.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5a5a702c55db40c77304c577b440f34dc610e8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058587"
---
# <a name="create-linkedresources"></a><span data-ttu-id="2a5b1-103">Создание Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="2a5b1-103">Create linkedResources</span></span>
<span data-ttu-id="2a5b1-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="2a5b1-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="2a5b1-105">Создание нового объекта Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-105">Create a new linkedResources object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a5b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a5b1-106">Permissions</span></span>
<span data-ttu-id="2a5b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a5b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a5b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a5b1-109">Permission type</span></span>|<span data-ttu-id="2a5b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a5b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a5b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a5b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a5b1-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a5b1-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2a5b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a5b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a5b1-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a5b1-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2a5b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a5b1-115">Application</span></span>|<span data-ttu-id="2a5b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a5b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a5b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="2a5b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a5b1-118">Request headers</span></span>
|<span data-ttu-id="2a5b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2a5b1-119">Name</span></span>|<span data-ttu-id="2a5b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2a5b1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a5b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a5b1-121">Authorization</span></span>|<span data-ttu-id="2a5b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a5b1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a5b1-124">Content-Type</span></span>|<span data-ttu-id="2a5b1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a5b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a5b1-127">Request body</span></span>
<span data-ttu-id="2a5b1-128">В тексте запроса добавьте представление объекта [линкедресаурце](../resources/linkedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="2a5b1-129">В следующей таблице приведены свойства, необходимые при создании [линкедресаурце](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="2a5b1-129">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="2a5b1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a5b1-130">Property</span></span>|<span data-ttu-id="2a5b1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2a5b1-131">Type</span></span>|<span data-ttu-id="2a5b1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2a5b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a5b1-133">id</span><span class="sxs-lookup"><span data-stu-id="2a5b1-133">id</span></span>|<span data-ttu-id="2a5b1-134">String</span><span class="sxs-lookup"><span data-stu-id="2a5b1-134">String</span></span>|<span data-ttu-id="2a5b1-135">Созданный сервером идентификатор связанной сущности, унаследованной от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="2a5b1-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="2a5b1-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="2a5b1-136">webUrl</span></span>|<span data-ttu-id="2a5b1-137">String</span><span class="sxs-lookup"><span data-stu-id="2a5b1-137">String</span></span>|<span data-ttu-id="2a5b1-138">Прямой ссылки на связанный объект</span><span class="sxs-lookup"><span data-stu-id="2a5b1-138">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="2a5b1-139">applicationName</span><span class="sxs-lookup"><span data-stu-id="2a5b1-139">applicationName</span></span>|<span data-ttu-id="2a5b1-140">String</span><span class="sxs-lookup"><span data-stu-id="2a5b1-140">String</span></span>|<span data-ttu-id="2a5b1-141">Поле, указывающее имя приложения источника, отправляющего связанный объект</span><span class="sxs-lookup"><span data-stu-id="2a5b1-141">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="2a5b1-142">displayName</span><span class="sxs-lookup"><span data-stu-id="2a5b1-142">displayName</span></span>|<span data-ttu-id="2a5b1-143">String</span><span class="sxs-lookup"><span data-stu-id="2a5b1-143">String</span></span>|<span data-ttu-id="2a5b1-144">Поле, указывающее название связанного объекта.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-144">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="2a5b1-145">externalId</span><span class="sxs-lookup"><span data-stu-id="2a5b1-145">externalId</span></span>|<span data-ttu-id="2a5b1-146">String</span><span class="sxs-lookup"><span data-stu-id="2a5b1-146">String</span></span>|<span data-ttu-id="2a5b1-147">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="2a5b1-147">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="2a5b1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a5b1-148">Response</span></span>

<span data-ttu-id="2a5b1-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-149">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a5b1-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a5b1-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a5b1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a5b1-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2a5b1-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a5b1-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="2a5b1-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a5b1-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2a5b1-154">C#</span><span class="sxs-lookup"><span data-stu-id="2a5b1-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a5b1-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a5b1-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2a5b1-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a5b1-156">Response</span></span>
<span data-ttu-id="2a5b1-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a5b1-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```



