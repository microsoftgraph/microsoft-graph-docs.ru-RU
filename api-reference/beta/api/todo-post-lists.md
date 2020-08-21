---
title: Создание объекта todoTaskList
description: Создание объекта lists.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2628721edff8ad1dad559e590c3dade972220c73
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850075"
---
# <a name="create-todotasklist"></a><span data-ttu-id="1a644-103">Создание объекта todoTaskList</span><span class="sxs-lookup"><span data-stu-id="1a644-103">Create todoTaskList</span></span>
<span data-ttu-id="1a644-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a644-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a644-105">Создание объекта lists.</span><span class="sxs-lookup"><span data-stu-id="1a644-105">Create a new lists object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a644-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a644-106">Permissions</span></span>
<span data-ttu-id="1a644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a644-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a644-109">Permission type</span></span>|<span data-ttu-id="1a644-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a644-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a644-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a644-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a644-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a644-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1a644-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a644-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a644-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a644-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="1a644-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a644-115">Application</span></span>|<span data-ttu-id="1a644-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1a644-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a644-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a644-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists
POST /users/{id|userPrincipalName}/todo/lists
```

## <a name="request-headers"></a><span data-ttu-id="1a644-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a644-118">Request headers</span></span>
|<span data-ttu-id="1a644-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1a644-119">Name</span></span>|<span data-ttu-id="1a644-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1a644-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1a644-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a644-121">Authorization</span></span>|<span data-ttu-id="1a644-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a644-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1a644-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a644-124">Content-Type</span></span>|<span data-ttu-id="1a644-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a644-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a644-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a644-127">Request body</span></span>
<span data-ttu-id="1a644-128">Представьте в тексте запроса описание объекта [todoTaskList в формате JSON.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="1a644-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="1a644-129">В приведенной ниже таблице указаны свойства, необходимые при создании [объекта todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="1a644-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="1a644-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a644-130">Property</span></span>|<span data-ttu-id="1a644-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1a644-131">Type</span></span>|<span data-ttu-id="1a644-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a644-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a644-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1a644-133">displayName</span></span>|<span data-ttu-id="1a644-134">String</span><span class="sxs-lookup"><span data-stu-id="1a644-134">String</span></span>|<span data-ttu-id="1a644-135">Поле, обозначающее заголовок списка задач.</span><span class="sxs-lookup"><span data-stu-id="1a644-135">Field indicating title of the task list.</span></span>|

## <a name="response"></a><span data-ttu-id="1a644-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a644-136">Response</span></span>

<span data-ttu-id="1a644-137">При успешном выполнении этот метод возвращает код `201 Created` ответа [и объект todoTaskList](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a644-137">If successful, this method returns a `201 Created` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a644-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a644-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a644-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a644-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="1a644-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a644-140">Response</span></span>
<span data-ttu-id="1a644-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1a644-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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