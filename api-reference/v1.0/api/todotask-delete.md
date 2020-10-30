---
title: Удаление Тодотаск
description: Удаляет объект Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ca86b2344e67c86418c8bc5d2d3914148994f1e9
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797451"
---
# <a name="delete-todotask"></a><span data-ttu-id="e4adf-103">Удаление Тодотаск</span><span class="sxs-lookup"><span data-stu-id="e4adf-103">Delete todoTask</span></span>
<span data-ttu-id="e4adf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4adf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4adf-105">Удаляет объект [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="e4adf-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4adf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4adf-106">Permissions</span></span>
<span data-ttu-id="e4adf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4adf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4adf-109">Permission type</span></span>|<span data-ttu-id="e4adf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4adf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4adf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4adf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4adf-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4adf-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e4adf-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4adf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4adf-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4adf-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="e4adf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4adf-115">Application</span></span>|<span data-ttu-id="e4adf-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e4adf-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4adf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4adf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="e4adf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4adf-118">Request headers</span></span>
|<span data-ttu-id="e4adf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e4adf-119">Name</span></span>|<span data-ttu-id="e4adf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e4adf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4adf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4adf-121">Authorization</span></span>|<span data-ttu-id="e4adf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4adf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4adf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4adf-124">Request body</span></span>
<span data-ttu-id="e4adf-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4adf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4adf-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4adf-126">Response</span></span>

<span data-ttu-id="e4adf-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4adf-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e4adf-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e4adf-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4adf-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4adf-129">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```


### <a name="response"></a><span data-ttu-id="e4adf-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4adf-130">Response</span></span>
<span data-ttu-id="e4adf-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e4adf-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



