---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 47be9fbd755b5dbfa10cd88dca5fe66942494817
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051776"
---
# <a name="delete-an-activity"></a><span data-ttu-id="4e483-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="4e483-103">Delete an activity</span></span>

<span data-ttu-id="4e483-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e483-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e483-105">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="4e483-105">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e483-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e483-106">Permissions</span></span>

<span data-ttu-id="4e483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e483-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e483-109">Permission type</span></span>      | <span data-ttu-id="4e483-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e483-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e483-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e483-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4e483-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4e483-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4e483-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e483-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e483-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4e483-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4e483-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e483-115">Application</span></span> | <span data-ttu-id="4e483-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e483-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e483-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e483-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4e483-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e483-118">Request headers</span></span>

|<span data-ttu-id="4e483-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4e483-119">Name</span></span> | <span data-ttu-id="4e483-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4e483-120">Type</span></span> | <span data-ttu-id="4e483-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4e483-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4e483-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e483-122">Authorization</span></span> | <span data-ttu-id="4e483-123">string</span><span class="sxs-lookup"><span data-stu-id="4e483-123">string</span></span> | <span data-ttu-id="4e483-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e483-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e483-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e483-126">Request body</span></span>

<span data-ttu-id="4e483-127">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="4e483-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="4e483-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e483-128">Response</span></span>

<span data-ttu-id="4e483-129">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если действие было удалено.</span><span class="sxs-lookup"><span data-stu-id="4e483-129">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="4e483-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4e483-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4e483-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e483-131">Request</span></span>

<span data-ttu-id="4e483-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e483-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4e483-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e483-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```
# <a name="c"></a>[<span data-ttu-id="4e483-134">C#</span><span class="sxs-lookup"><span data-stu-id="4e483-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e483-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e483-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e483-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e483-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e483-137">Java</span><span class="sxs-lookup"><span data-stu-id="4e483-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e483-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e483-138">Response</span></span>

<span data-ttu-id="4e483-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e483-139">Here is an example of the response.</span></span>

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

