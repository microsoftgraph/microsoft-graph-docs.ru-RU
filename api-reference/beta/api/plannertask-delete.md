---
title: Удаление объекта plannerTask
description: Удаление объекта **plannerTask**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 48777cec46e1f99547d255f91ccda013849adeb6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473509"
---
# <a name="delete-plannertask"></a><span data-ttu-id="8f119-103">Удаление объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="8f119-103">Delete plannerTask</span></span>

<span data-ttu-id="8f119-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f119-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f119-105">Удаление объекта **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="8f119-105">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f119-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f119-106">Permissions</span></span>
<span data-ttu-id="8f119-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f119-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f119-109">Permission type</span></span>      | <span data-ttu-id="8f119-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f119-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f119-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f119-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8f119-112">Tasks.ReadWrite, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f119-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f119-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f119-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f119-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f119-114">Not supported.</span></span>    |
|<span data-ttu-id="8f119-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f119-115">Application</span></span> | <span data-ttu-id="8f119-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f119-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f119-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f119-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8f119-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f119-118">Request headers</span></span>
| <span data-ttu-id="8f119-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f119-119">Name</span></span>       | <span data-ttu-id="8f119-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f119-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f119-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f119-121">Authorization</span></span>  | <span data-ttu-id="8f119-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f119-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f119-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="8f119-124">If-Match</span></span>  | <span data-ttu-id="8f119-p103">Последнее известное значение ETag удаляемого объекта **plannerTask**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f119-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f119-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f119-127">Request body</span></span>
<span data-ttu-id="8f119-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f119-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f119-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f119-129">Response</span></span>

<span data-ttu-id="8f119-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8f119-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="8f119-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8f119-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8f119-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8f119-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f119-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f119-136">Request</span></span>
<span data-ttu-id="8f119-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f119-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f119-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f119-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/tasks/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="c"></a>[<span data-ttu-id="8f119-139">C#</span><span class="sxs-lookup"><span data-stu-id="8f119-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannertask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f119-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f119-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannertask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f119-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f119-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannertask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f119-142">Java</span><span class="sxs-lookup"><span data-stu-id="8f119-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannertask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8f119-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f119-143">Response</span></span>
<span data-ttu-id="8f119-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f119-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


