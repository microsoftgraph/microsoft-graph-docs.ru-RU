---
title: Список планов
description: Получение списка объектов **plannerplan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: c4994950b58341d4c990e2d46d4f90ee743cc40c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455797"
---
# <a name="list-plans"></a><span data-ttu-id="bf9c0-103">Список планов</span><span class="sxs-lookup"><span data-stu-id="bf9c0-103">List plans</span></span>

<span data-ttu-id="bf9c0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bf9c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf9c0-105">Получение списка объектов **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-105">Retrieve a list of **plannerplan** objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf9c0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9c0-106">Permissions</span></span>
<span data-ttu-id="bf9c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9c0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9c0-109">Permission type</span></span>      | <span data-ttu-id="bf9c0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf9c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf9c0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf9c0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf9c0-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9c0-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bf9c0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf9c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf9c0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-114">Not supported.</span></span>    |
|<span data-ttu-id="bf9c0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf9c0-115">Application</span></span> | <span data-ttu-id="bf9c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf9c0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf9c0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bf9c0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf9c0-118">Optional query parameters</span></span>
<span data-ttu-id="bf9c0-119">Этот метод требует указания [фильтра](https://developer.microsoft.com/graph/docs/concepts/query_parameters) по владельцу.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-119">This method requires owner [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf9c0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf9c0-120">Request headers</span></span>
| <span data-ttu-id="bf9c0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bf9c0-121">Name</span></span>      |<span data-ttu-id="bf9c0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bf9c0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf9c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf9c0-123">Authorization</span></span>  | <span data-ttu-id="bf9c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf9c0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf9c0-126">Request body</span></span>
<span data-ttu-id="bf9c0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf9c0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf9c0-128">Response</span></span>

<span data-ttu-id="bf9c0-129">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-129">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="bf9c0-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="bf9c0-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bf9c0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bf9c0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf9c0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf9c0-134">Request</span></span>
<span data-ttu-id="bf9c0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf9c0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf9c0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="bf9c0-137">C#</span><span class="sxs-lookup"><span data-stu-id="bf9c0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf9c0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf9c0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf9c0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf9c0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bf9c0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf9c0-140">Response</span></span>
<span data-ttu-id="bf9c0-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf9c0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
