---
title: Список владельцев
description: Получение списка владельцев группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fd6534256e60b5fbc1e699eab2e6df787ab63864
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002123"
---
# <a name="list-owners"></a><span data-ttu-id="c5f62-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="c5f62-103">List owners</span></span>

<span data-ttu-id="c5f62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f62-p101">Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="c5f62-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5f62-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f62-107">Permissions</span></span>
<span data-ttu-id="c5f62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f62-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f62-110">Permission type</span></span>      | <span data-ttu-id="c5f62-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5f62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5f62-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5f62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5f62-113">Group. Read. ALL и User. ReadBasic. ALL, Group. Read. ALL и User. Read. ALL, Group. Read. ALL и User. ReadWrite. ALL, Group. Read. ALL и User. Read. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c5f62-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>  |
|<span data-ttu-id="c5f62-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5f62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f62-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f62-115">Not supported.</span></span>    |
|<span data-ttu-id="c5f62-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c5f62-116">Application</span></span> | <span data-ttu-id="c5f62-117">Group. Read. ALL и User. Read. ALL, Group. Read. ALL и User. ReadWrite. ALL, Group. Read. ALL и User. Read. ALL и Application. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="c5f62-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c5f62-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5f62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5f62-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5f62-119">Optional query parameters</span></span>
<span data-ttu-id="c5f62-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5f62-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5f62-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5f62-121">Request headers</span></span>
| <span data-ttu-id="c5f62-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c5f62-122">Name</span></span>       | <span data-ttu-id="c5f62-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f62-123">Type</span></span> | <span data-ttu-id="c5f62-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f62-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5f62-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f62-125">Authorization</span></span>  | <span data-ttu-id="c5f62-126">string</span><span class="sxs-lookup"><span data-stu-id="c5f62-126">string</span></span>  | <span data-ttu-id="c5f62-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5f62-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5f62-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5f62-129">Request body</span></span>
<span data-ttu-id="c5f62-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5f62-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5f62-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5f62-131">Response</span></span>
<span data-ttu-id="c5f62-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5f62-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f62-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c5f62-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c5f62-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f62-134">Request</span></span>
<span data-ttu-id="c5f62-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5f62-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5f62-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f62-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="c5f62-137">C#</span><span class="sxs-lookup"><span data-stu-id="c5f62-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5f62-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5f62-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5f62-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5f62-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5f62-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5f62-140">Response</span></span>
<span data-ttu-id="c5f62-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5f62-141">The following is an example of the response.</span></span>
><span data-ttu-id="c5f62-142">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c5f62-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c5f62-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5f62-143">All the properties will be returned from an actual call.</span></span>
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


