---
title: Список владельцев
description: 'Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2294378620f6d02da7cb98be657fb587a8a7b46b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335413"
---
# <a name="list-owners"></a><span data-ttu-id="c6f4e-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="c6f4e-104">List owners</span></span>

<span data-ttu-id="c6f4e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6f4e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6f4e-p102">Получение списка владельцев группы. Владельцы являются набором пользователей, не являющихся администраторами, или субъектов служб, которым разрешено изменять объект Group.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users or service principals who are allowed to modify the group object.</span></span> 

><span data-ttu-id="c6f4e-108">**Примечание:** В настоящее время субъекты-службы не указаны как владельцы групп из-за поэтапного развертывания субъектов-служб в конечной точке Microsoft Graph 1.0.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-108">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6f4e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6f4e-109">Permissions</span></span>
<span data-ttu-id="c6f4e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6f4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f4e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6f4e-112">Permission type</span></span>      | <span data-ttu-id="c6f4e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6f4e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6f4e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6f4e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c6f4e-115">Group. Read. ALL и User. ReadBasic. ALL, Group. Read. ALL и User. Read. ALL, Group. Read. ALL и User. ReadWrite. ALL, Group. Read. ALL и User. Read. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c6f4e-115">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="c6f4e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6f4e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6f4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-117">Not supported.</span></span>    |
|<span data-ttu-id="c6f4e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6f4e-118">Application</span></span> | <span data-ttu-id="c6f4e-119">Group. Read. ALL и User. Read. ALL, Group. Read. ALL и User. ReadWrite. ALL, Group. Read. ALL и User. Read. ALL и Application. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-119">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c6f4e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6f4e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6f4e-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c6f4e-121">Optional query parameters</span></span>
<span data-ttu-id="c6f4e-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6f4e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6f4e-123">Request headers</span></span>
| <span data-ttu-id="c6f4e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c6f4e-124">Name</span></span>       | <span data-ttu-id="c6f4e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c6f4e-125">Type</span></span> | <span data-ttu-id="c6f4e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c6f4e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c6f4e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6f4e-127">Authorization</span></span>  | <span data-ttu-id="c6f4e-128">string</span><span class="sxs-lookup"><span data-stu-id="c6f4e-128">string</span></span>  | <span data-ttu-id="c6f4e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6f4e-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6f4e-131">Request body</span></span>
<span data-ttu-id="c6f4e-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6f4e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6f4e-133">Response</span></span>
<span data-ttu-id="c6f4e-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6f4e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c6f4e-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c6f4e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6f4e-136">Request</span></span>
<span data-ttu-id="c6f4e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6f4e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6f4e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="c6f4e-139">C#</span><span class="sxs-lookup"><span data-stu-id="c6f4e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6f4e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6f4e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6f4e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6f4e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6f4e-142">Java</span><span class="sxs-lookup"><span data-stu-id="c6f4e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c6f4e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6f4e-143">Response</span></span>
<span data-ttu-id="c6f4e-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-144">The following is an example of the response.</span></span>
><span data-ttu-id="c6f4e-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c6f4e-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6f4e-146">All the properties will be returned from an actual call.</span></span>
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
