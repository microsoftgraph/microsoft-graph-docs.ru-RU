---
title: Удаление объекта todoTask
description: Удаляет объект todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bdf26a600f64891e3db90d55ff31f47d2df4eee7
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850072"
---
# <a name="delete-todotask"></a><span data-ttu-id="29709-103">Удаление объекта todoTask</span><span class="sxs-lookup"><span data-stu-id="29709-103">Delete todoTask</span></span>
<span data-ttu-id="29709-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="29709-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="29709-105">Удаляет объект [todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="29709-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="29709-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29709-106">Permissions</span></span>
<span data-ttu-id="29709-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29709-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29709-109">Permission type</span></span>|<span data-ttu-id="29709-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29709-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29709-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29709-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29709-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29709-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="29709-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29709-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29709-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29709-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="29709-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29709-115">Application</span></span>|<span data-ttu-id="29709-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="29709-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="29709-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29709-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="29709-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29709-118">Request headers</span></span>
|<span data-ttu-id="29709-119">Имя</span><span class="sxs-lookup"><span data-stu-id="29709-119">Name</span></span>|<span data-ttu-id="29709-120">Описание</span><span class="sxs-lookup"><span data-stu-id="29709-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="29709-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29709-121">Authorization</span></span>|<span data-ttu-id="29709-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29709-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29709-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29709-124">Request body</span></span>
<span data-ttu-id="29709-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29709-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29709-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="29709-126">Response</span></span>

<span data-ttu-id="29709-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="29709-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="29709-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="29709-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29709-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="29709-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```


### <a name="response"></a><span data-ttu-id="29709-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="29709-130">Response</span></span>
<span data-ttu-id="29709-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29709-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

