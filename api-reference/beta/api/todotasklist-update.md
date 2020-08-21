---
title: Обновление объекта todoTaskList
description: Обновление свойств объекта todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bedcf564fdc470a6bfcf1dacafe2efa82694e0ed
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850051"
---
# <a name="update-todotasklist"></a><span data-ttu-id="12309-103">Обновление объекта todoTaskList</span><span class="sxs-lookup"><span data-stu-id="12309-103">Update todoTaskList</span></span>
<span data-ttu-id="12309-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="12309-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="12309-105">Обновление свойств объекта [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="12309-105">Update the properties of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12309-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12309-106">Permissions</span></span>
<span data-ttu-id="12309-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12309-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12309-109">Permission type</span></span>|<span data-ttu-id="12309-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12309-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12309-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12309-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12309-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12309-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="12309-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12309-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12309-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12309-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="12309-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12309-115">Application</span></span>|<span data-ttu-id="12309-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12309-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="12309-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12309-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="12309-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12309-118">Request headers</span></span>
|<span data-ttu-id="12309-119">Имя</span><span class="sxs-lookup"><span data-stu-id="12309-119">Name</span></span>|<span data-ttu-id="12309-120">Описание</span><span class="sxs-lookup"><span data-stu-id="12309-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="12309-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12309-121">Authorization</span></span>|<span data-ttu-id="12309-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12309-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="12309-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12309-124">Content-Type</span></span>|<span data-ttu-id="12309-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12309-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12309-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12309-127">Request body</span></span>
<span data-ttu-id="12309-128">Представьте в тексте запроса описание объекта [todoTaskList в формате JSON.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="12309-128">In the request body, supply a JSON representation of the [todoTaskList](../resources/todotasklist.md) object.</span></span>

<span data-ttu-id="12309-129">В приведенной ниже таблице указаны свойства, необходимые при создании [объекта todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="12309-129">The following table shows the properties that are required when you create the [todoTaskList](../resources/todotasklist.md).</span></span>

|<span data-ttu-id="12309-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12309-130">Property</span></span>|<span data-ttu-id="12309-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12309-131">Type</span></span>|<span data-ttu-id="12309-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12309-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12309-133">displayName</span><span class="sxs-lookup"><span data-stu-id="12309-133">displayName</span></span>|<span data-ttu-id="12309-134">String</span><span class="sxs-lookup"><span data-stu-id="12309-134">String</span></span>|<span data-ttu-id="12309-135">Поле с информацией об обновленных заголовках списка задач.</span><span class="sxs-lookup"><span data-stu-id="12309-135">Field indicating updated title of the task list.</span></span>|



## <a name="response"></a><span data-ttu-id="12309-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="12309-136">Response</span></span>

<span data-ttu-id="12309-137">При успешном выполнении этот метод возвращает код `200 OK` отклика и [обновленный объект todoTaskList](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12309-137">If successful, this method returns a `200 OK` response code and an updated [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12309-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="12309-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12309-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="12309-139">Request</span></span>
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
  "displayName": "Vacation Plan",
}
```


### <a name="response"></a><span data-ttu-id="12309-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="12309-140">Response</span></span>
<span data-ttu-id="12309-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="12309-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

