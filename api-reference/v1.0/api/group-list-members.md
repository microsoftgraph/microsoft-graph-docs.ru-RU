---
title: Список участников
description: Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты и другие группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 04a55e4fa188fcd8d0cc6a068d6655f7fb62beee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016286"
---
# <a name="list-members"></a><span data-ttu-id="bd303-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="bd303-104">List members</span></span>
<span data-ttu-id="bd303-p102">Получение списка непосредственных участников группы. Участниками групп могут быть пользователи, контакты и другие группы. Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="bd303-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd303-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd303-108">Permissions</span></span>
<span data-ttu-id="bd303-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd303-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd303-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd303-111">Permission type</span></span>      | <span data-ttu-id="bd303-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd303-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd303-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd303-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bd303-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd303-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="bd303-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd303-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd303-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd303-116">Not supported.</span></span>    |
|<span data-ttu-id="bd303-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd303-117">Application</span></span> | <span data-ttu-id="bd303-118">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd303-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd303-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd303-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd303-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd303-120">Optional query parameters</span></span>
<span data-ttu-id="bd303-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bd303-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd303-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd303-122">Request headers</span></span>
| <span data-ttu-id="bd303-123">Имя</span><span class="sxs-lookup"><span data-stu-id="bd303-123">Name</span></span>       | <span data-ttu-id="bd303-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bd303-124">Type</span></span> | <span data-ttu-id="bd303-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bd303-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bd303-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd303-126">Authorization</span></span>  | <span data-ttu-id="bd303-127">string</span><span class="sxs-lookup"><span data-stu-id="bd303-127">string</span></span>  | <span data-ttu-id="bd303-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd303-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd303-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd303-130">Request body</span></span>
<span data-ttu-id="bd303-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd303-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd303-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd303-132">Response</span></span>
<span data-ttu-id="bd303-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd303-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd303-134">Пример</span><span class="sxs-lookup"><span data-stu-id="bd303-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bd303-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd303-135">Request</span></span>
<span data-ttu-id="bd303-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd303-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd303-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd303-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd303-138">C#</span><span class="sxs-lookup"><span data-stu-id="bd303-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd303-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd303-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd303-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd303-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bd303-141">Java</span><span class="sxs-lookup"><span data-stu-id="bd303-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd303-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd303-142">Response</span></span>
<span data-ttu-id="bd303-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd303-143">The following is an example of the response.</span></span>
><span data-ttu-id="bd303-144">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd303-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd303-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd303-145">All the properties will be returned from an actual call.</span></span>
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
