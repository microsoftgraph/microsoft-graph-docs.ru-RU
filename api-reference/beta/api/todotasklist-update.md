---
title: Обновление Тодотасклист
description: Обновление свойств объекта Тодотасклист.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f7689ee98e8bcc511285fbf87f3f010e2b22a08b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312780"
---
# <a name="update-todotasklist"></a><span data-ttu-id="75a01-103">Обновление Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="75a01-103">Update todoTaskList</span></span>
<span data-ttu-id="75a01-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="75a01-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="75a01-105">Обновление свойств объекта [тодотасклист](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="75a01-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75a01-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75a01-106">Permissions</span></span>
<span data-ttu-id="75a01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75a01-109">Permission type</span></span>|<span data-ttu-id="75a01-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75a01-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75a01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75a01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75a01-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75a01-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="75a01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75a01-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75a01-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75a01-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="75a01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75a01-115">Application</span></span>|<span data-ttu-id="75a01-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="75a01-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="75a01-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75a01-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="75a01-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75a01-118">Request headers</span></span>
|<span data-ttu-id="75a01-119">Имя</span><span class="sxs-lookup"><span data-stu-id="75a01-119">Name</span></span>|<span data-ttu-id="75a01-120">Описание</span><span class="sxs-lookup"><span data-stu-id="75a01-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75a01-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75a01-121">Authorization</span></span>|<span data-ttu-id="75a01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a01-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75a01-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75a01-124">Content-Type</span></span>|<span data-ttu-id="75a01-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a01-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75a01-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75a01-127">Request body</span></span>
<span data-ttu-id="75a01-128">В тексте запроса добавьте представление объекта [тодотасклист](../resources/todotasklist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75a01-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="75a01-129">В следующей таблице приведены свойства, необходимые при создании [тодотасклист](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="75a01-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="75a01-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75a01-130">Property</span></span>|<span data-ttu-id="75a01-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75a01-131">Type</span></span>|<span data-ttu-id="75a01-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75a01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a01-133">displayName</span><span class="sxs-lookup"><span data-stu-id="75a01-133">displayName</span></span>|<span data-ttu-id="75a01-134">String</span><span class="sxs-lookup"><span data-stu-id="75a01-134">String</span></span>|<span data-ttu-id="75a01-135">Поле, указывающее обновленное название списка задач.</span><span class="sxs-lookup"><span data-stu-id="75a01-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="75a01-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a01-136">Response</span></span>

<span data-ttu-id="75a01-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [тодотасклист](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75a01-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75a01-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="75a01-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75a01-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="75a01-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="75a01-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="75a01-140">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="75a01-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75a01-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="75a01-142">C#</span><span class="sxs-lookup"><span data-stu-id="75a01-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75a01-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75a01-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="75a01-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a01-144">Response</span></span>
<span data-ttu-id="75a01-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75a01-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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



