---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 931d1f06b968a2a8da68245d16eb0de5fec768f5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721280"
---
# <a name="list-members"></a><span data-ttu-id="fc459-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="fc459-104">List members</span></span>

<span data-ttu-id="fc459-105">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="fc459-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="fc459-106">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="fc459-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc459-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc459-107">Permissions</span></span>
<span data-ttu-id="fc459-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc459-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc459-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc459-110">Permission type</span></span>      | <span data-ttu-id="fc459-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc459-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc459-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc459-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc459-113">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="fc459-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc459-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc459-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc459-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc459-115">Not supported.</span></span>    |
|<span data-ttu-id="fc459-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc459-116">Application</span></span> | <span data-ttu-id="fc459-117">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fc459-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc459-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc459-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc459-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc459-119">Optional query parameters</span></span>
<span data-ttu-id="fc459-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fc459-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fc459-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc459-121">Request headers</span></span>
| <span data-ttu-id="fc459-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fc459-122">Name</span></span>       | <span data-ttu-id="fc459-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fc459-123">Type</span></span> | <span data-ttu-id="fc459-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fc459-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fc459-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc459-125">Authorization</span></span>  | <span data-ttu-id="fc459-126">string</span><span class="sxs-lookup"><span data-stu-id="fc459-126">string</span></span>  | <span data-ttu-id="fc459-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc459-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc459-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc459-129">Request body</span></span>
<span data-ttu-id="fc459-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc459-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc459-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc459-131">Response</span></span>

<span data-ttu-id="fc459-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc459-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc459-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fc459-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc459-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc459-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc459-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc459-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc459-136">C#</span><span class="sxs-lookup"><span data-stu-id="fc459-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc459-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc459-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc459-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fc459-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc459-139">Java</span><span class="sxs-lookup"><span data-stu-id="fc459-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc459-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc459-140">Response</span></span>
<span data-ttu-id="fc459-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc459-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
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
