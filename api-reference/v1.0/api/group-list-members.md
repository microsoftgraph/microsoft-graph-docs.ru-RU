---
title: Список участников
description: Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты организации и другие группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a4465a50db0611577bb78bc27b22432971599a64
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869894"
---
# <a name="list-members"></a><span data-ttu-id="0826a-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="0826a-104">List members</span></span>
<span data-ttu-id="0826a-p102">Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты организации и другие группы. Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="0826a-p102">Get a list of the group's direct members. A group can have users, organizational contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0826a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0826a-108">Permissions</span></span>
<span data-ttu-id="0826a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0826a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0826a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0826a-111">Permission type</span></span>      | <span data-ttu-id="0826a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0826a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0826a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0826a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0826a-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0826a-114">User.ReadBasic.All, User.Read.All, Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="0826a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0826a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0826a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0826a-116">Not supported.</span></span>    |
|<span data-ttu-id="0826a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0826a-117">Application</span></span> | <span data-ttu-id="0826a-118">User.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0826a-118">User.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0826a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0826a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0826a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0826a-120">Optional query parameters</span></span>
<span data-ttu-id="0826a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0826a-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0826a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0826a-122">Request headers</span></span>
| <span data-ttu-id="0826a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0826a-123">Header</span></span>       | <span data-ttu-id="0826a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0826a-124">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="0826a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0826a-125">Authorization</span></span>  | <span data-ttu-id="0826a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0826a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0826a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0826a-128">Request body</span></span>
<span data-ttu-id="0826a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0826a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0826a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0826a-130">Response</span></span>
<span data-ttu-id="0826a-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0826a-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0826a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0826a-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0826a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0826a-133">Request</span></span>
<span data-ttu-id="0826a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0826a-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0826a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0826a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0826a-136">C#</span><span class="sxs-lookup"><span data-stu-id="0826a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0826a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0826a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0826a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0826a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0826a-139">Java</span><span class="sxs-lookup"><span data-stu-id="0826a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0826a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0826a-140">Response</span></span>
<span data-ttu-id="0826a-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0826a-141">The following is an example of the response.</span></span>
><span data-ttu-id="0826a-142">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0826a-142">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
