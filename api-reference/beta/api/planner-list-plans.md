---
title: Список планов
description: Получение списка объектов **plannerplan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e61cc743435574328e5dd5880d1e6fe2368eaa5d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454162"
---
# <a name="list-plans"></a><span data-ttu-id="6f9b8-103">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="6f9b8-103">List plans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f9b8-104">Получение списка объектов **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-104">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f9b8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9b8-105">Permissions</span></span>
<span data-ttu-id="6f9b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f9b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f9b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9b8-108">Permission type</span></span>      | <span data-ttu-id="6f9b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f9b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f9b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f9b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f9b8-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f9b8-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f9b8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f9b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f9b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-113">Not supported.</span></span>    |
|<span data-ttu-id="6f9b8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f9b8-114">Application</span></span> | <span data-ttu-id="6f9b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f9b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f9b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f9b8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6f9b8-117">Optional query parameters</span></span>
<span data-ttu-id="6f9b8-118">Этот метод требует указания [фильтра](https://developer.microsoft.com/graph/docs/concepts/query_parameters) по владельцу.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-118">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f9b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f9b8-119">Request headers</span></span>
| <span data-ttu-id="6f9b8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6f9b8-120">Name</span></span>      |<span data-ttu-id="6f9b8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6f9b8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6f9b8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f9b8-122">Authorization</span></span>  | <span data-ttu-id="6f9b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f9b8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f9b8-125">Request body</span></span>
<span data-ttu-id="6f9b8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f9b8-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f9b8-127">Response</span></span>

<span data-ttu-id="6f9b8-128">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-128">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="6f9b8-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="6f9b8-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6f9b8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6f9b8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f9b8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f9b8-133">Request</span></span>
<span data-ttu-id="6f9b8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6f9b8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f9b8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f9b8-136">C#</span><span class="sxs-lookup"><span data-stu-id="6f9b8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f9b8-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="6f9b8-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f9b8-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6f9b8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6f9b8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f9b8-139">Response</span></span>
<span data-ttu-id="6f9b8-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f9b8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
