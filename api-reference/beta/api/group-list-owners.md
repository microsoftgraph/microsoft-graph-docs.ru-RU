---
title: Список владельцев
description: Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e131a95caa4a06bc6f3b5c5d95921a468822a372
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440416"
---
# <a name="list-owners"></a><span data-ttu-id="d6d3f-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="d6d3f-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6d3f-p102">Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6d3f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6d3f-107">Permissions</span></span>
<span data-ttu-id="d6d3f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6d3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6d3f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6d3f-110">Permission type</span></span>      | <span data-ttu-id="d6d3f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6d3f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6d3f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6d3f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d6d3f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-113">Not supported.</span></span>    |
|<span data-ttu-id="d6d3f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6d3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6d3f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-115">Not supported.</span></span>    |
|<span data-ttu-id="d6d3f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6d3f-116">Application</span></span> | <span data-ttu-id="d6d3f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6d3f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6d3f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6d3f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6d3f-119">Optional query parameters</span></span>
<span data-ttu-id="d6d3f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6d3f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6d3f-121">Request headers</span></span>
| <span data-ttu-id="d6d3f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d6d3f-122">Name</span></span>       | <span data-ttu-id="d6d3f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d6d3f-123">Type</span></span> | <span data-ttu-id="d6d3f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d6d3f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d6d3f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6d3f-125">Authorization</span></span>  | <span data-ttu-id="d6d3f-126">string</span><span class="sxs-lookup"><span data-stu-id="d6d3f-126">string</span></span>  | <span data-ttu-id="d6d3f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6d3f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6d3f-129">Request body</span></span>
<span data-ttu-id="d6d3f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6d3f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6d3f-131">Response</span></span>
<span data-ttu-id="d6d3f-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d3f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d6d3f-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d6d3f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6d3f-134">Request</span></span>
<span data-ttu-id="d6d3f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6d3f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6d3f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6d3f-137">C#</span><span class="sxs-lookup"><span data-stu-id="d6d3f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6d3f-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6d3f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6d3f-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d6d3f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d6d3f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6d3f-140">Response</span></span>
<span data-ttu-id="d6d3f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-141">The following is an example of the response.</span></span>
><span data-ttu-id="d6d3f-142">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d6d3f-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6d3f-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
