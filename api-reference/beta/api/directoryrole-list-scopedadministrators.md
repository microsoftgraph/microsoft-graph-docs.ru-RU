---
title: Список scopedMembers для роли каталога
description: Извлечение списка объектов scopedRoleMembership для роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6a699d0ad6a87bfffa97029292a9f833ce7294d1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436766"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="7891a-103">Список scopedMembers для роли каталога</span><span class="sxs-lookup"><span data-stu-id="7891a-103">List scopedMembers for a directory role</span></span>

<span data-ttu-id="7891a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7891a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7891a-105">Извлечение списка [объектов scopedRoleMembership](../resources/scopedrolemembership.md) для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="7891a-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="7891a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7891a-106">Permissions</span></span>
<span data-ttu-id="7891a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7891a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7891a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7891a-109">Permission type</span></span>      | <span data-ttu-id="7891a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7891a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7891a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7891a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7891a-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7891a-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7891a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7891a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7891a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7891a-114">Not supported.</span></span>    |
|<span data-ttu-id="7891a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7891a-115">Application</span></span> | <span data-ttu-id="7891a-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7891a-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7891a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7891a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7891a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7891a-118">Optional query parameters</span></span>
<span data-ttu-id="7891a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7891a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7891a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7891a-120">Request headers</span></span>
| <span data-ttu-id="7891a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7891a-121">Name</span></span>      |<span data-ttu-id="7891a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7891a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7891a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7891a-123">Authorization</span></span>  | <span data-ttu-id="7891a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7891a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7891a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7891a-126">Request body</span></span>
<span data-ttu-id="7891a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7891a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7891a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7891a-128">Response</span></span>

<span data-ttu-id="7891a-129">В случае успешного применения этот метод возвращает код ответа и коллекцию объектов `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7891a-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7891a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7891a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7891a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7891a-131">Request</span></span>
<span data-ttu-id="7891a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7891a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7891a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7891a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="7891a-134">C#</span><span class="sxs-lookup"><span data-stu-id="7891a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7891a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7891a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7891a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7891a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7891a-137">Java</span><span class="sxs-lookup"><span data-stu-id="7891a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7891a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7891a-138">Response</span></span>
<span data-ttu-id="7891a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7891a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
