---
title: Список Рецентпланс
description: Получение списка планов, недавно просмотренных пользователем. Вы можете обновить недавно просмотренные планы, обновив ресурс plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 72a91a1511f1d4be70de4cd95494bee74b319f54
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412987"
---
# <a name="list-recentplans"></a><span data-ttu-id="40efb-104">Список Рецентпланс</span><span class="sxs-lookup"><span data-stu-id="40efb-104">List recentPlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40efb-105">Получение списка [планов](../resources/plannerplan.md) , недавно просмотренных пользователем.</span><span class="sxs-lookup"><span data-stu-id="40efb-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="40efb-106">Вы можете обновить недавно просмотренные планы, [обновив ресурс plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="40efb-106">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="40efb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40efb-107">Permissions</span></span>
<span data-ttu-id="40efb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40efb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40efb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40efb-110">Permission type</span></span>      | <span data-ttu-id="40efb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40efb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40efb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40efb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40efb-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="40efb-113">Group.Read.All</span></span>    |
|<span data-ttu-id="40efb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40efb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40efb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40efb-115">Not supported.</span></span>    |
|<span data-ttu-id="40efb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40efb-116">Application</span></span> | <span data-ttu-id="40efb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40efb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40efb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40efb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/{id}/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="40efb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40efb-119">Request headers</span></span>
| <span data-ttu-id="40efb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="40efb-120">Name</span></span>      |<span data-ttu-id="40efb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="40efb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40efb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40efb-122">Authorization</span></span>  | <span data-ttu-id="40efb-123">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="40efb-123">Bearer {code}.</span></span> <span data-ttu-id="40efb-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="40efb-124">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40efb-125">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="40efb-125">Request body</span></span>
<span data-ttu-id="40efb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40efb-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="40efb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="40efb-127">Response</span></span>
<span data-ttu-id="40efb-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40efb-128">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40efb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="40efb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40efb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="40efb-130">Request</span></span>
<span data-ttu-id="40efb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40efb-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40efb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="40efb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="40efb-133">C#</span><span class="sxs-lookup"><span data-stu-id="40efb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40efb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40efb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40efb-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="40efb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="40efb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="40efb-136">Response</span></span>
<span data-ttu-id="40efb-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40efb-137">The following is an example of the response.</span></span> 

><span data-ttu-id="40efb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40efb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
