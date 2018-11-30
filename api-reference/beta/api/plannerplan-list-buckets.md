---
title: Перечисление сегментов
description: Получение списка объектов **plannerbucket**, содержащихся в объекте plannerPlan.
ms.openlocfilehash: 0f20e4f9c59fbaa9f2242142da254e49a107e68b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081249"
---
# <a name="list-buckets"></a><span data-ttu-id="b77cb-103">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="b77cb-103">List buckets</span></span>

> <span data-ttu-id="b77cb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b77cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b77cb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b77cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b77cb-106">Получение списка объектов **plannerbucket**, содержащихся в объекте [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="b77cb-106">Retrieve a list of **plannerbucket** objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b77cb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b77cb-107">Permissions</span></span>
<span data-ttu-id="b77cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b77cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b77cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b77cb-110">Permission type</span></span>      | <span data-ttu-id="b77cb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b77cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b77cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b77cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b77cb-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b77cb-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b77cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b77cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b77cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b77cb-115">Not supported.</span></span>    |
|<span data-ttu-id="b77cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b77cb-116">Application</span></span> | <span data-ttu-id="b77cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b77cb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b77cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b77cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/buckets
```

## <a name="request-headers"></a><span data-ttu-id="b77cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b77cb-119">Request headers</span></span>
| <span data-ttu-id="b77cb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b77cb-120">Name</span></span>      |<span data-ttu-id="b77cb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b77cb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b77cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b77cb-122">Authorization</span></span>  | <span data-ttu-id="b77cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b77cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b77cb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b77cb-125">Request body</span></span>
<span data-ttu-id="b77cb-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b77cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b77cb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b77cb-127">Response</span></span>

<span data-ttu-id="b77cb-128">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b77cb-128">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="b77cb-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b77cb-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="b77cb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b77cb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b77cb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b77cb-133">Request</span></span>
<span data-ttu-id="b77cb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b77cb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/2txjA-BMZEq-bKi6Wfj5aGQAB1OJ/buckets
```
##### <a name="response"></a><span data-ttu-id="b77cb-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b77cb-135">Response</span></span>
<span data-ttu-id="b77cb-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b77cb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->