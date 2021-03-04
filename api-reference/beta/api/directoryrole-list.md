---
title: Перечисление объектов directoryRole
description: Перечисление ролей каталога, активированных в клиенте.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 273a83bf85f884c3f1bb9eebeead67230d6420a5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436759"
---
# <a name="list-directoryroles"></a><span data-ttu-id="ca3a2-103">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="ca3a2-103">List directoryRoles</span></span>

<span data-ttu-id="ca3a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca3a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca3a2-105">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ca3a2-105">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca3a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3a2-106">Permissions</span></span>
<span data-ttu-id="ca3a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca3a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca3a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3a2-109">Permission type</span></span>      | <span data-ttu-id="ca3a2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca3a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca3a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca3a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca3a2-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca3a2-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca3a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca3a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca3a2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3a2-114">Not supported.</span></span>    |
|<span data-ttu-id="ca3a2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca3a2-115">Application</span></span> | <span data-ttu-id="ca3a2-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca3a2-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca3a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca3a2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca3a2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca3a2-118">Optional query parameters</span></span>
<span data-ttu-id="ca3a2-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="ca3a2-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca3a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca3a2-120">Request headers</span></span>
| <span data-ttu-id="ca3a2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ca3a2-121">Name</span></span>       | <span data-ttu-id="ca3a2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ca3a2-122">Type</span></span> | <span data-ttu-id="ca3a2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ca3a2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca3a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca3a2-124">Authorization</span></span>  | <span data-ttu-id="ca3a2-125">string</span><span class="sxs-lookup"><span data-stu-id="ca3a2-125">string</span></span>  | <span data-ttu-id="ca3a2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca3a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca3a2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca3a2-128">Request body</span></span>
<span data-ttu-id="ca3a2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca3a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca3a2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3a2-130">Response</span></span>

<span data-ttu-id="ca3a2-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3a2-131">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca3a2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ca3a2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca3a2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca3a2-133">Request</span></span>
<span data-ttu-id="ca3a2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca3a2-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca3a2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca3a2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="ca3a2-136">C#</span><span class="sxs-lookup"><span data-stu-id="ca3a2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca3a2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca3a2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca3a2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca3a2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca3a2-139">Java</span><span class="sxs-lookup"><span data-stu-id="ca3a2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca3a2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3a2-140">Response</span></span>
<span data-ttu-id="ca3a2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca3a2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
