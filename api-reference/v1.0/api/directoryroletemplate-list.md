---
title: Список directoryRoleTemplate
description: Получение списка объектов directoryRoleTemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 78901c7415d59f148010e572fc9a438a71dd1765
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441986"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="edce9-103">Список directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="edce9-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="edce9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edce9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edce9-105">Получение списка объектов directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="edce9-105">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="edce9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edce9-106">Permissions</span></span>
<span data-ttu-id="edce9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="edce9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edce9-109">Permission type</span></span>      | <span data-ttu-id="edce9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edce9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edce9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edce9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="edce9-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edce9-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="edce9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edce9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edce9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edce9-114">Not supported.</span></span>    |
|<span data-ttu-id="edce9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edce9-115">Application</span></span> | <span data-ttu-id="edce9-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edce9-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="edce9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edce9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="edce9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="edce9-118">Optional query parameters</span></span>
<span data-ttu-id="edce9-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="edce9-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="edce9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edce9-120">Request headers</span></span>
| <span data-ttu-id="edce9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="edce9-121">Name</span></span>       | <span data-ttu-id="edce9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="edce9-122">Type</span></span> | <span data-ttu-id="edce9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="edce9-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="edce9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="edce9-124">Authorization</span></span>  | <span data-ttu-id="edce9-125">string</span><span class="sxs-lookup"><span data-stu-id="edce9-125">string</span></span>  | <span data-ttu-id="edce9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edce9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="edce9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edce9-128">Request body</span></span>
<span data-ttu-id="edce9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edce9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edce9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="edce9-130">Response</span></span>

<span data-ttu-id="edce9-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="edce9-131">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="edce9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="edce9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edce9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="edce9-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="edce9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="edce9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
# <a name="c"></a>[<span data-ttu-id="edce9-135">C#</span><span class="sxs-lookup"><span data-stu-id="edce9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edce9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edce9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edce9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edce9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edce9-138">Java</span><span class="sxs-lookup"><span data-stu-id="edce9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="edce9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="edce9-139">Response</span></span>
<span data-ttu-id="edce9-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edce9-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
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
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
