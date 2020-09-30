---
title: Создание Линкедресаурце
description: Создание нового объекта Линкедресаурце.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 56ad2b1f83475cc6b5af748c129f0cd84cdc07b0
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313697"
---
# <a name="create-linkedresource"></a><span data-ttu-id="91488-103">Создание Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="91488-103">Create linkedResource</span></span>
<span data-ttu-id="91488-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="91488-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="91488-105">Создание нового объекта **линкедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="91488-105">Create a new **linkedResource** object.</span></span>

<span data-ttu-id="91488-106">Вы также можете создать объект **линкедресаурце** при [создании тодотаск](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span><span class="sxs-lookup"><span data-stu-id="91488-106">You can also create a **linkedResource** object while [creating a todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="91488-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91488-107">Permissions</span></span>
<span data-ttu-id="91488-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91488-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91488-110">Permission type</span></span>|<span data-ttu-id="91488-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91488-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91488-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91488-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91488-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91488-113">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="91488-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91488-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91488-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91488-115">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="91488-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91488-116">Application</span></span>|<span data-ttu-id="91488-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91488-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91488-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91488-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="91488-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91488-119">Request headers</span></span>
|<span data-ttu-id="91488-120">Имя</span><span class="sxs-lookup"><span data-stu-id="91488-120">Name</span></span>|<span data-ttu-id="91488-121">Описание</span><span class="sxs-lookup"><span data-stu-id="91488-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="91488-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91488-122">Authorization</span></span>|<span data-ttu-id="91488-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91488-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="91488-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91488-125">Content-Type</span></span>|<span data-ttu-id="91488-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91488-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91488-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91488-128">Request body</span></span>
<span data-ttu-id="91488-129">В тексте запроса добавьте представление объекта [линкедресаурце](../resources/linkedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91488-129">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="91488-130">В следующей таблице приведены свойства, необходимые при создании [линкедресаурце](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="91488-130">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="91488-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="91488-131">Property</span></span>|<span data-ttu-id="91488-132">Тип</span><span class="sxs-lookup"><span data-stu-id="91488-132">Type</span></span>|<span data-ttu-id="91488-133">Описание</span><span class="sxs-lookup"><span data-stu-id="91488-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91488-134">id</span><span class="sxs-lookup"><span data-stu-id="91488-134">id</span></span>|<span data-ttu-id="91488-135">String</span><span class="sxs-lookup"><span data-stu-id="91488-135">String</span></span>|<span data-ttu-id="91488-136">Созданный сервером идентификатор связанной сущности, унаследованной от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="91488-136">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="91488-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="91488-137">webUrl</span></span>|<span data-ttu-id="91488-138">String</span><span class="sxs-lookup"><span data-stu-id="91488-138">String</span></span>|<span data-ttu-id="91488-139">Прямой ссылки на связанный объект</span><span class="sxs-lookup"><span data-stu-id="91488-139">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="91488-140">applicationName</span><span class="sxs-lookup"><span data-stu-id="91488-140">applicationName</span></span>|<span data-ttu-id="91488-141">String</span><span class="sxs-lookup"><span data-stu-id="91488-141">String</span></span>|<span data-ttu-id="91488-142">Поле, указывающее имя приложения источника, отправляющего связанный объект</span><span class="sxs-lookup"><span data-stu-id="91488-142">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="91488-143">displayName</span><span class="sxs-lookup"><span data-stu-id="91488-143">displayName</span></span>|<span data-ttu-id="91488-144">String</span><span class="sxs-lookup"><span data-stu-id="91488-144">String</span></span>|<span data-ttu-id="91488-145">Поле, указывающее название связанного объекта.</span><span class="sxs-lookup"><span data-stu-id="91488-145">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="91488-146">externalId</span><span class="sxs-lookup"><span data-stu-id="91488-146">externalId</span></span>|<span data-ttu-id="91488-147">String</span><span class="sxs-lookup"><span data-stu-id="91488-147">String</span></span>|<span data-ttu-id="91488-148">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="91488-148">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="91488-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="91488-149">Response</span></span>

<span data-ttu-id="91488-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91488-150">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91488-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="91488-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91488-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="91488-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="91488-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="91488-153">HTTP</span></span>](#tab/http)
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
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="91488-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91488-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="91488-155">C#</span><span class="sxs-lookup"><span data-stu-id="91488-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91488-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91488-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="91488-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="91488-157">Response</span></span>
<span data-ttu-id="91488-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91488-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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



