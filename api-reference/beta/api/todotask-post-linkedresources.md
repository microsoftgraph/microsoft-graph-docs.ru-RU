---
title: Создание Линкедресаурце
description: Создание нового объекта Линкедресаурце.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e99f1d74a63baa2c83c2fc27e9e45a32ad52a46a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974349"
---
# <a name="create-linkedresource"></a><span data-ttu-id="b5618-103">Создание Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="b5618-103">Create linkedResource</span></span>
<span data-ttu-id="b5618-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="b5618-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="b5618-105">Создайте объект [линкедресаурце](../resources/linkedresource.md) для связи указанной [задачи](../resources/todotask.md) с элементом партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="b5618-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="b5618-106">Например, вы можете связать задачу с элементом электронной почты в Outlook, спурред задачу, а также создать объект **линкедресаурце** для отслеживания его связи.</span><span class="sxs-lookup"><span data-stu-id="b5618-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="b5618-107">Вы также можете создать объект **линкедресаурце** при [создании тодотаск](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span><span class="sxs-lookup"><span data-stu-id="b5618-107">You can also create a **linkedResource** object while [creating a todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5618-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5618-108">Permissions</span></span>
<span data-ttu-id="b5618-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5618-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5618-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5618-111">Permission type</span></span>|<span data-ttu-id="b5618-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5618-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5618-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5618-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5618-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5618-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b5618-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5618-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5618-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5618-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b5618-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5618-117">Application</span></span>|<span data-ttu-id="b5618-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5618-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5618-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5618-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="b5618-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5618-120">Request headers</span></span>
|<span data-ttu-id="b5618-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b5618-121">Name</span></span>|<span data-ttu-id="b5618-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b5618-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b5618-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5618-123">Authorization</span></span>|<span data-ttu-id="b5618-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5618-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b5618-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5618-126">Content-Type</span></span>|<span data-ttu-id="b5618-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5618-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5618-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5618-129">Request body</span></span>
<span data-ttu-id="b5618-130">В тексте запроса добавьте представление объекта [линкедресаурце](../resources/linkedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5618-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="b5618-131">В следующей таблице приведены свойства, необходимые при создании [линкедресаурце](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="b5618-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="b5618-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5618-132">Property</span></span>|<span data-ttu-id="b5618-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b5618-133">Type</span></span>|<span data-ttu-id="b5618-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b5618-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5618-135">id</span><span class="sxs-lookup"><span data-stu-id="b5618-135">id</span></span>|<span data-ttu-id="b5618-136">String</span><span class="sxs-lookup"><span data-stu-id="b5618-136">String</span></span>|<span data-ttu-id="b5618-137">Созданный сервером идентификатор связанной сущности, унаследованной от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="b5618-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="b5618-138">webUrl</span><span class="sxs-lookup"><span data-stu-id="b5618-138">webUrl</span></span>|<span data-ttu-id="b5618-139">String</span><span class="sxs-lookup"><span data-stu-id="b5618-139">String</span></span>|<span data-ttu-id="b5618-140">Прямой ссылки на связанный объект</span><span class="sxs-lookup"><span data-stu-id="b5618-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="b5618-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="b5618-141">applicationName</span></span>|<span data-ttu-id="b5618-142">String</span><span class="sxs-lookup"><span data-stu-id="b5618-142">String</span></span>|<span data-ttu-id="b5618-143">Поле, указывающее имя приложения источника, отправляющего связанный объект</span><span class="sxs-lookup"><span data-stu-id="b5618-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="b5618-144">displayName</span><span class="sxs-lookup"><span data-stu-id="b5618-144">displayName</span></span>|<span data-ttu-id="b5618-145">String</span><span class="sxs-lookup"><span data-stu-id="b5618-145">String</span></span>|<span data-ttu-id="b5618-146">Поле, указывающее название связанного объекта.</span><span class="sxs-lookup"><span data-stu-id="b5618-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="b5618-147">externalId</span><span class="sxs-lookup"><span data-stu-id="b5618-147">externalId</span></span>|<span data-ttu-id="b5618-148">String</span><span class="sxs-lookup"><span data-stu-id="b5618-148">String</span></span>|<span data-ttu-id="b5618-149">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="b5618-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="b5618-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5618-150">Response</span></span>

<span data-ttu-id="b5618-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5618-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5618-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5618-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5618-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5618-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b5618-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5618-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b5618-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5618-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b5618-156">C#</span><span class="sxs-lookup"><span data-stu-id="b5618-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5618-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5618-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5618-158">Java</span><span class="sxs-lookup"><span data-stu-id="b5618-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-linkedresource-from-linkedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b5618-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5618-159">Response</span></span>
<span data-ttu-id="b5618-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b5618-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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



