---
title: Перечисление задач
description: Получение списка объектов **plannerTask**, связанных с объектом plannerBucket.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6414fd311fb3cd93955644f903bcaf0d26ee8348
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264500"
---
# <a name="list-tasks"></a><span data-ttu-id="e1f6d-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="e1f6d-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1f6d-104">Получение списка объектов **plannerTask**, связанных с объектом [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="e1f6d-104">Retrieve a list of **plannerTask** objects associated to a [plannerBucket](../resources/plannerbucket.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1f6d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1f6d-105">Permissions</span></span>
<span data-ttu-id="e1f6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f6d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1f6d-108">Permission type</span></span>      | <span data-ttu-id="e1f6d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1f6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1f6d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1f6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1f6d-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1f6d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1f6d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1f6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1f6d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-113">Not supported.</span></span>    |
|<span data-ttu-id="e1f6d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1f6d-114">Application</span></span> | <span data-ttu-id="e1f6d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1f6d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1f6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/<id>/tasks
```

## <a name="request-headers"></a><span data-ttu-id="e1f6d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1f6d-117">Request headers</span></span>
| <span data-ttu-id="e1f6d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e1f6d-118">Name</span></span>      |<span data-ttu-id="e1f6d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e1f6d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1f6d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1f6d-120">Authorization</span></span>  | <span data-ttu-id="e1f6d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1f6d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1f6d-123">Request body</span></span>
<span data-ttu-id="e1f6d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1f6d-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1f6d-125">Response</span></span>

<span data-ttu-id="e1f6d-126">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="e1f6d-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e1f6d-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e1f6d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e1f6d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1f6d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1f6d-131">Request</span></span>
<span data-ttu-id="e1f6d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/planner/buckets/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/tasks
```
##### <a name="response"></a><span data-ttu-id="e1f6d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1f6d-133">Response</span></span>
<span data-ttu-id="e1f6d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerassignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1f6d-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e1f6d-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1f6d-138">C#</span><span class="sxs-lookup"><span data-stu-id="e1f6d-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tasks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1f6d-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1f6d-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tasks-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e1f6d-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e1f6d-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_tasks-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerbucket-list-tasks.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/plannerbucket-list-tasks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerbucket-list-tasks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
