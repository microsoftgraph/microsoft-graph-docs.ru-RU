---
title: Список объектов recentPlans
description: Получение списка объектов plannerPlan, недавно просмотренных пользователем. Вы можете обновить недавно просмотримые планы, обновив ресурс plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 30409a99c089d490398b433b9bcd280240455ba8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049942"
---
# <a name="list-recentplans"></a><span data-ttu-id="4e460-104">Список объектов recentPlans</span><span class="sxs-lookup"><span data-stu-id="4e460-104">List recentPlans</span></span>

<span data-ttu-id="4e460-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e460-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e460-106">Извлечение списка [планировщикаPlans,](../resources/plannerplan.md) недавно просмотреного пользователем.</span><span class="sxs-lookup"><span data-stu-id="4e460-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="4e460-107">Вы можете обновить недавно просмотримые планы, [обновив ресурс plannerUser.](planneruser-update.md)</span><span class="sxs-lookup"><span data-stu-id="4e460-107">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4e460-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e460-108">Permissions</span></span>
<span data-ttu-id="4e460-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e460-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e460-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e460-111">Permission type</span></span>      | <span data-ttu-id="4e460-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e460-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e460-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e460-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4e460-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e460-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="4e460-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e460-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e460-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e460-116">Not supported.</span></span>    |
|<span data-ttu-id="4e460-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e460-117">Application</span></span> | <span data-ttu-id="4e460-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e460-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e460-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e460-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/{id}/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="4e460-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e460-120">Request headers</span></span>
| <span data-ttu-id="4e460-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4e460-121">Name</span></span>      |<span data-ttu-id="4e460-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4e460-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e460-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e460-123">Authorization</span></span>  | <span data-ttu-id="4e460-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="4e460-124">Bearer {code}.</span></span> <span data-ttu-id="4e460-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e460-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e460-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e460-126">Request body</span></span>
<span data-ttu-id="4e460-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e460-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4e460-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e460-128">Response</span></span>
<span data-ttu-id="4e460-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4e460-129">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e460-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4e460-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e460-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e460-131">Request</span></span>
<span data-ttu-id="4e460-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e460-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e460-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e460-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="c"></a>[<span data-ttu-id="4e460-134">C#</span><span class="sxs-lookup"><span data-stu-id="4e460-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e460-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e460-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e460-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e460-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e460-137">Java</span><span class="sxs-lookup"><span data-stu-id="4e460-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recentplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e460-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e460-138">Response</span></span>
<span data-ttu-id="4e460-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4e460-139">The following is an example of the response.</span></span> 

><span data-ttu-id="4e460-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4e460-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


