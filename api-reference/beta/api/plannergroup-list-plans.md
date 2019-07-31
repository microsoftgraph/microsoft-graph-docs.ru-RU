---
title: Список планов
description: Получение списка объектов **plannerPlan**, принадлежащих объекту group.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: d062f7b18f8f1d1b7e0a79b948385a08a6f0ed1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979083"
---
# <a name="list-plans"></a><span data-ttu-id="9d75c-103">Список планов</span><span class="sxs-lookup"><span data-stu-id="9d75c-103">List plans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d75c-104">Получение списка объектов **plannerPlan**, принадлежащих объекту [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="9d75c-104">Retrieve a list of **plannerPlan** objects owned by a [group](../resources/group.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d75c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d75c-105">Permissions</span></span>
<span data-ttu-id="9d75c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d75c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d75c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d75c-108">Permission type</span></span>      | <span data-ttu-id="9d75c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d75c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d75c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d75c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d75c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d75c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d75c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d75c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d75c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d75c-113">Not supported.</span></span>    |
|<span data-ttu-id="9d75c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d75c-114">Application</span></span> | <span data-ttu-id="9d75c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d75c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d75c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d75c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{group-id}/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="9d75c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d75c-117">Request headers</span></span>
| <span data-ttu-id="9d75c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9d75c-118">Name</span></span>      |<span data-ttu-id="9d75c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9d75c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d75c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d75c-120">Authorization</span></span>  | <span data-ttu-id="9d75c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d75c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d75c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d75c-123">Request body</span></span>
<span data-ttu-id="9d75c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d75c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d75c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d75c-125">Response</span></span>

<span data-ttu-id="9d75c-126">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9d75c-126">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="9d75c-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="9d75c-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="9d75c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9d75c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d75c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d75c-131">Request</span></span>
<span data-ttu-id="9d75c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d75c-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d75c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d75c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874/planner/plans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d75c-134">C#</span><span class="sxs-lookup"><span data-stu-id="9d75c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d75c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="9d75c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d75c-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9d75c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9d75c-137">Java</span><span class="sxs-lookup"><span data-stu-id="9d75c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9d75c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d75c-138">Response</span></span>
<span data-ttu-id="9d75c-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d75c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
