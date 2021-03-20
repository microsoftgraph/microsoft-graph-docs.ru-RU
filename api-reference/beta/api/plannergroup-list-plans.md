---
title: Список планов
description: Получение списка объектов **plannerPlan**, принадлежащих объекту group.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1c832f393142513ce4f38d9eb49e9c60217549f5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945965"
---
# <a name="list-plans"></a><span data-ttu-id="b5318-103">Список планов</span><span class="sxs-lookup"><span data-stu-id="b5318-103">List plans</span></span>

<span data-ttu-id="b5318-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5318-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5318-105">Получение списка объектов **plannerPlan**, принадлежащих объекту [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="b5318-105">Retrieve a list of **plannerPlan** objects owned by a [group](../resources/group.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5318-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5318-106">Permissions</span></span>
<span data-ttu-id="b5318-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5318-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5318-109">Permission type</span></span>      | <span data-ttu-id="b5318-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5318-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5318-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5318-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5318-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5318-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5318-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5318-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5318-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5318-114">Not supported.</span></span>    |
|<span data-ttu-id="b5318-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5318-115">Application</span></span> | <span data-ttu-id="b5318-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5318-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5318-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5318-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{group-id}/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="b5318-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5318-118">Request headers</span></span>
| <span data-ttu-id="b5318-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b5318-119">Name</span></span>      |<span data-ttu-id="b5318-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b5318-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5318-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5318-121">Authorization</span></span>  | <span data-ttu-id="b5318-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5318-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5318-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5318-124">Request body</span></span>
<span data-ttu-id="b5318-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5318-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5318-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5318-126">Response</span></span>

<span data-ttu-id="b5318-127">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b5318-127">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="b5318-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b5318-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="b5318-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b5318-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5318-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5318-132">Request</span></span>
<span data-ttu-id="b5318-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5318-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5318-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5318-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="b5318-135">C#</span><span class="sxs-lookup"><span data-stu-id="b5318-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5318-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5318-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5318-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5318-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5318-138">Java</span><span class="sxs-lookup"><span data-stu-id="b5318-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5318-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5318-139">Response</span></span>
<span data-ttu-id="b5318-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5318-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "container": {
         "@odata.type": "microsoft.graph.plannerPlanContainer",
         "url": "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874",
         "containerId": "ebf3b108-5234-4e22-b93d-656d7dae5874",
         "type": "group"
      },
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


