---
title: Создание Линкедресаурце
description: Создание нового объекта Линкедресаурце.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f915765192cf039c2095bac7e64a573d9b43b595
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797338"
---
# <a name="create-linkedresource"></a><span data-ttu-id="2e2d0-103">Создание Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="2e2d0-103">Create linkedResource</span></span>
<span data-ttu-id="2e2d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e2d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e2d0-105">Создайте объект [линкедресаурце](../resources/linkedresource.md) для связи указанной [задачи](../resources/todotask.md) с элементом партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="2e2d0-106">Например, вы можете связать задачу с элементом электронной почты в Outlook, спурред задачу, а также создать объект **линкедресаурце** для отслеживания его связи.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="2e2d0-107">Вы также можете создать объект **линкедресаурце** во время [создания задачи](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span><span class="sxs-lookup"><span data-stu-id="2e2d0-107">You can also create a **linkedResource** object while [creating a task](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e2d0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e2d0-108">Permissions</span></span>
<span data-ttu-id="2e2d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e2d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e2d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e2d0-111">Permission type</span></span>|<span data-ttu-id="2e2d0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e2d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e2d0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e2d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e2d0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e2d0-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2e2d0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e2d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e2d0-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e2d0-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2e2d0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e2d0-117">Application</span></span>|<span data-ttu-id="2e2d0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e2d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e2d0-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="2e2d0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e2d0-120">Request headers</span></span>
|<span data-ttu-id="2e2d0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2e2d0-121">Name</span></span>|<span data-ttu-id="2e2d0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2e2d0-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2e2d0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e2d0-123">Authorization</span></span>|<span data-ttu-id="2e2d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2e2d0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e2d0-126">Content-Type</span></span>|<span data-ttu-id="2e2d0-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e2d0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e2d0-129">Request body</span></span>
<span data-ttu-id="2e2d0-130">В тексте запроса добавьте представление объекта [линкедресаурце](../resources/linkedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="2e2d0-131">В следующей таблице приведены свойства, необходимые при создании [линкедресаурце](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="2e2d0-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="2e2d0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e2d0-132">Property</span></span>|<span data-ttu-id="2e2d0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2e2d0-133">Type</span></span>|<span data-ttu-id="2e2d0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2e2d0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e2d0-135">id</span><span class="sxs-lookup"><span data-stu-id="2e2d0-135">id</span></span>|<span data-ttu-id="2e2d0-136">String</span><span class="sxs-lookup"><span data-stu-id="2e2d0-136">String</span></span>|<span data-ttu-id="2e2d0-137">Созданный сервером идентификатор связанной сущности, унаследованной от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="2e2d0-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="2e2d0-138">webUrl</span><span class="sxs-lookup"><span data-stu-id="2e2d0-138">webUrl</span></span>|<span data-ttu-id="2e2d0-139">String</span><span class="sxs-lookup"><span data-stu-id="2e2d0-139">String</span></span>|<span data-ttu-id="2e2d0-140">Прямой ссылки на связанный объект</span><span class="sxs-lookup"><span data-stu-id="2e2d0-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="2e2d0-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="2e2d0-141">applicationName</span></span>|<span data-ttu-id="2e2d0-142">String</span><span class="sxs-lookup"><span data-stu-id="2e2d0-142">String</span></span>|<span data-ttu-id="2e2d0-143">Поле, указывающее имя приложения источника, отправляющего связанный объект</span><span class="sxs-lookup"><span data-stu-id="2e2d0-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="2e2d0-144">displayName</span><span class="sxs-lookup"><span data-stu-id="2e2d0-144">displayName</span></span>|<span data-ttu-id="2e2d0-145">String</span><span class="sxs-lookup"><span data-stu-id="2e2d0-145">String</span></span>|<span data-ttu-id="2e2d0-146">Поле, указывающее название связанного объекта.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="2e2d0-147">externalId</span><span class="sxs-lookup"><span data-stu-id="2e2d0-147">externalId</span></span>|<span data-ttu-id="2e2d0-148">String</span><span class="sxs-lookup"><span data-stu-id="2e2d0-148">String</span></span>|<span data-ttu-id="2e2d0-149">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="2e2d0-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="2e2d0-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e2d0-150">Response</span></span>

<span data-ttu-id="2e2d0-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e2d0-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e2d0-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e2d0-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e2d0-153">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="2e2d0-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e2d0-154">Response</span></span>
<span data-ttu-id="2e2d0-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e2d0-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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



