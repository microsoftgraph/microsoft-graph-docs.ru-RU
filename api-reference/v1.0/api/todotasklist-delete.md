---
title: Удаление Тодотасклист
description: Удаляет объект Тодотасклист.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 83944ea1b4749a556646fe6133facb14e88d612c
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797350"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="cb0f7-103">Удаление Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="cb0f7-103">Delete todoTaskList</span></span>
<span data-ttu-id="cb0f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb0f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb0f7-105">Удаляет объект [тодотасклист](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="cb0f7-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb0f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb0f7-106">Permissions</span></span>
<span data-ttu-id="cb0f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb0f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb0f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb0f7-109">Permission type</span></span>|<span data-ttu-id="cb0f7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb0f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb0f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb0f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb0f7-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cb0f7-112">Tasks.Read</span></span>|
|<span data-ttu-id="cb0f7-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb0f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb0f7-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cb0f7-114">Tasks.Read</span></span>|
|<span data-ttu-id="cb0f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb0f7-115">Application</span></span>|<span data-ttu-id="cb0f7-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cb0f7-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb0f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb0f7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="cb0f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb0f7-118">Request headers</span></span>
|<span data-ttu-id="cb0f7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cb0f7-119">Name</span></span>|<span data-ttu-id="cb0f7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cb0f7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb0f7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb0f7-121">Authorization</span></span>|<span data-ttu-id="cb0f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb0f7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb0f7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb0f7-124">Request body</span></span>
<span data-ttu-id="cb0f7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb0f7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb0f7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb0f7-126">Response</span></span>

<span data-ttu-id="cb0f7-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cb0f7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cb0f7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb0f7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb0f7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb0f7-129">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```


### <a name="response"></a><span data-ttu-id="cb0f7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb0f7-130">Response</span></span>
<span data-ttu-id="cb0f7-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb0f7-131">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



