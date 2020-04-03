---
title: Список memberOf
description: 'Получение групп, непосредственным членом которых является данная группа. '
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7f30b10ef9c6b33fc92b86b02fefe8c4c71c4a39
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125227"
---
# <a name="list-memberof"></a><span data-ttu-id="6a093-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="6a093-103">List memberOf</span></span>

<span data-ttu-id="6a093-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a093-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a093-105">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="6a093-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="6a093-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Office 365", эта операция возвращает группы всех типов, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="6a093-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a093-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a093-108">Permissions</span></span>
<span data-ttu-id="6a093-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a093-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a093-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a093-111">Permission type</span></span>      | <span data-ttu-id="6a093-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a093-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a093-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a093-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6a093-114">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a093-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="6a093-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a093-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a093-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a093-116">Not supported.</span></span>    |
|<span data-ttu-id="6a093-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6a093-117">Application</span></span> | <span data-ttu-id="6a093-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a093-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6a093-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a093-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a093-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a093-120">Optional query parameters</span></span>
<span data-ttu-id="6a093-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a093-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a093-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a093-122">Request headers</span></span>
| <span data-ttu-id="6a093-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6a093-123">Name</span></span>       | <span data-ttu-id="6a093-124">Тип</span><span class="sxs-lookup"><span data-stu-id="6a093-124">Type</span></span> | <span data-ttu-id="6a093-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6a093-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a093-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a093-126">Authorization</span></span>  | <span data-ttu-id="6a093-127">string</span><span class="sxs-lookup"><span data-stu-id="6a093-127">string</span></span>  | <span data-ttu-id="6a093-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a093-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a093-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a093-130">Request body</span></span>
<span data-ttu-id="6a093-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a093-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a093-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a093-132">Response</span></span>
<span data-ttu-id="6a093-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a093-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a093-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6a093-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6a093-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a093-135">Request</span></span>
<span data-ttu-id="6a093-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a093-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a093-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a093-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="6a093-138">C#</span><span class="sxs-lookup"><span data-stu-id="6a093-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a093-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a093-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a093-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a093-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a093-141">Java</span><span class="sxs-lookup"><span data-stu-id="6a093-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6a093-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a093-142">Response</span></span>
<span data-ttu-id="6a093-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a093-143">The following is an example of the response.</span></span>
><span data-ttu-id="6a093-144">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6a093-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6a093-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a093-145">All the properties will be returned from an actual call.</span></span>
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
