---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 293c6abe64aec124f280e5e33239f63339753733
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010600"
---
# <a name="delete-an-activity"></a><span data-ttu-id="d8239-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="d8239-103">Delete an activity</span></span>

<span data-ttu-id="d8239-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8239-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8239-105">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="d8239-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8239-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8239-106">Permissions</span></span>

<span data-ttu-id="d8239-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8239-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8239-109">Permission type</span></span>      | <span data-ttu-id="d8239-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8239-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8239-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8239-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d8239-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d8239-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d8239-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8239-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8239-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d8239-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d8239-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8239-115">Application</span></span> | <span data-ttu-id="d8239-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8239-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8239-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8239-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8239-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8239-118">Request headers</span></span>

|<span data-ttu-id="d8239-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d8239-119">Name</span></span> | <span data-ttu-id="d8239-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d8239-120">Type</span></span> | <span data-ttu-id="d8239-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d8239-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d8239-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8239-122">Authorization</span></span> | <span data-ttu-id="d8239-123">string</span><span class="sxs-lookup"><span data-stu-id="d8239-123">string</span></span> | <span data-ttu-id="d8239-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8239-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8239-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8239-126">Request body</span></span>

<span data-ttu-id="d8239-127">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="d8239-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="d8239-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8239-128">Response</span></span>

<span data-ttu-id="d8239-129">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если действие было удалено.</span><span class="sxs-lookup"><span data-stu-id="d8239-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="d8239-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d8239-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8239-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8239-131">Request</span></span>

<span data-ttu-id="d8239-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8239-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d8239-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8239-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="c"></a>[<span data-ttu-id="d8239-134">C#</span><span class="sxs-lookup"><span data-stu-id="d8239-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8239-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8239-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8239-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8239-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8239-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8239-137">Response</span></span>

<span data-ttu-id="d8239-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8239-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


