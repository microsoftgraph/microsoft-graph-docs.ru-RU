---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: d4874fee43956afe98eeeb39338195a6d4ae5f1b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510748"
---
# <a name="delete-an-activity"></a><span data-ttu-id="ccd47-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="ccd47-103">Delete an activity</span></span>

<span data-ttu-id="ccd47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccd47-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccd47-105">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="ccd47-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccd47-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd47-106">Permissions</span></span>

<span data-ttu-id="ccd47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ccd47-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd47-109">Permission type</span></span>      | <span data-ttu-id="ccd47-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccd47-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccd47-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccd47-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ccd47-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ccd47-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ccd47-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccd47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd47-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ccd47-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ccd47-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccd47-115">Application</span></span> | <span data-ttu-id="ccd47-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd47-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccd47-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccd47-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ccd47-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccd47-118">Request headers</span></span>

|<span data-ttu-id="ccd47-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ccd47-119">Name</span></span> | <span data-ttu-id="ccd47-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ccd47-120">Type</span></span> | <span data-ttu-id="ccd47-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd47-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ccd47-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccd47-122">Authorization</span></span> | <span data-ttu-id="ccd47-123">string</span><span class="sxs-lookup"><span data-stu-id="ccd47-123">string</span></span> | <span data-ttu-id="ccd47-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccd47-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd47-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccd47-126">Request body</span></span>

<span data-ttu-id="ccd47-127">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="ccd47-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="ccd47-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccd47-128">Response</span></span>

<span data-ttu-id="ccd47-129">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если действие было удалено.</span><span class="sxs-lookup"><span data-stu-id="ccd47-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="ccd47-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ccd47-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ccd47-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccd47-131">Request</span></span>

<span data-ttu-id="ccd47-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccd47-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ccd47-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd47-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```
# <a name="c"></a>[<span data-ttu-id="ccd47-134">C#</span><span class="sxs-lookup"><span data-stu-id="ccd47-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccd47-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccd47-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccd47-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccd47-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccd47-137">Java</span><span class="sxs-lookup"><span data-stu-id="ccd47-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ccd47-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd47-138">Response</span></span>

<span data-ttu-id="ccd47-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccd47-139">Here is an example of the response.</span></span>

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
