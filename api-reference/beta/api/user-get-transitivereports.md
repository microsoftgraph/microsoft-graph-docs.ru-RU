---
title: Get transitiveReports для пользователя
description: Получите количество транзитных отчетов для пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5d04b1240c54b186a2e5f5cfb77f651e032f1eda
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316610"
---
# <a name="get-transitivereports-for-a-user"></a><span data-ttu-id="810fb-103">Get transitiveReports для пользователя</span><span class="sxs-lookup"><span data-stu-id="810fb-103">Get transitiveReports for a user</span></span>

<span data-ttu-id="810fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="810fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="810fb-105">Извлечение графа транзитных отчетов для пользователя.</span><span class="sxs-lookup"><span data-stu-id="810fb-105">Retrieve a count of transitive reports for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="810fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="810fb-106">Permissions</span></span>

<span data-ttu-id="810fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="810fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="810fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="810fb-109">Permission type</span></span> | <span data-ttu-id="810fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="810fb-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="810fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="810fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="810fb-112">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="810fb-112">User.Read, User.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="810fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="810fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="810fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="810fb-114">Not supported.</span></span> |
| <span data-ttu-id="810fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="810fb-115">Application</span></span> | <span data-ttu-id="810fb-116">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="810fb-116">User.Read, User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="810fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="810fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/transitiveReports/$count
```
## <a name="optional-query-parameters"></a><span data-ttu-id="810fb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="810fb-118">Optional query parameters</span></span>

<span data-ttu-id="810fb-119">Этот метод поддерживает параметр запроса только для `$filter` **свойства accountEnabled.**</span><span class="sxs-lookup"><span data-stu-id="810fb-119">This method supports the `$filter` query parameter for only the **accountEnabled** property.</span></span> <span data-ttu-id="810fb-120">Дополнительные сведения об использовании параметров запроса см. в дополнительных сведениях о параметрах [запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="810fb-120">For more information about using query parameters, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="810fb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="810fb-121">Request headers</span></span>

| <span data-ttu-id="810fb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="810fb-122">Header</span></span>       | <span data-ttu-id="810fb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="810fb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="810fb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="810fb-124">Authorization</span></span>  | <span data-ttu-id="810fb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="810fb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="810fb-127">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="810fb-127">ConsistencyLevel</span></span> | <span data-ttu-id="810fb-128">необязательный.</span><span class="sxs-lookup"><span data-stu-id="810fb-128">eventual.</span></span> <span data-ttu-id="810fb-129">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="810fb-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="810fb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="810fb-130">Request body</span></span>

<span data-ttu-id="810fb-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="810fb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="810fb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="810fb-132">Response</span></span>

<span data-ttu-id="810fb-133">В случае успешной работы этот метод возвращает код ответа и количество транзитных отчетов для пользователя `200 OK` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="810fb-133">If successful, this method returns a `200 OK` response code and a count of transitive reports for the user in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="810fb-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="810fb-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="810fb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="810fb-135">Request</span></span>

<span data-ttu-id="810fb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="810fb-136">The following is an example of the request.</span></span> <span data-ttu-id="810fb-137">Требуется `$count` сегмент запроса.</span><span class="sxs-lookup"><span data-stu-id="810fb-137">The `$count` query segment is required.</span></span>


# <a name="http"></a>[<span data-ttu-id="810fb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="810fb-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivereports_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```
# <a name="c"></a>[<span data-ttu-id="810fb-139">C#</span><span class="sxs-lookup"><span data-stu-id="810fb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivereports-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="810fb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="810fb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivereports-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="810fb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="810fb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivereports-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="810fb-142">Java</span><span class="sxs-lookup"><span data-stu-id="810fb-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivereports-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="810fb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="810fb-143">Response</span></span>

<span data-ttu-id="810fb-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="810fb-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="810fb-145">5 </span><span class="sxs-lookup"><span data-stu-id="810fb-145">5</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get transitiveReports for a user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
