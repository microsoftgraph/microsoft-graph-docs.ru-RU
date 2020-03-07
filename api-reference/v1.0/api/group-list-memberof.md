---
title: Список memberOf
description: 'Получение групп, непосредственным членом которых является данная группа. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 120cb02837ee30bc67ce315e158d4d4361a8be42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517077"
---
# <a name="list-memberof"></a><span data-ttu-id="31847-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="31847-103">List memberOf</span></span>

<span data-ttu-id="31847-104">Пространство имен: microsoft.graph. Получение групп, непосредственным участником которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="31847-104">Namespace: microsoft.graph Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="31847-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Office 365", эта операция возвращает группы всех типов, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="31847-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="31847-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31847-107">Permissions</span></span>
<span data-ttu-id="31847-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31847-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31847-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31847-110">Permission type</span></span>      | <span data-ttu-id="31847-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31847-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31847-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31847-112">Delegated (work or school account)</span></span> | <span data-ttu-id="31847-113">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31847-113">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="31847-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31847-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31847-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31847-115">Not supported.</span></span>    |
|<span data-ttu-id="31847-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="31847-116">Application</span></span> | <span data-ttu-id="31847-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="31847-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="31847-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31847-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31847-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="31847-119">Optional query parameters</span></span>
<span data-ttu-id="31847-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="31847-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31847-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31847-121">Request headers</span></span>
| <span data-ttu-id="31847-122">Имя</span><span class="sxs-lookup"><span data-stu-id="31847-122">Name</span></span>       | <span data-ttu-id="31847-123">Тип</span><span class="sxs-lookup"><span data-stu-id="31847-123">Type</span></span> | <span data-ttu-id="31847-124">Описание</span><span class="sxs-lookup"><span data-stu-id="31847-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="31847-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="31847-125">Authorization</span></span>  | <span data-ttu-id="31847-126">string</span><span class="sxs-lookup"><span data-stu-id="31847-126">string</span></span>  | <span data-ttu-id="31847-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31847-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31847-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31847-129">Request body</span></span>
<span data-ttu-id="31847-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31847-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31847-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="31847-131">Response</span></span>
<span data-ttu-id="31847-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31847-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31847-133">Пример</span><span class="sxs-lookup"><span data-stu-id="31847-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="31847-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="31847-134">Request</span></span>
<span data-ttu-id="31847-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31847-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31847-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="31847-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="31847-137">C#</span><span class="sxs-lookup"><span data-stu-id="31847-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31847-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31847-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31847-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31847-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31847-140">Java</span><span class="sxs-lookup"><span data-stu-id="31847-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="31847-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="31847-141">Response</span></span>
<span data-ttu-id="31847-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31847-142">The following is an example of the response.</span></span>
><span data-ttu-id="31847-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31847-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="31847-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31847-144">All the properties will be returned from an actual call.</span></span>
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
