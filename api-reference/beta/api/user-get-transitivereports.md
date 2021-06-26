---
title: Get transitiveReports для пользователя
description: Получите количество транзитных отчетов для пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a1ec6b231592ffec0d8847282b50e4ad227ecf06
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151787"
---
# <a name="get-transitivereports-for-a-user"></a><span data-ttu-id="b3a71-103">Get transitiveReports для пользователя</span><span class="sxs-lookup"><span data-stu-id="b3a71-103">Get transitiveReports for a user</span></span>

<span data-ttu-id="b3a71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3a71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3a71-105">Извлечение графа транзитных отчетов для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b3a71-105">Retrieve a count of transitive reports for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3a71-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3a71-106">Permissions</span></span>

<span data-ttu-id="b3a71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3a71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="b3a71-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3a71-109">Permission type</span></span> | <span data-ttu-id="b3a71-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3a71-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="b3a71-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3a71-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3a71-112">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3a71-112">User.Read, User.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="b3a71-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3a71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3a71-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3a71-114">Not supported.</span></span> |
| <span data-ttu-id="b3a71-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3a71-115">Application</span></span> | <span data-ttu-id="b3a71-116">User.Read, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3a71-116">User.Read, User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3a71-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3a71-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/transitiveReports/$count
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3a71-118">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b3a71-118">Optional query parameters</span></span>

<span data-ttu-id="b3a71-119">Этот метод поддерживает параметр запроса только для `$filter` **свойства accountEnabled.**</span><span class="sxs-lookup"><span data-stu-id="b3a71-119">This method supports the `$filter` query parameter for only the **accountEnabled** property.</span></span> <span data-ttu-id="b3a71-120">Дополнительные сведения об использовании параметров запроса см. в дополнительных сведениях о параметрах [запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="b3a71-120">For more information about using query parameters, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3a71-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3a71-121">Request headers</span></span>

| <span data-ttu-id="b3a71-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3a71-122">Header</span></span>       | <span data-ttu-id="b3a71-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b3a71-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3a71-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3a71-124">Authorization</span></span>  | <span data-ttu-id="b3a71-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3a71-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b3a71-127">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="b3a71-127">ConsistencyLevel</span></span> | <span data-ttu-id="b3a71-128">необязательный.</span><span class="sxs-lookup"><span data-stu-id="b3a71-128">eventual.</span></span> <span data-ttu-id="b3a71-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b3a71-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3a71-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3a71-130">Request body</span></span>

<span data-ttu-id="b3a71-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3a71-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3a71-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3a71-132">Response</span></span>

<span data-ttu-id="b3a71-133">В случае успешной работы этот метод возвращает код ответа и количество транзитных отчетов для пользователя `200 OK` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b3a71-133">If successful, this method returns a `200 OK` response code and a count of transitive reports for the user in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3a71-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3a71-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3a71-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3a71-135">Request</span></span>

<span data-ttu-id="b3a71-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3a71-136">The following is an example of the request.</span></span> <span data-ttu-id="b3a71-137">Требуется `$count` сегмент запроса.</span><span class="sxs-lookup"><span data-stu-id="b3a71-137">The `$count` query segment is required.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitivereports_user"
}-->
```http
GET https://graph.microsoft.com/beta/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```

### <a name="response"></a><span data-ttu-id="b3a71-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3a71-138">Response</span></span>

<span data-ttu-id="b3a71-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b3a71-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="b3a71-140">5 </span><span class="sxs-lookup"><span data-stu-id="b3a71-140">5</span></span>

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
