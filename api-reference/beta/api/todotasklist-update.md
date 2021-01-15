---
title: Обновление todoTaskList
description: Обновление свойств объекта todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 582e9eb65ab0670d1f5c5e735c156e0ac414a19e
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873194"
---
# <a name="update-todotasklist"></a><span data-ttu-id="485ec-103">Обновление todoTaskList</span><span class="sxs-lookup"><span data-stu-id="485ec-103">Update todoTaskList</span></span>
<span data-ttu-id="485ec-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="485ec-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="485ec-105">Обновление свойств объекта [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="485ec-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="485ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="485ec-106">Permissions</span></span>
<span data-ttu-id="485ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="485ec-109">Permission type</span></span>|<span data-ttu-id="485ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="485ec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="485ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="485ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="485ec-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485ec-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="485ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="485ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="485ec-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485ec-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="485ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="485ec-115">Application</span></span>|<span data-ttu-id="485ec-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="485ec-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="485ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="485ec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="485ec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="485ec-118">Request headers</span></span>
|<span data-ttu-id="485ec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="485ec-119">Name</span></span>|<span data-ttu-id="485ec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="485ec-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="485ec-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="485ec-121">Authorization</span></span>|<span data-ttu-id="485ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485ec-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="485ec-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="485ec-124">Content-Type</span></span>|<span data-ttu-id="485ec-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485ec-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="485ec-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="485ec-127">Request body</span></span>
<span data-ttu-id="485ec-128">В теле запроса укажу представление объекта [todoTaskList](../resources/todotasklist.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="485ec-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="485ec-129">В следующей таблице показаны свойства, необходимые при создании [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="485ec-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="485ec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="485ec-130">Property</span></span>|<span data-ttu-id="485ec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="485ec-131">Type</span></span>|<span data-ttu-id="485ec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="485ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="485ec-133">displayName</span><span class="sxs-lookup"><span data-stu-id="485ec-133">displayName</span></span>|<span data-ttu-id="485ec-134">String</span><span class="sxs-lookup"><span data-stu-id="485ec-134">String</span></span>|<span data-ttu-id="485ec-135">Поле, указывающее обновленный заголовок списка задач.</span><span class="sxs-lookup"><span data-stu-id="485ec-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="485ec-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="485ec-136">Response</span></span>

<span data-ttu-id="485ec-137">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [todoTaskList](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="485ec-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="485ec-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="485ec-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="485ec-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="485ec-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="485ec-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="485ec-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPWAAA="],
  "name": "update_todotasklist"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPWAAA=
Content-Type: application/json
Content-length: 167

{
  "displayName": "Vacation Plan"
}
```
# <a name="javascript"></a>[<span data-ttu-id="485ec-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="485ec-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="485ec-142">C#</span><span class="sxs-lookup"><span data-stu-id="485ec-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="485ec-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="485ec-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="485ec-144">Java</span><span class="sxs-lookup"><span data-stu-id="485ec-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="485ec-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="485ec-145">Response</span></span>
<span data-ttu-id="485ec-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="485ec-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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



