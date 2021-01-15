---
title: Обновление todoTaskList
description: Обновление свойств объекта todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8c575a938bb2a2689860cf3c58e46ae9d43d24c6
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873523"
---
# <a name="update-todotasklist"></a><span data-ttu-id="c662d-103">Обновление todoTaskList</span><span class="sxs-lookup"><span data-stu-id="c662d-103">Update todoTaskList</span></span>
<span data-ttu-id="c662d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c662d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c662d-105">Обновление свойств объекта [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="c662d-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c662d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c662d-106">Permissions</span></span>
<span data-ttu-id="c662d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c662d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c662d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c662d-109">Permission type</span></span>|<span data-ttu-id="c662d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c662d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c662d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c662d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c662d-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c662d-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="c662d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c662d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c662d-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c662d-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="c662d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c662d-115">Application</span></span>|<span data-ttu-id="c662d-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c662d-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="c662d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c662d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="c662d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c662d-118">Request headers</span></span>
|<span data-ttu-id="c662d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c662d-119">Name</span></span>|<span data-ttu-id="c662d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c662d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c662d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c662d-121">Authorization</span></span>|<span data-ttu-id="c662d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c662d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c662d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c662d-124">Content-Type</span></span>|<span data-ttu-id="c662d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c662d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c662d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c662d-127">Request body</span></span>
<span data-ttu-id="c662d-128">В теле запроса укажу представление объекта [todoTaskList](../resources/todotasklist.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="c662d-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="c662d-129">В следующей таблице показаны свойства, необходимые при создании [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="c662d-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="c662d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c662d-130">Property</span></span>|<span data-ttu-id="c662d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c662d-131">Type</span></span>|<span data-ttu-id="c662d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c662d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c662d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c662d-133">displayName</span></span>|<span data-ttu-id="c662d-134">String</span><span class="sxs-lookup"><span data-stu-id="c662d-134">String</span></span>|<span data-ttu-id="c662d-135">Поле, указывающее обновленный заголовок списка задач.</span><span class="sxs-lookup"><span data-stu-id="c662d-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="c662d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c662d-136">Response</span></span>

<span data-ttu-id="c662d-137">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [todoTaskList](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c662d-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c662d-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="c662d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c662d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c662d-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c662d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c662d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPWAAA="],
  "name": "update_todotasklist"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPWAAA=
Content-Type: application/json
Content-length: 167

{
  "displayName": "Vacation Plan"
}
```
# <a name="c"></a>[<span data-ttu-id="c662d-141">C#</span><span class="sxs-lookup"><span data-stu-id="c662d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c662d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c662d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c662d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c662d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c662d-144">Java</span><span class="sxs-lookup"><span data-stu-id="c662d-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c662d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c662d-145">Response</span></span>
<span data-ttu-id="c662d-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c662d-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Vacation Plan",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```



