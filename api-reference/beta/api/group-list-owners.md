---
title: Список владельцев
description: Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 4db7b27899879d6564670725fb205f4b47fa6d33
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263044"
---
# <a name="list-owners"></a><span data-ttu-id="20669-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="20669-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20669-p102">Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="20669-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20669-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20669-107">Permissions</span></span>
<span data-ttu-id="20669-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20669-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20669-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20669-110">Permission type</span></span>      | <span data-ttu-id="20669-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20669-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20669-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20669-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20669-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20669-113">Not supported.</span></span>    |
|<span data-ttu-id="20669-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20669-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20669-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20669-115">Not supported.</span></span>    |
|<span data-ttu-id="20669-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20669-116">Application</span></span> | <span data-ttu-id="20669-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20669-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20669-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20669-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20669-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20669-119">Optional query parameters</span></span>
<span data-ttu-id="20669-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="20669-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20669-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20669-121">Request headers</span></span>
| <span data-ttu-id="20669-122">Имя</span><span class="sxs-lookup"><span data-stu-id="20669-122">Name</span></span>       | <span data-ttu-id="20669-123">Тип</span><span class="sxs-lookup"><span data-stu-id="20669-123">Type</span></span> | <span data-ttu-id="20669-124">Описание</span><span class="sxs-lookup"><span data-stu-id="20669-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20669-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="20669-125">Authorization</span></span>  | <span data-ttu-id="20669-126">string</span><span class="sxs-lookup"><span data-stu-id="20669-126">string</span></span>  | <span data-ttu-id="20669-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20669-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20669-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20669-129">Request body</span></span>
<span data-ttu-id="20669-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20669-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20669-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="20669-131">Response</span></span>
<span data-ttu-id="20669-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20669-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20669-133">Пример</span><span class="sxs-lookup"><span data-stu-id="20669-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="20669-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="20669-134">Request</span></span>
<span data-ttu-id="20669-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20669-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="20669-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="20669-136">Response</span></span>
<span data-ttu-id="20669-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20669-137">The following is an example of the response.</span></span>
><span data-ttu-id="20669-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="20669-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="20669-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20669-139">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="20669-140">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="20669-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="20669-141">C#</span><span class="sxs-lookup"><span data-stu-id="20669-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20669-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="20669-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="20669-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="20669-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_owners-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
