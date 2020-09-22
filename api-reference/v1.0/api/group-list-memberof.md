---
title: Список memberOf
description: 'Получение групп, непосредственным членом которых является данная группа. '
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a6a87d643c9cd0b53b4769f6943f4a6f8e779f5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038622"
---
# <a name="list-memberof"></a><span data-ttu-id="7e85a-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="7e85a-103">List memberOf</span></span>

<span data-ttu-id="7e85a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e85a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e85a-105">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="7e85a-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="7e85a-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Microsoft 365", эта операция возвращает группы всех типов, а не только группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7e85a-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e85a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e85a-108">Permissions</span></span>
<span data-ttu-id="7e85a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e85a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e85a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e85a-111">Permission type</span></span>      | <span data-ttu-id="7e85a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e85a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e85a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e85a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7e85a-114">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e85a-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="7e85a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e85a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e85a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e85a-116">Not supported.</span></span>    |
|<span data-ttu-id="7e85a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7e85a-117">Application</span></span> | <span data-ttu-id="7e85a-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e85a-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="7e85a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e85a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e85a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e85a-120">Optional query parameters</span></span>
<span data-ttu-id="7e85a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e85a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e85a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e85a-122">Request headers</span></span>
| <span data-ttu-id="7e85a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7e85a-123">Name</span></span>       | <span data-ttu-id="7e85a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7e85a-124">Type</span></span> | <span data-ttu-id="7e85a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7e85a-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7e85a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e85a-126">Authorization</span></span>  | <span data-ttu-id="7e85a-127">string</span><span class="sxs-lookup"><span data-stu-id="7e85a-127">string</span></span>  | <span data-ttu-id="7e85a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e85a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e85a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e85a-130">Request body</span></span>
<span data-ttu-id="7e85a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e85a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e85a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e85a-132">Response</span></span>
<span data-ttu-id="7e85a-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e85a-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e85a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7e85a-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7e85a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e85a-135">Request</span></span>
<span data-ttu-id="7e85a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e85a-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e85a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e85a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="7e85a-138">C#</span><span class="sxs-lookup"><span data-stu-id="7e85a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e85a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e85a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e85a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e85a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e85a-141">Java</span><span class="sxs-lookup"><span data-stu-id="7e85a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e85a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e85a-142">Response</span></span>
<span data-ttu-id="7e85a-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e85a-143">The following is an example of the response.</span></span>
><span data-ttu-id="7e85a-144">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7e85a-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7e85a-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e85a-145">All the properties will be returned from an actual call.</span></span>
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

