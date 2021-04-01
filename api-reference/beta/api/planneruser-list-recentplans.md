---
title: Список объектов recentPlans
description: Получение списка объектов plannerPlan, недавно просмотренных пользователем. Вы можете обновить недавно просмотримые планы, обновив ресурс plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: abe618b63bdd15e3053c831352490255468bb0f2
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473474"
---
# <a name="list-recentplans"></a><span data-ttu-id="41abb-104">Список объектов recentPlans</span><span class="sxs-lookup"><span data-stu-id="41abb-104">List recentPlans</span></span>

<span data-ttu-id="41abb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41abb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41abb-106">Извлечение списка [планировщикаPlans,](../resources/plannerplan.md) недавно просмотреного пользователем.</span><span class="sxs-lookup"><span data-stu-id="41abb-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="41abb-107">Вы можете обновить недавно просмотримые планы, [обновив ресурс plannerUser.](planneruser-update.md)</span><span class="sxs-lookup"><span data-stu-id="41abb-107">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="41abb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41abb-108">Permissions</span></span>
<span data-ttu-id="41abb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41abb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41abb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41abb-111">Permission type</span></span>      | <span data-ttu-id="41abb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41abb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41abb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41abb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="41abb-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="41abb-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="41abb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41abb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41abb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41abb-116">Not supported.</span></span>    |
|<span data-ttu-id="41abb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41abb-117">Application</span></span> | <span data-ttu-id="41abb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41abb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41abb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41abb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/{id}/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="41abb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41abb-120">Request headers</span></span>
| <span data-ttu-id="41abb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="41abb-121">Name</span></span>      |<span data-ttu-id="41abb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="41abb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41abb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41abb-123">Authorization</span></span>  | <span data-ttu-id="41abb-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="41abb-124">Bearer {code}.</span></span> <span data-ttu-id="41abb-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="41abb-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41abb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41abb-126">Request body</span></span>
<span data-ttu-id="41abb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41abb-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="41abb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="41abb-128">Response</span></span>
<span data-ttu-id="41abb-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="41abb-129">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41abb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="41abb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41abb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="41abb-131">Request</span></span>
<span data-ttu-id="41abb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41abb-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41abb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="41abb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="c"></a>[<span data-ttu-id="41abb-134">C#</span><span class="sxs-lookup"><span data-stu-id="41abb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41abb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41abb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41abb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41abb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41abb-137">Java</span><span class="sxs-lookup"><span data-stu-id="41abb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recentplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="41abb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="41abb-138">Response</span></span>
<span data-ttu-id="41abb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="41abb-139">The following is an example of the response.</span></span> 

><span data-ttu-id="41abb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41abb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


