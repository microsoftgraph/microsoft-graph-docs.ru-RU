---
title: Удаление действия
description: Удаление существующей активности пользователя для приложения.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: d30fda3d79a7afe6f370a735f6ed6e331fba714b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401535"
---
# <a name="delete-an-activity"></a><span data-ttu-id="84f90-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="84f90-103">Delete an activity</span></span>

<span data-ttu-id="84f90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84f90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84f90-105">Удаление существующей активности пользователя для приложения.</span><span class="sxs-lookup"><span data-stu-id="84f90-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="84f90-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84f90-106">Permissions</span></span>

<span data-ttu-id="84f90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84f90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="84f90-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84f90-109">Permission type</span></span>      | <span data-ttu-id="84f90-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84f90-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84f90-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84f90-111">Delegated (work or school account)</span></span> | <span data-ttu-id="84f90-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="84f90-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="84f90-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84f90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84f90-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="84f90-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="84f90-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84f90-115">Application</span></span> | <span data-ttu-id="84f90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84f90-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84f90-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84f90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84f90-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84f90-118">Request headers</span></span>

|<span data-ttu-id="84f90-119">Имя</span><span class="sxs-lookup"><span data-stu-id="84f90-119">Name</span></span> | <span data-ttu-id="84f90-120">Тип</span><span class="sxs-lookup"><span data-stu-id="84f90-120">Type</span></span> | <span data-ttu-id="84f90-121">Описание</span><span class="sxs-lookup"><span data-stu-id="84f90-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="84f90-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84f90-122">Authorization</span></span> | <span data-ttu-id="84f90-123">string</span><span class="sxs-lookup"><span data-stu-id="84f90-123">string</span></span> | <span data-ttu-id="84f90-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84f90-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84f90-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84f90-126">Request body</span></span>

<span data-ttu-id="84f90-127">Нет тела запроса.</span><span class="sxs-lookup"><span data-stu-id="84f90-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="84f90-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="84f90-128">Response</span></span>

<span data-ttu-id="84f90-129">В случае успешной работы этот метод возвращает код ответа, если `204 No Content` действие удалено.</span><span class="sxs-lookup"><span data-stu-id="84f90-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="84f90-130">Пример</span><span class="sxs-lookup"><span data-stu-id="84f90-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="84f90-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="84f90-131">Request</span></span>

<span data-ttu-id="84f90-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84f90-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="84f90-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="84f90-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="c"></a>[<span data-ttu-id="84f90-134">C#</span><span class="sxs-lookup"><span data-stu-id="84f90-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84f90-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84f90-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84f90-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84f90-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84f90-137">Java</span><span class="sxs-lookup"><span data-stu-id="84f90-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84f90-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="84f90-138">Response</span></span>

<span data-ttu-id="84f90-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84f90-139">The following is an example of the response.</span></span>

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


