---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: f4e8261efd52ac4871315c18d569e43495dc8f80
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375690"
---
# <a name="delete-an-activity"></a><span data-ttu-id="6f051-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="6f051-103">Delete an activity</span></span>

<span data-ttu-id="6f051-104">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="6f051-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f051-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f051-105">Permissions</span></span>

<span data-ttu-id="6f051-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f051-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6f051-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f051-108">Permission type</span></span>      | <span data-ttu-id="6f051-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f051-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f051-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f051-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f051-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6f051-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6f051-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f051-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f051-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6f051-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6f051-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f051-114">Application</span></span> | <span data-ttu-id="6f051-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f051-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f051-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f051-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6f051-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f051-117">Request headers</span></span>

|<span data-ttu-id="6f051-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6f051-118">Name</span></span> | <span data-ttu-id="6f051-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6f051-119">Type</span></span> | <span data-ttu-id="6f051-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f051-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="6f051-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f051-121">Authorization</span></span> | <span data-ttu-id="6f051-122">string</span><span class="sxs-lookup"><span data-stu-id="6f051-122">string</span></span> | <span data-ttu-id="6f051-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f051-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f051-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f051-125">Request body</span></span>

<span data-ttu-id="6f051-126">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="6f051-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="6f051-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f051-127">Response</span></span>

<span data-ttu-id="6f051-128">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если действие было удалено.</span><span class="sxs-lookup"><span data-stu-id="6f051-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="6f051-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6f051-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6f051-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f051-130">Request</span></span>

<span data-ttu-id="6f051-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f051-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6f051-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f051-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f051-133">C#</span><span class="sxs-lookup"><span data-stu-id="6f051-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f051-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f051-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f051-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6f051-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6f051-136">Java</span><span class="sxs-lookup"><span data-stu-id="6f051-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6f051-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f051-137">Response</span></span>

<span data-ttu-id="6f051-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f051-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
