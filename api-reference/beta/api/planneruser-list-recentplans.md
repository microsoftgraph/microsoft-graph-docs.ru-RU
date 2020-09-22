---
title: Список объектов recentPlans
description: Получение списка объектов plannerPlan, недавно просмотренных пользователем. Вы можете обновить недавно просмотренные планы, обновив ресурс plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a1d005eb071eabab88d1e758997b284571025713
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017362"
---
# <a name="list-recentplans"></a><span data-ttu-id="16861-104">Список объектов recentPlans</span><span class="sxs-lookup"><span data-stu-id="16861-104">List recentPlans</span></span>

<span data-ttu-id="16861-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16861-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16861-106">Получение списка [планов](../resources/plannerplan.md) , недавно просмотренных пользователем.</span><span class="sxs-lookup"><span data-stu-id="16861-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="16861-107">Вы можете обновить недавно просмотренные планы, [обновив ресурс plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="16861-107">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="16861-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16861-108">Permissions</span></span>
<span data-ttu-id="16861-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16861-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16861-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16861-111">Permission type</span></span>      | <span data-ttu-id="16861-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16861-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16861-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16861-113">Delegated (work or school account)</span></span> | <span data-ttu-id="16861-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="16861-114">Group.Read.All</span></span>    |
|<span data-ttu-id="16861-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16861-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16861-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16861-116">Not supported.</span></span>    |
|<span data-ttu-id="16861-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16861-117">Application</span></span> | <span data-ttu-id="16861-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16861-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16861-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16861-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/{id}/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="16861-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16861-120">Request headers</span></span>
| <span data-ttu-id="16861-121">Имя</span><span class="sxs-lookup"><span data-stu-id="16861-121">Name</span></span>      |<span data-ttu-id="16861-122">Описание</span><span class="sxs-lookup"><span data-stu-id="16861-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16861-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16861-123">Authorization</span></span>  | <span data-ttu-id="16861-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="16861-124">Bearer {code}.</span></span> <span data-ttu-id="16861-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="16861-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16861-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16861-126">Request body</span></span>
<span data-ttu-id="16861-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16861-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="16861-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="16861-128">Response</span></span>
<span data-ttu-id="16861-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16861-129">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16861-130">Пример</span><span class="sxs-lookup"><span data-stu-id="16861-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16861-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="16861-131">Request</span></span>
<span data-ttu-id="16861-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16861-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16861-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="16861-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="c"></a>[<span data-ttu-id="16861-134">C#</span><span class="sxs-lookup"><span data-stu-id="16861-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16861-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16861-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16861-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16861-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16861-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="16861-137">Response</span></span>
<span data-ttu-id="16861-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16861-138">The following is an example of the response.</span></span> 

><span data-ttu-id="16861-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16861-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


