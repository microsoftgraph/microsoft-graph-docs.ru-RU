---
title: Создание Тодотасклист
description: Создание нового объекта lists.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a0753faa0c417d8e3f5fec326b27043e14b5a5ad
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872866"
---
# <a name="create-todotasklist"></a><span data-ttu-id="3265b-103">Создание Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="3265b-103">Create todoTaskList</span></span>
<span data-ttu-id="3265b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3265b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3265b-105">Создание нового объекта lists.</span><span class="sxs-lookup"><span data-stu-id="3265b-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3265b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3265b-106">Permissions</span></span>
<span data-ttu-id="3265b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3265b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3265b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3265b-109">Permission type</span></span>|<span data-ttu-id="3265b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3265b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3265b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3265b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3265b-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3265b-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="3265b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3265b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3265b-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3265b-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="3265b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3265b-115">Application</span></span>|<span data-ttu-id="3265b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3265b-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="3265b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3265b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="3265b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3265b-118">Request headers</span></span>
|<span data-ttu-id="3265b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3265b-119">Name</span></span>|<span data-ttu-id="3265b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3265b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3265b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3265b-121">Authorization</span></span>|<span data-ttu-id="3265b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3265b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3265b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3265b-124">Content-Type</span></span>|<span data-ttu-id="3265b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3265b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3265b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3265b-127">Request body</span></span>
<span data-ttu-id="3265b-128">В тексте запроса добавьте представление объекта [тодотасклист](../resources/todotasklist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3265b-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="3265b-129">В следующей таблице приведены свойства, необходимые при создании [тодотасклист](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="3265b-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="3265b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3265b-130">Property</span></span>|<span data-ttu-id="3265b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3265b-131">Type</span></span>|<span data-ttu-id="3265b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3265b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3265b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3265b-133">displayName</span></span>|<span data-ttu-id="3265b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3265b-134">String</span></span>|<span data-ttu-id="3265b-135">Поле, указывающее название списка задач.</span><span class="sxs-lookup"><span data-stu-id="3265b-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="3265b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="3265b-136">Response</span></span>

<span data-ttu-id="3265b-137">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тодотасклист](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3265b-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3265b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="3265b-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3265b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3265b-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3265b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3265b-140">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="3265b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3265b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotasklist-from-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3265b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3265b-142">Response</span></span>
<span data-ttu-id="3265b-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3265b-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
