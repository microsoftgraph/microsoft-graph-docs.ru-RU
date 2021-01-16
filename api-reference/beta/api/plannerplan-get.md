---
title: Получение объекта plannerPlan
description: Получение свойств и связей объекта **plannerplan**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e6b0df111dba9a5c3a1c27b05951a30fdaefe4f0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882921"
---
# <a name="get-plannerplan"></a><span data-ttu-id="fde96-103">Получение объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fde96-103">Get plannerPlan</span></span>

<span data-ttu-id="fde96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fde96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fde96-105">Извлечение свойств и связей объекта [plannerplan.](../resources/plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="fde96-105">Retrieve the properties and relationships of a [plannerplan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fde96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fde96-106">Permissions</span></span>
<span data-ttu-id="fde96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fde96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fde96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fde96-109">Permission type</span></span>      | <span data-ttu-id="fde96-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fde96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fde96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fde96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fde96-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fde96-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fde96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fde96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fde96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde96-114">Not supported.</span></span>    |
|<span data-ttu-id="fde96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fde96-115">Application</span></span> | <span data-ttu-id="fde96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde96-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fde96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fde96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}
```
## <a name="request-headers"></a><span data-ttu-id="fde96-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fde96-118">Request headers</span></span>
| <span data-ttu-id="fde96-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fde96-119">Name</span></span>      |<span data-ttu-id="fde96-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fde96-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fde96-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fde96-121">Authorization</span></span>  | <span data-ttu-id="fde96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fde96-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fde96-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fde96-124">Request body</span></span>
<span data-ttu-id="fde96-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fde96-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fde96-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde96-126">Response</span></span>

<span data-ttu-id="fde96-127">В случае успеха этот метод возвращает код отклика и объект `200 OK` [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fde96-127">If successful, this method returns a `200 OK` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="fde96-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="fde96-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="fde96-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fde96-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fde96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fde96-132">Request</span></span>
<span data-ttu-id="fde96-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fde96-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fde96-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fde96-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/plans/{id}
```
# <a name="c"></a>[<span data-ttu-id="fde96-135">C#</span><span class="sxs-lookup"><span data-stu-id="fde96-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fde96-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fde96-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fde96-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fde96-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fde96-138">Java</span><span class="sxs-lookup"><span data-stu-id="fde96-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fde96-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fde96-139">Response</span></span>
<span data-ttu-id="fde96-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fde96-140">Here is an example of the response.</span></span> 

><span data-ttu-id="fde96-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fde96-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


