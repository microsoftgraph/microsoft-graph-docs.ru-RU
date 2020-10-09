---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4a0b047592d3e357f83125ca6662074f58d2d8e3
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401133"
---
# <a name="list-members"></a><span data-ttu-id="06896-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="06896-104">List members</span></span>

<span data-ttu-id="06896-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06896-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06896-106">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="06896-106">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="06896-107">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="06896-107">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="06896-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06896-108">Permissions</span></span>
<span data-ttu-id="06896-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06896-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06896-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06896-111">Permission type</span></span>      | <span data-ttu-id="06896-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06896-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06896-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06896-113">Delegated (work or school account)</span></span> | <span data-ttu-id="06896-114">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="06896-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06896-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06896-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06896-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06896-116">Not supported.</span></span>    |
|<span data-ttu-id="06896-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06896-117">Application</span></span> | <span data-ttu-id="06896-118">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="06896-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="06896-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06896-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06896-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06896-120">Optional query parameters</span></span>
<span data-ttu-id="06896-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06896-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="06896-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06896-122">Request headers</span></span>
| <span data-ttu-id="06896-123">Имя</span><span class="sxs-lookup"><span data-stu-id="06896-123">Name</span></span>       | <span data-ttu-id="06896-124">Тип</span><span class="sxs-lookup"><span data-stu-id="06896-124">Type</span></span> | <span data-ttu-id="06896-125">Описание</span><span class="sxs-lookup"><span data-stu-id="06896-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06896-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="06896-126">Authorization</span></span>  | <span data-ttu-id="06896-127">string</span><span class="sxs-lookup"><span data-stu-id="06896-127">string</span></span>  | <span data-ttu-id="06896-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06896-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06896-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06896-130">Request body</span></span>
<span data-ttu-id="06896-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06896-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06896-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="06896-132">Response</span></span>

<span data-ttu-id="06896-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06896-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06896-134">Пример</span><span class="sxs-lookup"><span data-stu-id="06896-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06896-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="06896-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="06896-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="06896-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="06896-137">C#</span><span class="sxs-lookup"><span data-stu-id="06896-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06896-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06896-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06896-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06896-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06896-140">Java</span><span class="sxs-lookup"><span data-stu-id="06896-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06896-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="06896-141">Response</span></span>
<span data-ttu-id="06896-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06896-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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