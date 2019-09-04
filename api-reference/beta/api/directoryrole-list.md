---
title: Перечисление объектов directoryRole
description: Перечисление ролей каталога, активированных в клиенте.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 252dab6bf32e4e09abc2aacfa20ac37dbde60174
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719537"
---
# <a name="list-directoryroles"></a><span data-ttu-id="db7f6-103">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="db7f6-103">List directoryRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db7f6-104">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="db7f6-104">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="db7f6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db7f6-105">Permissions</span></span>
<span data-ttu-id="db7f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db7f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7f6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db7f6-108">Permission type</span></span>      | <span data-ttu-id="db7f6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db7f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db7f6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db7f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db7f6-111">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="db7f6-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db7f6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db7f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db7f6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db7f6-113">Not supported.</span></span>    |
|<span data-ttu-id="db7f6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db7f6-114">Application</span></span> | <span data-ttu-id="db7f6-115">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="db7f6-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db7f6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db7f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="db7f6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db7f6-117">Optional query parameters</span></span>
<span data-ttu-id="db7f6-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="db7f6-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="db7f6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db7f6-119">Request headers</span></span>
| <span data-ttu-id="db7f6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db7f6-120">Name</span></span>       | <span data-ttu-id="db7f6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="db7f6-121">Type</span></span> | <span data-ttu-id="db7f6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="db7f6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db7f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db7f6-123">Authorization</span></span>  | <span data-ttu-id="db7f6-124">string</span><span class="sxs-lookup"><span data-stu-id="db7f6-124">string</span></span>  | <span data-ttu-id="db7f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db7f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db7f6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="db7f6-127">Request body</span></span>
<span data-ttu-id="db7f6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db7f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db7f6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="db7f6-129">Response</span></span>

<span data-ttu-id="db7f6-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db7f6-130">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db7f6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="db7f6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db7f6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="db7f6-132">Request</span></span>
<span data-ttu-id="db7f6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db7f6-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db7f6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="db7f6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db7f6-135">C#</span><span class="sxs-lookup"><span data-stu-id="db7f6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db7f6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db7f6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db7f6-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="db7f6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db7f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="db7f6-138">Response</span></span>
<span data-ttu-id="db7f6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db7f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

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
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
