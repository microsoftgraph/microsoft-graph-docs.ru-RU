---
title: Список планов
description: Получение списка объектов **plannerplan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5dc43ae6aa6cea867e0d04308566b8114fccd10e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276596"
---
# <a name="list-plans"></a><span data-ttu-id="9e934-103">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="9e934-103">List plans</span></span>

<span data-ttu-id="9e934-104">Получение списка объектов **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="9e934-104">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e934-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e934-105">Permissions</span></span>
<span data-ttu-id="9e934-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e934-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e934-108">Permission type</span></span>      | <span data-ttu-id="9e934-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e934-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e934-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e934-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e934-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e934-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e934-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e934-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e934-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e934-113">Not supported.</span></span>    |
|<span data-ttu-id="9e934-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e934-114">Application</span></span> | <span data-ttu-id="9e934-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e934-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e934-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e934-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e934-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e934-117">Optional query parameters</span></span>
<span data-ttu-id="9e934-118">Этот метод требует указания [фильтра](https://developer.microsoft.com/graph/docs/concepts/query_parameters) по владельцу.</span><span class="sxs-lookup"><span data-stu-id="9e934-118">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e934-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e934-119">Request headers</span></span>
| <span data-ttu-id="9e934-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9e934-120">Name</span></span>      |<span data-ttu-id="9e934-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9e934-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e934-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e934-122">Authorization</span></span>  | <span data-ttu-id="9e934-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e934-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e934-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e934-125">Request body</span></span>
<span data-ttu-id="9e934-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e934-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e934-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e934-127">Response</span></span>

<span data-ttu-id="9e934-128">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9e934-128">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="9e934-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9e934-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="9e934-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9e934-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e934-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e934-133">Request</span></span>
<span data-ttu-id="9e934-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e934-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans
```
##### <a name="response"></a><span data-ttu-id="9e934-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e934-135">Response</span></span>
<span data-ttu-id="9e934-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e934-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9e934-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9e934-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9e934-140">C#</span><span class="sxs-lookup"><span data-stu-id="9e934-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plans-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e934-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="9e934-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plans-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9e934-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9e934-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_plans-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/planner-list-plans.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/planner-list-plans.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/planner-list-plans.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
