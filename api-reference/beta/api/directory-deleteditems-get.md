---
title: Получение удаленного элемента
description: Получение свойств недавно удаленного элемента.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 58a6b537e8b4e4f2a1e589651de73556da096332
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319610"
---
# <a name="get-deleted-item"></a><span data-ttu-id="5bad9-103">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="5bad9-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bad9-104">Получение свойств недавно [удаленного элемента](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="5bad9-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="5bad9-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="5bad9-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bad9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bad9-106">Permissions</span></span>
<span data-ttu-id="5bad9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bad9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="5bad9-109">Для пользователей: User. Read. ALL, User. ReadWrite. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5bad9-109">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="5bad9-110">Для групп: Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5bad9-110">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5bad9-111">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bad9-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bad9-112">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5bad9-112">Optional query parameters</span></span>
<span data-ttu-id="5bad9-113">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5bad9-113">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bad9-114">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bad9-114">Request headers</span></span>
| <span data-ttu-id="5bad9-115">Имя</span><span class="sxs-lookup"><span data-stu-id="5bad9-115">Name</span></span>      |<span data-ttu-id="5bad9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="5bad9-116">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5bad9-117">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bad9-117">Authorization</span></span>  | <span data-ttu-id="5bad9-118">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="5bad9-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="5bad9-119">Accept</span><span class="sxs-lookup"><span data-stu-id="5bad9-119">Accept</span></span>  | <span data-ttu-id="5bad9-120">application/json</span><span class="sxs-lookup"><span data-stu-id="5bad9-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bad9-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bad9-121">Request body</span></span>
<span data-ttu-id="5bad9-122">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bad9-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bad9-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bad9-123">Response</span></span>

<span data-ttu-id="5bad9-124">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bad9-124">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5bad9-125">Пример</span><span class="sxs-lookup"><span data-stu-id="5bad9-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bad9-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bad9-126">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5bad9-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bad9-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5bad9-128">C#</span><span class="sxs-lookup"><span data-stu-id="5bad9-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bad9-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bad9-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5bad9-130">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5bad9-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5bad9-131">Java</span><span class="sxs-lookup"><span data-stu-id="5bad9-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5bad9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bad9-132">Response</span></span>
<span data-ttu-id="5bad9-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bad9-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
