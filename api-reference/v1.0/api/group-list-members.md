---
title: Список участников
description: Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты и другие группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6c79b4bd4ee3059e693e63817420e1c5d0b8d612
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279326"
---
# <a name="list-members"></a><span data-ttu-id="4212b-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="4212b-104">List members</span></span>
<span data-ttu-id="4212b-p102">Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты и другие группы. Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="4212b-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4212b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4212b-108">Permissions</span></span>
<span data-ttu-id="4212b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4212b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4212b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4212b-111">Permission type</span></span>      | <span data-ttu-id="4212b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4212b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4212b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4212b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4212b-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4212b-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="4212b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4212b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4212b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4212b-116">Not supported.</span></span>    |
|<span data-ttu-id="4212b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4212b-117">Application</span></span> | <span data-ttu-id="4212b-118">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4212b-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4212b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4212b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4212b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4212b-120">Optional query parameters</span></span>
<span data-ttu-id="4212b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4212b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4212b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4212b-122">Request headers</span></span>
| <span data-ttu-id="4212b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4212b-123">Name</span></span>       | <span data-ttu-id="4212b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="4212b-124">Type</span></span> | <span data-ttu-id="4212b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4212b-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4212b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4212b-126">Authorization</span></span>  | <span data-ttu-id="4212b-127">string</span><span class="sxs-lookup"><span data-stu-id="4212b-127">string</span></span>  | <span data-ttu-id="4212b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4212b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4212b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4212b-130">Request body</span></span>
<span data-ttu-id="4212b-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4212b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4212b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4212b-132">Response</span></span>
<span data-ttu-id="4212b-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4212b-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4212b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4212b-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4212b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4212b-135">Request</span></span>
<span data-ttu-id="4212b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4212b-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="4212b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4212b-137">Response</span></span>
<span data-ttu-id="4212b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4212b-138">The following is an example of the response.</span></span>
><span data-ttu-id="4212b-139">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4212b-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4212b-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4212b-140">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4212b-141">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="4212b-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4212b-142">C#</span><span class="sxs-lookup"><span data-stu-id="4212b-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4212b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4212b-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4212b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4212b-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
