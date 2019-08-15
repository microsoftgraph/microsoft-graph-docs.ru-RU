---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: 12584b1b84facb6a14155b6ae1cf91112cad33e3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412420"
---
# <a name="delete-an-activity"></a><span data-ttu-id="d5c13-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="d5c13-103">Delete an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5c13-104">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="d5c13-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c13-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5c13-105">Permissions</span></span>

<span data-ttu-id="d5c13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5c13-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5c13-108">Permission type</span></span>      | <span data-ttu-id="d5c13-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5c13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5c13-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5c13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5c13-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d5c13-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d5c13-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5c13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5c13-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d5c13-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d5c13-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5c13-114">Application</span></span> | <span data-ttu-id="d5c13-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5c13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5c13-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5c13-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d5c13-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5c13-117">Request headers</span></span>

|<span data-ttu-id="d5c13-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d5c13-118">Name</span></span> | <span data-ttu-id="d5c13-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d5c13-119">Type</span></span> | <span data-ttu-id="d5c13-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d5c13-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d5c13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c13-121">Authorization</span></span> | <span data-ttu-id="d5c13-122">string</span><span class="sxs-lookup"><span data-stu-id="d5c13-122">string</span></span> | <span data-ttu-id="d5c13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5c13-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c13-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5c13-125">Request body</span></span>

<span data-ttu-id="d5c13-126">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="d5c13-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="d5c13-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5c13-127">Response</span></span>

<span data-ttu-id="d5c13-128">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если действие было удалено.</span><span class="sxs-lookup"><span data-stu-id="d5c13-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="d5c13-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d5c13-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d5c13-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5c13-130">Request</span></span>

<span data-ttu-id="d5c13-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5c13-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5c13-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c13-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5c13-133">C#</span><span class="sxs-lookup"><span data-stu-id="d5c13-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5c13-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5c13-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5c13-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d5c13-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d5c13-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5c13-136">Response</span></span>

<span data-ttu-id="d5c13-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5c13-137">Here is an example of the response.</span></span>

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
