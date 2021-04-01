---
title: Список объектов favoritePlans
description: Получение списка объектов plannerPlan, отмеченных пользователем как избранные. Вы можете отметить план как любимый, обновив ресурс plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1650ea55e1fc7dc6200e4985e417fdfb67fb0ee3
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473488"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="c2aaf-104">Список объектов favoritePlans</span><span class="sxs-lookup"><span data-stu-id="c2aaf-104">List favoritePlans</span></span>

<span data-ttu-id="c2aaf-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2aaf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2aaf-106">Извлечение списка [plannerPlans,](../resources/plannerplan.md) помеченных пользователем как любимые.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="c2aaf-107">Вы можете отметить план как любимый, [обновив ресурс plannerUser.](planneruser-update.md)</span><span class="sxs-lookup"><span data-stu-id="c2aaf-107">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2aaf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2aaf-108">Permissions</span></span>
<span data-ttu-id="c2aaf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2aaf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2aaf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2aaf-111">Permission type</span></span>      | <span data-ttu-id="c2aaf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2aaf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2aaf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2aaf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c2aaf-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2aaf-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="c2aaf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2aaf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2aaf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-116">Not supported.</span></span>    |
|<span data-ttu-id="c2aaf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2aaf-117">Application</span></span> | <span data-ttu-id="c2aaf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2aaf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2aaf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/{id}/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2aaf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2aaf-120">Optional query parameters</span></span>
<span data-ttu-id="c2aaf-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2aaf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2aaf-122">Request headers</span></span>
| <span data-ttu-id="c2aaf-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c2aaf-123">Name</span></span>      |<span data-ttu-id="c2aaf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c2aaf-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2aaf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2aaf-125">Authorization</span></span>  | <span data-ttu-id="c2aaf-126">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-126">Bearer {code}.</span></span> <span data-ttu-id="c2aaf-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2aaf-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2aaf-128">Request body</span></span>
<span data-ttu-id="c2aaf-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c2aaf-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2aaf-130">Response</span></span>
<span data-ttu-id="c2aaf-131">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2aaf-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c2aaf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2aaf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2aaf-133">Request</span></span>
<span data-ttu-id="c2aaf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2aaf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2aaf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
# <a name="c"></a>[<span data-ttu-id="c2aaf-136">C#</span><span class="sxs-lookup"><span data-stu-id="c2aaf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-favoriteplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2aaf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2aaf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-favoriteplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2aaf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2aaf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-favoriteplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2aaf-139">Java</span><span class="sxs-lookup"><span data-stu-id="c2aaf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-favoriteplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2aaf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2aaf-140">Response</span></span>
<span data-ttu-id="c2aaf-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-141">The following is an example of the response.</span></span> 

><span data-ttu-id="c2aaf-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2aaf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
