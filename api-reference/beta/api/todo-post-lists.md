---
title: Создание Тодотасклист
description: Создание нового объекта lists.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 91b7211e15d02dd97101ca513be8cb85147c23a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010448"
---
# <a name="create-todotasklist"></a><span data-ttu-id="553ce-103">Создание Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="553ce-103">Create todoTaskList</span></span>
<span data-ttu-id="553ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="553ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="553ce-105">Создание нового объекта lists.</span><span class="sxs-lookup"><span data-stu-id="553ce-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="553ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="553ce-106">Permissions</span></span>
<span data-ttu-id="553ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="553ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553ce-109">Permission type</span></span>|<span data-ttu-id="553ce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="553ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="553ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="553ce-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553ce-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="553ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="553ce-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553ce-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="553ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="553ce-115">Application</span></span>|<span data-ttu-id="553ce-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="553ce-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="553ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553ce-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="553ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553ce-118">Request headers</span></span>
|<span data-ttu-id="553ce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="553ce-119">Name</span></span>|<span data-ttu-id="553ce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="553ce-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="553ce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="553ce-121">Authorization</span></span>|<span data-ttu-id="553ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="553ce-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="553ce-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="553ce-124">Content-Type</span></span>|<span data-ttu-id="553ce-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="553ce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="553ce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="553ce-127">Request body</span></span>
<span data-ttu-id="553ce-128">В тексте запроса добавьте представление объекта [тодотасклист](../resources/todotasklist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="553ce-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="553ce-129">В следующей таблице приведены свойства, необходимые при создании [тодотасклист](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="553ce-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="553ce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="553ce-130">Property</span></span>|<span data-ttu-id="553ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="553ce-131">Type</span></span>|<span data-ttu-id="553ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="553ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="553ce-133">displayName</span><span class="sxs-lookup"><span data-stu-id="553ce-133">displayName</span></span>|<span data-ttu-id="553ce-134">String</span><span class="sxs-lookup"><span data-stu-id="553ce-134">String</span></span>|<span data-ttu-id="553ce-135">Поле, указывающее название списка задач.</span><span class="sxs-lookup"><span data-stu-id="553ce-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="553ce-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="553ce-136">Response</span></span>

<span data-ttu-id="553ce-137">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тодотасклист](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="553ce-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="553ce-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="553ce-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="553ce-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="553ce-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="553ce-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="553ce-140">HTTP</span></span>](#tab/http)
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
  "displayName": "Travel items",
}
```
# <a name="javascript"></a>[<span data-ttu-id="553ce-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="553ce-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="553ce-142">C#</span><span class="sxs-lookup"><span data-stu-id="553ce-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotasklist-from-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="553ce-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="553ce-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotasklist-from-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="553ce-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="553ce-144">Response</span></span>
<span data-ttu-id="553ce-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="553ce-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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


