---
title: Удаление объекта plannerPlan
description: Удаление объекта **plannerPlan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 3e31dac12c3843f19c036dcc4d58e20e9a961b01
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594574"
---
# <a name="delete-plannerplan"></a><span data-ttu-id="0c223-103">Удаление объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="0c223-103">Delete plannerPlan</span></span>

<span data-ttu-id="0c223-104">Удаление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="0c223-104">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c223-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c223-105">Permissions</span></span>
<span data-ttu-id="0c223-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c223-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c223-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c223-108">Permission type</span></span>      | <span data-ttu-id="0c223-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c223-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c223-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c223-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c223-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c223-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c223-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c223-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c223-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c223-113">Not supported.</span></span>    |
|<span data-ttu-id="0c223-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c223-114">Application</span></span> | <span data-ttu-id="0c223-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c223-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c223-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c223-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0c223-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c223-117">Request headers</span></span>
| <span data-ttu-id="0c223-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0c223-118">Name</span></span>       | <span data-ttu-id="0c223-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0c223-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c223-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c223-120">Authorization</span></span>  | <span data-ttu-id="0c223-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c223-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c223-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="0c223-123">If-Match</span></span>  | <span data-ttu-id="0c223-p103">Последнее известное значение ETag удаляемого объекта **plannerPlan**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c223-p103">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c223-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c223-126">Request body</span></span>
<span data-ttu-id="0c223-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c223-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c223-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c223-128">Response</span></span>

<span data-ttu-id="0c223-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0c223-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="0c223-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="0c223-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0c223-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0c223-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c223-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c223-135">Request</span></span>
<span data-ttu-id="0c223-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c223-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/plans/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="0c223-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c223-137">Response</span></span>
<span data-ttu-id="0c223-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c223-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c223-141">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="0c223-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c223-142">Языках</span><span class="sxs-lookup"><span data-stu-id="0c223-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_plannerplan-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c223-143">Язык</span><span class="sxs-lookup"><span data-stu-id="0c223-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_plannerplan-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplan-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplan-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
