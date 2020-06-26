---
title: Список транзитивных групп memberOf
description: Получение групп, членом которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от того, что получает группы Microsoft 365 пользователя, возвращаются все типы групп, а не только группы Майкрософт 365.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ba428fb4f0eb78171ac8f29e659047065148f592
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897857"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="569ea-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="569ea-105">List group transitive memberOf</span></span>

<span data-ttu-id="569ea-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="569ea-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="569ea-107">Получение групп, членом которых является группа.</span><span class="sxs-lookup"><span data-stu-id="569ea-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="569ea-108">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="569ea-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="569ea-109">В отличие от того, что получает группы Microsoft 365 пользователя, возвращаются все типы групп, а не только группы Майкрософт 365.</span><span class="sxs-lookup"><span data-stu-id="569ea-109">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="569ea-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="569ea-110">Permissions</span></span>

<span data-ttu-id="569ea-111">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="569ea-111">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="569ea-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="569ea-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="569ea-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="569ea-113">Permission type</span></span>      | <span data-ttu-id="569ea-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="569ea-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="569ea-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="569ea-115">Delegated (work or school account)</span></span> | <span data-ttu-id="569ea-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="569ea-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="569ea-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="569ea-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="569ea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="569ea-118">Not supported.</span></span>    |
|<span data-ttu-id="569ea-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="569ea-119">Application</span></span> | <span data-ttu-id="569ea-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569ea-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="569ea-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="569ea-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="569ea-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="569ea-122">Optional query parameters</span></span>
<span data-ttu-id="569ea-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="569ea-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="569ea-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="569ea-124">Request headers</span></span>
| <span data-ttu-id="569ea-125">Имя</span><span class="sxs-lookup"><span data-stu-id="569ea-125">Name</span></span>       | <span data-ttu-id="569ea-126">Тип</span><span class="sxs-lookup"><span data-stu-id="569ea-126">Type</span></span> | <span data-ttu-id="569ea-127">Описание</span><span class="sxs-lookup"><span data-stu-id="569ea-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="569ea-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="569ea-128">Authorization</span></span>  | <span data-ttu-id="569ea-129">string</span><span class="sxs-lookup"><span data-stu-id="569ea-129">string</span></span>  | <span data-ttu-id="569ea-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="569ea-130">Bearer {token}.</span></span> <span data-ttu-id="569ea-131">Required.</span><span class="sxs-lookup"><span data-stu-id="569ea-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="569ea-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="569ea-132">Request body</span></span>
<span data-ttu-id="569ea-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="569ea-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="569ea-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="569ea-134">Response</span></span>
<span data-ttu-id="569ea-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="569ea-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="569ea-136">Пример</span><span class="sxs-lookup"><span data-stu-id="569ea-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="569ea-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="569ea-137">Request</span></span>
<span data-ttu-id="569ea-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="569ea-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="569ea-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="569ea-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="569ea-140">C#</span><span class="sxs-lookup"><span data-stu-id="569ea-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="569ea-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="569ea-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="569ea-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="569ea-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="569ea-143">Java</span><span class="sxs-lookup"><span data-stu-id="569ea-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="569ea-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="569ea-144">Response</span></span>

<span data-ttu-id="569ea-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="569ea-145">The following is an example of the response.</span></span>
><span data-ttu-id="569ea-146">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="569ea-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="569ea-147">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="569ea-147">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
