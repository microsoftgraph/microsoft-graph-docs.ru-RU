---
title: Создание Линкедресаурце
description: Создание нового объекта Линкедресаурце.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e296600642b3aad7bbd895260da139e5dd1a37c7
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796637"
---
# <a name="create-linkedresource"></a><span data-ttu-id="240c4-103">Создание Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="240c4-103">Create linkedResource</span></span>
<span data-ttu-id="240c4-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="240c4-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="240c4-105">Создайте объект [линкедресаурце](../resources/linkedresource.md) для связи указанной [задачи](../resources/todotask.md) с элементом партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="240c4-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="240c4-106">Например, вы можете связать задачу с элементом электронной почты в Outlook, спурред задачу, а также создать объект **линкедресаурце** для отслеживания его связи.</span><span class="sxs-lookup"><span data-stu-id="240c4-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="240c4-107">Вы также можете создать объект **линкедресаурце** при [создании тодотаск](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span><span class="sxs-lookup"><span data-stu-id="240c4-107">You can also create a **linkedResource** object while [creating a todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="240c4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="240c4-108">Permissions</span></span>
<span data-ttu-id="240c4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="240c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="240c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="240c4-111">Permission type</span></span>|<span data-ttu-id="240c4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="240c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="240c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="240c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="240c4-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="240c4-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="240c4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="240c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="240c4-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="240c4-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="240c4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="240c4-117">Application</span></span>|<span data-ttu-id="240c4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="240c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="240c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="240c4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="240c4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="240c4-120">Request headers</span></span>
|<span data-ttu-id="240c4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="240c4-121">Name</span></span>|<span data-ttu-id="240c4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="240c4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="240c4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="240c4-123">Authorization</span></span>|<span data-ttu-id="240c4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="240c4-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="240c4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="240c4-126">Content-Type</span></span>|<span data-ttu-id="240c4-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="240c4-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="240c4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="240c4-129">Request body</span></span>
<span data-ttu-id="240c4-130">В тексте запроса добавьте представление объекта [линкедресаурце](../resources/linkedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="240c4-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="240c4-131">В следующей таблице приведены свойства, необходимые при создании [линкедресаурце](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="240c4-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="240c4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="240c4-132">Property</span></span>|<span data-ttu-id="240c4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="240c4-133">Type</span></span>|<span data-ttu-id="240c4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="240c4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="240c4-135">id</span><span class="sxs-lookup"><span data-stu-id="240c4-135">id</span></span>|<span data-ttu-id="240c4-136">String</span><span class="sxs-lookup"><span data-stu-id="240c4-136">String</span></span>|<span data-ttu-id="240c4-137">Созданный сервером идентификатор связанной сущности, унаследованной от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="240c4-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="240c4-138">webUrl</span><span class="sxs-lookup"><span data-stu-id="240c4-138">webUrl</span></span>|<span data-ttu-id="240c4-139">String</span><span class="sxs-lookup"><span data-stu-id="240c4-139">String</span></span>|<span data-ttu-id="240c4-140">Прямой ссылки на связанный объект</span><span class="sxs-lookup"><span data-stu-id="240c4-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="240c4-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="240c4-141">applicationName</span></span>|<span data-ttu-id="240c4-142">String</span><span class="sxs-lookup"><span data-stu-id="240c4-142">String</span></span>|<span data-ttu-id="240c4-143">Поле, указывающее имя приложения источника, отправляющего связанный объект</span><span class="sxs-lookup"><span data-stu-id="240c4-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="240c4-144">displayName</span><span class="sxs-lookup"><span data-stu-id="240c4-144">displayName</span></span>|<span data-ttu-id="240c4-145">String</span><span class="sxs-lookup"><span data-stu-id="240c4-145">String</span></span>|<span data-ttu-id="240c4-146">Поле, указывающее название связанного объекта.</span><span class="sxs-lookup"><span data-stu-id="240c4-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="240c4-147">externalId</span><span class="sxs-lookup"><span data-stu-id="240c4-147">externalId</span></span>|<span data-ttu-id="240c4-148">String</span><span class="sxs-lookup"><span data-stu-id="240c4-148">String</span></span>|<span data-ttu-id="240c4-149">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="240c4-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="240c4-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="240c4-150">Response</span></span>

<span data-ttu-id="240c4-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="240c4-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="240c4-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="240c4-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="240c4-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="240c4-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="240c4-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="240c4-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="240c4-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="240c4-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="240c4-156">C#</span><span class="sxs-lookup"><span data-stu-id="240c4-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="240c4-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="240c4-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="240c4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="240c4-158">Response</span></span>
<span data-ttu-id="240c4-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="240c4-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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



