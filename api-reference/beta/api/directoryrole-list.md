---
title: Перечисление объектов directoryRole
description: Перечисление ролей каталога, активированных в клиенте.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: daad6cdab1c9c773d640c00bf3df0585820df4f7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964040"
---
# <a name="list-directoryroles"></a><span data-ttu-id="748ca-103">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="748ca-103">List directoryRoles</span></span>

<span data-ttu-id="748ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="748ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="748ca-105">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="748ca-105">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="748ca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="748ca-106">Permissions</span></span>
<span data-ttu-id="748ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="748ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="748ca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="748ca-109">Permission type</span></span>      | <span data-ttu-id="748ca-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="748ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="748ca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="748ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="748ca-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="748ca-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="748ca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="748ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="748ca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="748ca-114">Not supported.</span></span>    |
|<span data-ttu-id="748ca-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="748ca-115">Application</span></span> | <span data-ttu-id="748ca-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="748ca-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="748ca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="748ca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="748ca-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="748ca-118">Optional query parameters</span></span>
<span data-ttu-id="748ca-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="748ca-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="748ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="748ca-120">Request headers</span></span>
| <span data-ttu-id="748ca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="748ca-121">Name</span></span>       | <span data-ttu-id="748ca-122">Тип</span><span class="sxs-lookup"><span data-stu-id="748ca-122">Type</span></span> | <span data-ttu-id="748ca-123">Описание</span><span class="sxs-lookup"><span data-stu-id="748ca-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="748ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="748ca-124">Authorization</span></span>  | <span data-ttu-id="748ca-125">string</span><span class="sxs-lookup"><span data-stu-id="748ca-125">string</span></span>  | <span data-ttu-id="748ca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="748ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="748ca-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="748ca-128">Request body</span></span>
<span data-ttu-id="748ca-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="748ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="748ca-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="748ca-130">Response</span></span>

<span data-ttu-id="748ca-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="748ca-131">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="748ca-132">Пример</span><span class="sxs-lookup"><span data-stu-id="748ca-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="748ca-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="748ca-133">Request</span></span>
<span data-ttu-id="748ca-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="748ca-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="748ca-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="748ca-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="748ca-136">C#</span><span class="sxs-lookup"><span data-stu-id="748ca-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="748ca-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="748ca-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="748ca-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="748ca-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="748ca-139">Java</span><span class="sxs-lookup"><span data-stu-id="748ca-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="748ca-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="748ca-140">Response</span></span>
<span data-ttu-id="748ca-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="748ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
