---
title: Список memberOf
description: 'Получение групп, непосредственным членом которых является данная группа. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0907ea075077fa11df9503b484185fffdbec8954
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720825"
---
# <a name="list-memberof"></a><span data-ttu-id="086db-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="086db-103">List memberOf</span></span>
<span data-ttu-id="086db-104">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="086db-104">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="086db-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Office 365", эта операция возвращает группы всех типов, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="086db-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="086db-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="086db-107">Permissions</span></span>
<span data-ttu-id="086db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="086db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="086db-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="086db-110">Permission type</span></span>      | <span data-ttu-id="086db-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="086db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="086db-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="086db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="086db-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="086db-113">Group.Read.All</span></span>    |
|<span data-ttu-id="086db-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="086db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="086db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="086db-115">Not supported.</span></span>    |
|<span data-ttu-id="086db-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="086db-116">Application</span></span> | <span data-ttu-id="086db-117">Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="086db-117">Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="086db-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="086db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="086db-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="086db-119">Optional query parameters</span></span>
<span data-ttu-id="086db-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="086db-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="086db-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="086db-121">Request headers</span></span>
| <span data-ttu-id="086db-122">Имя</span><span class="sxs-lookup"><span data-stu-id="086db-122">Name</span></span>       | <span data-ttu-id="086db-123">Тип</span><span class="sxs-lookup"><span data-stu-id="086db-123">Type</span></span> | <span data-ttu-id="086db-124">Описание</span><span class="sxs-lookup"><span data-stu-id="086db-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="086db-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="086db-125">Authorization</span></span>  | <span data-ttu-id="086db-126">string</span><span class="sxs-lookup"><span data-stu-id="086db-126">string</span></span>  | <span data-ttu-id="086db-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="086db-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="086db-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="086db-129">Request body</span></span>
<span data-ttu-id="086db-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="086db-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="086db-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="086db-131">Response</span></span>
<span data-ttu-id="086db-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="086db-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="086db-133">Пример</span><span class="sxs-lookup"><span data-stu-id="086db-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="086db-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="086db-134">Request</span></span>
<span data-ttu-id="086db-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="086db-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="086db-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="086db-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="086db-137">C#</span><span class="sxs-lookup"><span data-stu-id="086db-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="086db-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="086db-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="086db-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="086db-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="086db-140">Java</span><span class="sxs-lookup"><span data-stu-id="086db-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="086db-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="086db-141">Response</span></span>
<span data-ttu-id="086db-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="086db-142">The following is an example of the response.</span></span>
><span data-ttu-id="086db-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="086db-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="086db-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="086db-144">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
