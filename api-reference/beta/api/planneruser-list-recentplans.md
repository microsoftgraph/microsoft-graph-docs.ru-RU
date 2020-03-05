---
title: Список объектов recentPlans
description: Получение списка объектов plannerPlan, недавно просмотренных пользователем. Вы можете обновить недавно просмотренные планы, обновив ресурс plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: af0492c5f99545bbe823dafc301826d6ba9a3234
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455566"
---
# <a name="list-recentplans"></a><span data-ttu-id="a7b0c-104">Список объектов recentPlans</span><span class="sxs-lookup"><span data-stu-id="a7b0c-104">List recentPlans</span></span>

<span data-ttu-id="a7b0c-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a7b0c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7b0c-106">Получение списка [планов](../resources/plannerplan.md) , недавно просмотренных пользователем.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="a7b0c-107">Вы можете обновить недавно просмотренные планы, [обновив ресурс plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="a7b0c-107">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a7b0c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7b0c-108">Permissions</span></span>
<span data-ttu-id="a7b0c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7b0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7b0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7b0c-111">Permission type</span></span>      | <span data-ttu-id="a7b0c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7b0c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7b0c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7b0c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a7b0c-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7b0c-114">Group.Read.All</span></span>    |
|<span data-ttu-id="a7b0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7b0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7b0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-116">Not supported.</span></span>    |
|<span data-ttu-id="a7b0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7b0c-117">Application</span></span> | <span data-ttu-id="a7b0c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7b0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7b0c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/{id}/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="a7b0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7b0c-120">Request headers</span></span>
| <span data-ttu-id="a7b0c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a7b0c-121">Name</span></span>      |<span data-ttu-id="a7b0c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a7b0c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a7b0c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7b0c-123">Authorization</span></span>  | <span data-ttu-id="a7b0c-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-124">Bearer {code}.</span></span> <span data-ttu-id="a7b0c-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7b0c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7b0c-126">Request body</span></span>
<span data-ttu-id="a7b0c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a7b0c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7b0c-128">Response</span></span>
<span data-ttu-id="a7b0c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-129">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7b0c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a7b0c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7b0c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7b0c-131">Request</span></span>
<span data-ttu-id="a7b0c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7b0c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7b0c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="c"></a>[<span data-ttu-id="a7b0c-134">C#</span><span class="sxs-lookup"><span data-stu-id="a7b0c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7b0c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7b0c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7b0c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7b0c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7b0c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7b0c-137">Response</span></span>
<span data-ttu-id="a7b0c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-138">The following is an example of the response.</span></span> 

><span data-ttu-id="a7b0c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7b0c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
