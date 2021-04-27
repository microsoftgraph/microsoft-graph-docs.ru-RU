---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9425849444a31454e3a98fcd2fbabd8a04184938
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046827"
---
# <a name="list-members"></a><span data-ttu-id="c736d-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="c736d-104">List members</span></span>

<span data-ttu-id="c736d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c736d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c736d-p102">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="c736d-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="c736d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c736d-108">Permissions</span></span>
<span data-ttu-id="c736d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c736d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c736d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c736d-111">Permission type</span></span>      | <span data-ttu-id="c736d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c736d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c736d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c736d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c736d-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c736d-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c736d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c736d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c736d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c736d-116">Not supported.</span></span>    |
|<span data-ttu-id="c736d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c736d-117">Application</span></span> | <span data-ttu-id="c736d-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c736d-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c736d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c736d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c736d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c736d-120">Optional query parameters</span></span>
<span data-ttu-id="c736d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c736d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c736d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c736d-122">Request headers</span></span>
| <span data-ttu-id="c736d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c736d-123">Name</span></span>       | <span data-ttu-id="c736d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c736d-124">Type</span></span> | <span data-ttu-id="c736d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c736d-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c736d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c736d-126">Authorization</span></span>  | <span data-ttu-id="c736d-127">string</span><span class="sxs-lookup"><span data-stu-id="c736d-127">string</span></span>  | <span data-ttu-id="c736d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c736d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c736d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c736d-130">Request body</span></span>
<span data-ttu-id="c736d-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c736d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c736d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c736d-132">Response</span></span>

<span data-ttu-id="c736d-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c736d-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c736d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c736d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c736d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c736d-135">Request</span></span>
<span data-ttu-id="c736d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c736d-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c736d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c736d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="c736d-138">C#</span><span class="sxs-lookup"><span data-stu-id="c736d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c736d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c736d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c736d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c736d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c736d-141">Java</span><span class="sxs-lookup"><span data-stu-id="c736d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c736d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c736d-142">Response</span></span>
<span data-ttu-id="c736d-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c736d-143">Here is an example of the response.</span></span> <span data-ttu-id="c736d-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c736d-144">Note: The response object shown here might be shortened for readability.</span></span>
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
