---
title: Список владельцев
description: 'Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы. '
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6a8da4193aa4e5d5fcbcb773082e4d123f0ba547
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864749"
---
# <a name="list-owners"></a><span data-ttu-id="07d66-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="07d66-104">List owners</span></span>
<span data-ttu-id="07d66-p102">Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="07d66-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="07d66-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07d66-107">Permissions</span></span>
<span data-ttu-id="07d66-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d66-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d66-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07d66-110">Permission type</span></span>      | <span data-ttu-id="07d66-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07d66-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d66-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07d66-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07d66-113">Group.Read.All и User.ReadBasic.All, Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d66-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="07d66-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07d66-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d66-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d66-115">Not supported.</span></span>    |
|<span data-ttu-id="07d66-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07d66-116">Application</span></span> | <span data-ttu-id="07d66-117">Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d66-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="07d66-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07d66-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07d66-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07d66-119">Optional query parameters</span></span>
<span data-ttu-id="07d66-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07d66-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07d66-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07d66-121">Request headers</span></span>
| <span data-ttu-id="07d66-122">Имя</span><span class="sxs-lookup"><span data-stu-id="07d66-122">Name</span></span>       | <span data-ttu-id="07d66-123">Тип</span><span class="sxs-lookup"><span data-stu-id="07d66-123">Type</span></span> | <span data-ttu-id="07d66-124">Описание</span><span class="sxs-lookup"><span data-stu-id="07d66-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07d66-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07d66-125">Authorization</span></span>  | <span data-ttu-id="07d66-126">string</span><span class="sxs-lookup"><span data-stu-id="07d66-126">string</span></span>  | <span data-ttu-id="07d66-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07d66-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07d66-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07d66-129">Request body</span></span>
<span data-ttu-id="07d66-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07d66-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07d66-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d66-131">Response</span></span>
<span data-ttu-id="07d66-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07d66-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07d66-133">Пример</span><span class="sxs-lookup"><span data-stu-id="07d66-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="07d66-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d66-134">Request</span></span>
<span data-ttu-id="07d66-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d66-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="07d66-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="07d66-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="07d66-137">C#</span><span class="sxs-lookup"><span data-stu-id="07d66-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07d66-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07d66-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="07d66-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07d66-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="07d66-140">Java</span><span class="sxs-lookup"><span data-stu-id="07d66-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="07d66-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d66-141">Response</span></span>
<span data-ttu-id="07d66-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07d66-142">The following is an example of the response.</span></span>
><span data-ttu-id="07d66-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="07d66-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07d66-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07d66-144">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
