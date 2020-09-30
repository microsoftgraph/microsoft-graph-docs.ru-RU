---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 47b5e3df716a98a1e8a90f382ed0caa6c6564497
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313410"
---
# <a name="list-members"></a><span data-ttu-id="271a0-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="271a0-104">List members</span></span>

<span data-ttu-id="271a0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="271a0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="271a0-106">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="271a0-106">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="271a0-107">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="271a0-107">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="271a0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="271a0-108">Permissions</span></span>
<span data-ttu-id="271a0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="271a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="271a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="271a0-111">Permission type</span></span>      | <span data-ttu-id="271a0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="271a0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="271a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="271a0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="271a0-114">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="271a0-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="271a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="271a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="271a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="271a0-116">Not supported.</span></span>    |
|<span data-ttu-id="271a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="271a0-117">Application</span></span> | <span data-ttu-id="271a0-118">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="271a0-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="271a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="271a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="271a0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="271a0-120">Optional query parameters</span></span>
<span data-ttu-id="271a0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="271a0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="271a0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="271a0-122">Request headers</span></span>
| <span data-ttu-id="271a0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="271a0-123">Name</span></span>       | <span data-ttu-id="271a0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="271a0-124">Type</span></span> | <span data-ttu-id="271a0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="271a0-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="271a0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="271a0-126">Authorization</span></span>  | <span data-ttu-id="271a0-127">string</span><span class="sxs-lookup"><span data-stu-id="271a0-127">string</span></span>  | <span data-ttu-id="271a0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="271a0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="271a0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="271a0-130">Request body</span></span>
<span data-ttu-id="271a0-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="271a0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="271a0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="271a0-132">Response</span></span>

<span data-ttu-id="271a0-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="271a0-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="271a0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="271a0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="271a0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="271a0-135">Request</span></span>
<span data-ttu-id="271a0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="271a0-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="271a0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="271a0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="271a0-138">C#</span><span class="sxs-lookup"><span data-stu-id="271a0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="271a0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="271a0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="271a0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="271a0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="271a0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="271a0-141">Response</span></span>
<span data-ttu-id="271a0-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="271a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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