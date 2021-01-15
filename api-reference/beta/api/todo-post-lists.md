---
title: Создание todoTaskList
description: Создание объекта lists.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 92242d0973b3d47af0126f6fefb093d258f46d74
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874083"
---
# <a name="create-todotasklist"></a><span data-ttu-id="f450f-103">Создание todoTaskList</span><span class="sxs-lookup"><span data-stu-id="f450f-103">Create todoTaskList</span></span>
<span data-ttu-id="f450f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f450f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f450f-105">Создание объекта lists.</span><span class="sxs-lookup"><span data-stu-id="f450f-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f450f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f450f-106">Permissions</span></span>
<span data-ttu-id="f450f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f450f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f450f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f450f-109">Permission type</span></span>|<span data-ttu-id="f450f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f450f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f450f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f450f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f450f-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f450f-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f450f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f450f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f450f-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f450f-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="f450f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f450f-115">Application</span></span>|<span data-ttu-id="f450f-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f450f-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="f450f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f450f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="f450f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f450f-118">Request headers</span></span>
|<span data-ttu-id="f450f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f450f-119">Name</span></span>|<span data-ttu-id="f450f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f450f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f450f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f450f-121">Authorization</span></span>|<span data-ttu-id="f450f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f450f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f450f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f450f-124">Content-Type</span></span>|<span data-ttu-id="f450f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f450f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f450f-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="f450f-127">Request body</span></span>
<span data-ttu-id="f450f-128">В теле запроса укажу представление объекта [todoTaskList](../resources/todotasklist.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="f450f-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="f450f-129">В следующей таблице показаны свойства, необходимые при создании [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="f450f-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="f450f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f450f-130">Property</span></span>|<span data-ttu-id="f450f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f450f-131">Type</span></span>|<span data-ttu-id="f450f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f450f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f450f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f450f-133">displayName</span></span>|<span data-ttu-id="f450f-134">String</span><span class="sxs-lookup"><span data-stu-id="f450f-134">String</span></span>|<span data-ttu-id="f450f-135">Поле, указывающее заголовок списка задач.</span><span class="sxs-lookup"><span data-stu-id="f450f-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="f450f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f450f-136">Response</span></span>

<span data-ttu-id="f450f-137">В случае успеха этот метод возвращает код отклика и объект `201 Created` [todoTaskList](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f450f-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f450f-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="f450f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f450f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f450f-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f450f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f450f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_todotasklist_from_lists"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists
Content-Type: application/json
Content-length: 60

{
  "displayName": "Travel items"
}
```
# <a name="javascript"></a>[<span data-ttu-id="f450f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f450f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f450f-142">C#</span><span class="sxs-lookup"><span data-stu-id="f450f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotasklist-from-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f450f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f450f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotasklist-from-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f450f-144">Java</span><span class="sxs-lookup"><span data-stu-id="f450f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotasklist-from-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f450f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f450f-145">Response</span></span>
<span data-ttu-id="f450f-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f450f-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "AAMkADIyAAAhrbPWAAA=",
  "displayName": "Travel items",
  "isOwner": true,
  "isShared": false,
  "wellknownListName": "none"
}
```


