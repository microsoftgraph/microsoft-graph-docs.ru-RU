---
title: Перечисление объектов directoryRole
description: Перечисление ролей каталога, активированных в клиенте.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 998646fc16119ad7aaccf468fff5b9156cf7a3d2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434407"
---
# <a name="list-directoryroles"></a><span data-ttu-id="e42fc-103">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="e42fc-103">List directoryRoles</span></span>

<span data-ttu-id="e42fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e42fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e42fc-105">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e42fc-105">List the directory roles that are activated in the tenant.</span></span>

<span data-ttu-id="e42fc-106">Эта операция возвращает только роли, которые были активированы.</span><span class="sxs-lookup"><span data-stu-id="e42fc-106">This operation only returns roles that have been activated.</span></span> <span data-ttu-id="e42fc-107">Роль активируется, когда администратор активирует роль с помощью API [Activat directoryRole.](directoryrole-post-directoryroles.md)</span><span class="sxs-lookup"><span data-stu-id="e42fc-107">A role becomes activated when an admin activates the role using the [Activate directoryRole](directoryrole-post-directoryroles.md) API.</span></span> <span data-ttu-id="e42fc-108">Не все встроенные роли изначально активируются.</span><span class="sxs-lookup"><span data-stu-id="e42fc-108">Not all built-in roles are initially activated.</span></span> 

<span data-ttu-id="e42fc-109">При назначении роли с помощью портала Azure шаг активации роли неявно делается от имени администратора.</span><span class="sxs-lookup"><span data-stu-id="e42fc-109">When assigning a role using the Azure portal, the role activation step is implicitly done on the admin's behalf.</span></span> <span data-ttu-id="e42fc-110">Чтобы получить полный список ролей, доступных в Azure AD, используйте [list directoryRoleTemplates.](directoryroletemplate-list.md)</span><span class="sxs-lookup"><span data-stu-id="e42fc-110">To get the full list of roles that are available in Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e42fc-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e42fc-111">Permissions</span></span>
<span data-ttu-id="e42fc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e42fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e42fc-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e42fc-114">Permission type</span></span>      | <span data-ttu-id="e42fc-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e42fc-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e42fc-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e42fc-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e42fc-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e42fc-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e42fc-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e42fc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e42fc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e42fc-119">Not supported.</span></span>    |
|<span data-ttu-id="e42fc-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e42fc-120">Application</span></span> | <span data-ttu-id="e42fc-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e42fc-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e42fc-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e42fc-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e42fc-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e42fc-123">Optional query parameters</span></span>
<span data-ttu-id="e42fc-124">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="e42fc-124">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e42fc-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e42fc-125">Request headers</span></span>
| <span data-ttu-id="e42fc-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e42fc-126">Name</span></span>       | <span data-ttu-id="e42fc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e42fc-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e42fc-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e42fc-128">Authorization</span></span>  | <span data-ttu-id="e42fc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e42fc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e42fc-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e42fc-131">Request body</span></span>
<span data-ttu-id="e42fc-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e42fc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e42fc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e42fc-133">Response</span></span>

<span data-ttu-id="e42fc-134">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e42fc-134">If successful, this method returns a `200 OK` response code and a collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e42fc-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e42fc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e42fc-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e42fc-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e42fc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e42fc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="e42fc-138">C#</span><span class="sxs-lookup"><span data-stu-id="e42fc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e42fc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e42fc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e42fc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e42fc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e42fc-141">Java</span><span class="sxs-lookup"><span data-stu-id="e42fc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e42fc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e42fc-142">Response</span></span>
<span data-ttu-id="e42fc-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e42fc-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
