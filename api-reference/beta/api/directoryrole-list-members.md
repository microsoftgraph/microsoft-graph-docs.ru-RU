---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0f4b0337d5e070af24e6bbfc7d3bdc3aeddbd3aa
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719558"
---
# <a name="list-members"></a><span data-ttu-id="9d0b3-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="9d0b3-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d0b3-105">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="9d0b3-106">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d0b3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d0b3-107">Permissions</span></span>
<span data-ttu-id="9d0b3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d0b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d0b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d0b3-110">Permission type</span></span>      | <span data-ttu-id="9d0b3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d0b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d0b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d0b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d0b3-113">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9d0b3-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d0b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d0b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d0b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-115">Not supported.</span></span>    |
|<span data-ttu-id="9d0b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d0b3-116">Application</span></span> | <span data-ttu-id="9d0b3-117">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9d0b3-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d0b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d0b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d0b3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d0b3-119">Optional query parameters</span></span>
<span data-ttu-id="9d0b3-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9d0b3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d0b3-121">Request headers</span></span>
| <span data-ttu-id="9d0b3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9d0b3-122">Name</span></span>       | <span data-ttu-id="9d0b3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9d0b3-123">Type</span></span> | <span data-ttu-id="9d0b3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9d0b3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d0b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d0b3-125">Authorization</span></span>  | <span data-ttu-id="9d0b3-126">string</span><span class="sxs-lookup"><span data-stu-id="9d0b3-126">string</span></span>  | <span data-ttu-id="9d0b3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d0b3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d0b3-129">Request body</span></span>
<span data-ttu-id="9d0b3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d0b3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d0b3-131">Response</span></span>

<span data-ttu-id="9d0b3-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d0b3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9d0b3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d0b3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d0b3-134">Request</span></span>
<span data-ttu-id="9d0b3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9d0b3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d0b3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9d0b3-137">C#</span><span class="sxs-lookup"><span data-stu-id="9d0b3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9d0b3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d0b3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9d0b3-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9d0b3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9d0b3-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d0b3-140">Response</span></span>
<span data-ttu-id="9d0b3-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d0b3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
