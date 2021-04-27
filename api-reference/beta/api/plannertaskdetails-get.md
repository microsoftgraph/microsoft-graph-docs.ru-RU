---
title: Получение объекта plannerTaskDetails
description: Получение свойств и связей объекта **plannertaskdetails**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: eb1318bbb28884c5d9e95b97274c4cae836ef322
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049977"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="d11f9-103">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d11f9-103">Get plannerTaskDetails</span></span>

<span data-ttu-id="d11f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d11f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d11f9-105">Получение свойств и связей объекта **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="d11f9-105">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d11f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d11f9-106">Permissions</span></span>
<span data-ttu-id="d11f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d11f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d11f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d11f9-109">Permission type</span></span>      | <span data-ttu-id="d11f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d11f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d11f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d11f9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d11f9-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d11f9-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d11f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d11f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d11f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11f9-114">Not supported.</span></span>    |
|<span data-ttu-id="d11f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d11f9-115">Application</span></span> | <span data-ttu-id="d11f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11f9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d11f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d11f9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="d11f9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d11f9-118">Request headers</span></span>
| <span data-ttu-id="d11f9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d11f9-119">Name</span></span>      |<span data-ttu-id="d11f9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d11f9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d11f9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d11f9-121">Authorization</span></span>  | <span data-ttu-id="d11f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d11f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d11f9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d11f9-124">Request body</span></span>
<span data-ttu-id="d11f9-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d11f9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d11f9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11f9-126">Response</span></span>

<span data-ttu-id="d11f9-127">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerTaskDetails](../resources/plannertaskdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d11f9-127">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="d11f9-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d11f9-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d11f9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d11f9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d11f9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d11f9-132">Request</span></span>
<span data-ttu-id="d11f9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d11f9-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d11f9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d11f9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
```
# <a name="c"></a>[<span data-ttu-id="d11f9-135">C#</span><span class="sxs-lookup"><span data-stu-id="d11f9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertaskdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d11f9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d11f9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d11f9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d11f9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertaskdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d11f9-138">Java</span><span class="sxs-lookup"><span data-stu-id="d11f9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannertaskdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d11f9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11f9-139">Response</span></span>
<span data-ttu-id="d11f9-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d11f9-140">Here is an example of the response.</span></span> <span data-ttu-id="d11f9-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d11f9-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


