---
title: Удаление объекта plannerPlan
description: Удаление объекта **plannerPlan**.
localization_priority: Normal
ms.openlocfilehash: 45354d2db0f2d5cbd06a93086250b13a8af30a58
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884751"
---
# <a name="delete-plannerplan"></a><span data-ttu-id="f577d-103">Удаление объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="f577d-103">Delete plannerPlan</span></span>

<span data-ttu-id="f577d-104">Удаление объекта **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="f577d-104">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="f577d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f577d-105">Permissions</span></span>
<span data-ttu-id="f577d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f577d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f577d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f577d-108">Permission type</span></span>      | <span data-ttu-id="f577d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f577d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f577d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f577d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f577d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f577d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f577d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f577d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f577d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f577d-113">Not supported.</span></span>    |
|<span data-ttu-id="f577d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f577d-114">Application</span></span> | <span data-ttu-id="f577d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f577d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f577d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f577d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f577d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f577d-117">Request headers</span></span>
| <span data-ttu-id="f577d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f577d-118">Name</span></span>       | <span data-ttu-id="f577d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f577d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f577d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f577d-120">Authorization</span></span>  | <span data-ttu-id="f577d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f577d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f577d-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="f577d-123">If-Match</span></span>  | <span data-ttu-id="f577d-p103">Последнее известное значение ETag удаляемого объекта **plannerPlan**. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f577d-p103">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f577d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f577d-126">Request body</span></span>
<span data-ttu-id="f577d-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f577d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f577d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f577d-128">Response</span></span>

<span data-ttu-id="f577d-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f577d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="f577d-p105">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f577d-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f577d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f577d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f577d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f577d-135">Request</span></span>
<span data-ttu-id="f577d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f577d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/plans/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="f577d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="f577d-137">Response</span></span>
<span data-ttu-id="f577d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f577d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
