---
title: Создание linkedResource
description: Создание объекта linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8c99568099c99622373b91fff4a4b247e80f9288
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874405"
---
# <a name="create-linkedresource"></a><span data-ttu-id="53b84-103">Создание linkedResource</span><span class="sxs-lookup"><span data-stu-id="53b84-103">Create linkedResource</span></span>
<span data-ttu-id="53b84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53b84-105">Создайте [объект linkedResource,](../resources/linkedresource.md) чтобы [](../resources/todotask.md) связать указанную задачу с элементом в партнерской службе.</span><span class="sxs-lookup"><span data-stu-id="53b84-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="53b84-106">Например, можно связать задачу с элементом электронной почты в Outlook, который создал задачу, и создать объект **linkedResource** для отслеживания ее связи.</span><span class="sxs-lookup"><span data-stu-id="53b84-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="53b84-107">Вы также можете создать объект **linkedResource** при [создании задачи.](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples)</span><span class="sxs-lookup"><span data-stu-id="53b84-107">You can also create a **linkedResource** object while [creating a task](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="53b84-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53b84-108">Permissions</span></span>
<span data-ttu-id="53b84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53b84-111">Permission type</span></span>|<span data-ttu-id="53b84-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53b84-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53b84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53b84-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53b84-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="53b84-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53b84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b84-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53b84-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="53b84-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53b84-117">Application</span></span>|<span data-ttu-id="53b84-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b84-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="53b84-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53b84-120">Request headers</span></span>
|<span data-ttu-id="53b84-121">Имя</span><span class="sxs-lookup"><span data-stu-id="53b84-121">Name</span></span>|<span data-ttu-id="53b84-122">Описание</span><span class="sxs-lookup"><span data-stu-id="53b84-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53b84-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53b84-123">Authorization</span></span>|<span data-ttu-id="53b84-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b84-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="53b84-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53b84-126">Content-Type</span></span>|<span data-ttu-id="53b84-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b84-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b84-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53b84-129">Request body</span></span>
<span data-ttu-id="53b84-130">В теле запроса укажу представление объекта [linkedResource](../resources/linkedresource.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="53b84-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="53b84-131">В следующей таблице показаны свойства, необходимые при создании [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="53b84-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="53b84-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="53b84-132">Property</span></span>|<span data-ttu-id="53b84-133">Тип</span><span class="sxs-lookup"><span data-stu-id="53b84-133">Type</span></span>|<span data-ttu-id="53b84-134">Описание</span><span class="sxs-lookup"><span data-stu-id="53b84-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b84-135">id</span><span class="sxs-lookup"><span data-stu-id="53b84-135">id</span></span>|<span data-ttu-id="53b84-136">String</span><span class="sxs-lookup"><span data-stu-id="53b84-136">String</span></span>|<span data-ttu-id="53b84-137">Созданный сервером ИД для связанного объекта Inherited from [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="53b84-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="53b84-138">webUrl</span><span class="sxs-lookup"><span data-stu-id="53b84-138">webUrl</span></span>|<span data-ttu-id="53b84-139">String</span><span class="sxs-lookup"><span data-stu-id="53b84-139">String</span></span>|<span data-ttu-id="53b84-140">Глубокая связь со связанным объектом</span><span class="sxs-lookup"><span data-stu-id="53b84-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="53b84-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="53b84-141">applicationName</span></span>|<span data-ttu-id="53b84-142">String</span><span class="sxs-lookup"><span data-stu-id="53b84-142">String</span></span>|<span data-ttu-id="53b84-143">Поле, указывающее имя приложения источника, который отправляет связанную сущность</span><span class="sxs-lookup"><span data-stu-id="53b84-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="53b84-144">displayName</span><span class="sxs-lookup"><span data-stu-id="53b84-144">displayName</span></span>|<span data-ttu-id="53b84-145">String</span><span class="sxs-lookup"><span data-stu-id="53b84-145">String</span></span>|<span data-ttu-id="53b84-146">Поле, указывающее заголовок связанной сущности.</span><span class="sxs-lookup"><span data-stu-id="53b84-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="53b84-147">externalId</span><span class="sxs-lookup"><span data-stu-id="53b84-147">externalId</span></span>|<span data-ttu-id="53b84-148">String</span><span class="sxs-lookup"><span data-stu-id="53b84-148">String</span></span>|<span data-ttu-id="53b84-149">ИД объекта, связанного с этой задачей в стороншей или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="53b84-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="53b84-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b84-150">Response</span></span>

<span data-ttu-id="53b84-151">В случае успеха этот метод возвращает код отклика и объект `201 Created` [linkedResource](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53b84-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53b84-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="53b84-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53b84-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="53b84-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="53b84-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b84-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="c"></a>[<span data-ttu-id="53b84-155">C#</span><span class="sxs-lookup"><span data-stu-id="53b84-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53b84-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b84-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53b84-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b84-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53b84-158">Java</span><span class="sxs-lookup"><span data-stu-id="53b84-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-linkedresource-from-linkedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="53b84-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b84-159">Response</span></span>
<span data-ttu-id="53b84-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="53b84-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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



