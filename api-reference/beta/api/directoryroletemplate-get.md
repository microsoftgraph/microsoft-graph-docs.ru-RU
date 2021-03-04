---
title: Вывод объекта directoryRoleTemplate
description: Получение свойств и связей объекта directoryRoleTemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4b6f238fc4c3cafe83b1fdd908e3b5b2bb6bf9fa
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436717"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="1599a-103">Вывод объекта directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="1599a-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="1599a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1599a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1599a-105">Получение свойств и связей объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="1599a-105">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1599a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1599a-106">Permissions</span></span>
<span data-ttu-id="1599a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1599a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1599a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1599a-109">Permission type</span></span>      | <span data-ttu-id="1599a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1599a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1599a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1599a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1599a-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1599a-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1599a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1599a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1599a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1599a-114">Not supported.</span></span>    |
|<span data-ttu-id="1599a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1599a-115">Application</span></span> | <span data-ttu-id="1599a-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1599a-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1599a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1599a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1599a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1599a-118">Optional query parameters</span></span>
<span data-ttu-id="1599a-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="1599a-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1599a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1599a-120">Request headers</span></span>
| <span data-ttu-id="1599a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1599a-121">Name</span></span>       | <span data-ttu-id="1599a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1599a-122">Type</span></span> | <span data-ttu-id="1599a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1599a-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1599a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1599a-124">Authorization</span></span>  | <span data-ttu-id="1599a-125">string</span><span class="sxs-lookup"><span data-stu-id="1599a-125">string</span></span>  | <span data-ttu-id="1599a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1599a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1599a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1599a-128">Request body</span></span>
<span data-ttu-id="1599a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1599a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1599a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1599a-130">Response</span></span>

<span data-ttu-id="1599a-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1599a-131">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1599a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1599a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1599a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1599a-133">Request</span></span>
<span data-ttu-id="1599a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1599a-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1599a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1599a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="1599a-136">C#</span><span class="sxs-lookup"><span data-stu-id="1599a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1599a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1599a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1599a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1599a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1599a-139">Java</span><span class="sxs-lookup"><span data-stu-id="1599a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1599a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1599a-140">Response</span></span>
<span data-ttu-id="1599a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1599a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
