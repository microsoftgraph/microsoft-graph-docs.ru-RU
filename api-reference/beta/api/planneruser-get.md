---
title: Получение объекта plannerUser
description: 'Получение свойств и связей объекта plannerUser. Возвращенные свойства включают любимые планы пользователя и недавно просматриваемые планы. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 05e192b4b57f06b84eca8325ae08960bb74839af
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473338"
---
# <a name="get-planneruser"></a><span data-ttu-id="d12cc-104">Получение объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="d12cc-104">Get plannerUser</span></span>

<span data-ttu-id="d12cc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d12cc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d12cc-106">Извлечение свойств и связей объекта [plannerUser.](../resources/planneruser.md)</span><span class="sxs-lookup"><span data-stu-id="d12cc-106">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="d12cc-107">Возвращенные свойства включают любимые планы пользователя и недавно просматриваемые планы.</span><span class="sxs-lookup"><span data-stu-id="d12cc-107">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="d12cc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d12cc-108">Permissions</span></span>
<span data-ttu-id="d12cc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d12cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d12cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d12cc-111">Permission type</span></span>      | <span data-ttu-id="d12cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d12cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d12cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d12cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d12cc-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d12cc-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="d12cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d12cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d12cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d12cc-116">Not supported.</span></span>    |
|<span data-ttu-id="d12cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d12cc-117">Application</span></span> | <span data-ttu-id="d12cc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d12cc-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d12cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d12cc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/{id}/planner
```

## <a name="request-headers"></a><span data-ttu-id="d12cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d12cc-120">Request headers</span></span>
| <span data-ttu-id="d12cc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d12cc-121">Name</span></span>      |<span data-ttu-id="d12cc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d12cc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d12cc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d12cc-123">Authorization</span></span>  | <span data-ttu-id="d12cc-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="d12cc-124">Bearer {code}.</span></span> <span data-ttu-id="d12cc-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d12cc-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d12cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d12cc-126">Request body</span></span>
<span data-ttu-id="d12cc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d12cc-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d12cc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d12cc-128">Response</span></span>
<span data-ttu-id="d12cc-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [plannerUser](../resources/planneruser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d12cc-129">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d12cc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d12cc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d12cc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d12cc-131">Request</span></span>
<span data-ttu-id="d12cc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d12cc-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d12cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d12cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_planneruser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner
```
# <a name="c"></a>[<span data-ttu-id="d12cc-134">C#</span><span class="sxs-lookup"><span data-stu-id="d12cc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-planneruser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d12cc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d12cc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-planneruser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d12cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d12cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-planneruser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d12cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="d12cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-planneruser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d12cc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d12cc-138">Response</span></span>
<span data-ttu-id="d12cc-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d12cc-139">The following is an example of the response.</span></span> 

><span data-ttu-id="d12cc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d12cc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


