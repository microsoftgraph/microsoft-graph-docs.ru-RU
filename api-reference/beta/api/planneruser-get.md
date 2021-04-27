---
title: Получение объекта plannerUser
description: 'Получение свойств и связей объекта plannerUser. Возвращенные свойства включают любимые планы пользователя и недавно просматриваемые планы. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: bc1d212f9f9e75770e66067bc3cf22438fa71988
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049963"
---
# <a name="get-planneruser"></a><span data-ttu-id="a2022-104">Получение объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="a2022-104">Get plannerUser</span></span>

<span data-ttu-id="a2022-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2022-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2022-106">Извлечение свойств и связей объекта [plannerUser.](../resources/planneruser.md)</span><span class="sxs-lookup"><span data-stu-id="a2022-106">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="a2022-107">Возвращенные свойства включают любимые планы пользователя и недавно просматриваемые планы.</span><span class="sxs-lookup"><span data-stu-id="a2022-107">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="a2022-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2022-108">Permissions</span></span>
<span data-ttu-id="a2022-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2022-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2022-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2022-111">Permission type</span></span>      | <span data-ttu-id="a2022-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2022-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2022-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2022-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a2022-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2022-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="a2022-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2022-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2022-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2022-116">Not supported.</span></span>    |
|<span data-ttu-id="a2022-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2022-117">Application</span></span> | <span data-ttu-id="a2022-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2022-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2022-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2022-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/{id}/planner
```

## <a name="request-headers"></a><span data-ttu-id="a2022-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2022-120">Request headers</span></span>
| <span data-ttu-id="a2022-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a2022-121">Name</span></span>      |<span data-ttu-id="a2022-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a2022-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2022-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2022-123">Authorization</span></span>  | <span data-ttu-id="a2022-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="a2022-124">Bearer {code}.</span></span> <span data-ttu-id="a2022-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a2022-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2022-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2022-126">Request body</span></span>
<span data-ttu-id="a2022-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2022-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a2022-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2022-128">Response</span></span>
<span data-ttu-id="a2022-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [plannerUser](../resources/planneruser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a2022-129">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2022-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a2022-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2022-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2022-131">Request</span></span>
<span data-ttu-id="a2022-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2022-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2022-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2022-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_planneruser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner
```
# <a name="c"></a>[<span data-ttu-id="a2022-134">C#</span><span class="sxs-lookup"><span data-stu-id="a2022-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-planneruser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2022-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2022-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-planneruser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2022-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2022-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-planneruser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2022-137">Java</span><span class="sxs-lookup"><span data-stu-id="a2022-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-planneruser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a2022-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2022-138">Response</span></span>
<span data-ttu-id="a2022-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a2022-139">The following is an example of the response.</span></span> 

><span data-ttu-id="a2022-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a2022-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


