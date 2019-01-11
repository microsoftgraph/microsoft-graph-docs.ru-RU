---
title: Получение объекта plannerTask
description: Получение свойств и связей объекта **plannertask**.
localization_priority: Normal
ms.openlocfilehash: be6ca0f71aaaa446424c4bf34ff6a0851c4cd266
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833665"
---
# <a name="get-plannertask"></a><span data-ttu-id="4c755-103">Получение объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="4c755-103">Get plannerTask</span></span>

<span data-ttu-id="4c755-104">Получение свойств и связей объекта **plannertask**.</span><span class="sxs-lookup"><span data-stu-id="4c755-104">Retrieve the properties and relationships of **plannertask** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c755-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c755-105">Permissions</span></span>
<span data-ttu-id="4c755-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c755-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c755-108">Permission type</span></span>      | <span data-ttu-id="4c755-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c755-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c755-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c755-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c755-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c755-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c755-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c755-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c755-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c755-113">Not supported.</span></span>    |
|<span data-ttu-id="4c755-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c755-114">Application</span></span> | <span data-ttu-id="4c755-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c755-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c755-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c755-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4c755-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c755-117">Request headers</span></span>
| <span data-ttu-id="4c755-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4c755-118">Name</span></span>      |<span data-ttu-id="4c755-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4c755-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c755-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c755-120">Authorization</span></span>  | <span data-ttu-id="4c755-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c755-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c755-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c755-123">Request body</span></span>
<span data-ttu-id="4c755-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c755-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c755-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c755-125">Response</span></span>

<span data-ttu-id="4c755-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4c755-126">If successful, this method returns a `200 OK` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="4c755-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="4c755-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4c755-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4c755-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c755-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c755-131">Request</span></span>
<span data-ttu-id="4c755-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c755-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}
```
##### <a name="response"></a><span data-ttu-id="4c755-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c755-133">Response</span></span>
<span data-ttu-id="4c755-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c755-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 707

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
      "@odata.type": "#microsoft.graph.plannerAssignment",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
