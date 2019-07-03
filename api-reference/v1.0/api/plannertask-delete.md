---
title: Удаление объекта plannerTask
description: Удаление объекта **plannerTask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5b8262f934c522b945a2920b30a63f13601fe67d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458504"
---
# <a name="delete-plannertask"></a><span data-ttu-id="4fea6-103">Удаление объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="4fea6-103">Delete plannerTask</span></span>

<span data-ttu-id="4fea6-104">Удаление объекта **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="4fea6-104">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="4fea6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fea6-105">Permissions</span></span>
<span data-ttu-id="4fea6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fea6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fea6-108">Permission type</span></span>      | <span data-ttu-id="4fea6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fea6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fea6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fea6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4fea6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fea6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4fea6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fea6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fea6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fea6-113">Not supported.</span></span>    |
|<span data-ttu-id="4fea6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fea6-114">Application</span></span> | <span data-ttu-id="4fea6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fea6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fea6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fea6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4fea6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fea6-117">Request headers</span></span>
| <span data-ttu-id="4fea6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4fea6-118">Name</span></span>       | <span data-ttu-id="4fea6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4fea6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4fea6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fea6-120">Authorization</span></span>  | <span data-ttu-id="4fea6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fea6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fea6-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="4fea6-123">If-Match</span></span>  | <span data-ttu-id="4fea6-p103">Последнее известное значение ETag удаляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fea6-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fea6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fea6-126">Request body</span></span>
<span data-ttu-id="4fea6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fea6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fea6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fea6-128">Response</span></span>

<span data-ttu-id="4fea6-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4fea6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="4fea6-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4fea6-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4fea6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4fea6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fea6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fea6-135">Request</span></span>
<span data-ttu-id="4fea6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fea6-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4fea6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fea6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/tasks/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4fea6-138">C#</span><span class="sxs-lookup"><span data-stu-id="4fea6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fea6-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4fea6-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4fea6-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4fea6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannertask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4fea6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fea6-141">Response</span></span>
<span data-ttu-id="4fea6-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fea6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
