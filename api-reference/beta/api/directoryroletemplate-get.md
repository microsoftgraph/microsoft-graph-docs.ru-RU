---
title: Вывод объекта directoryRoleTemplate
description: Получение свойств и связей объекта directoryRoleTemplate.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 378795707b0cdcff9b2bb1c45d257078b68189e3
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312864"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="178ac-103">Вывод объекта directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="178ac-103">Get directoryRoleTemplate</span></span>

<span data-ttu-id="178ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="178ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="178ac-105">Получение свойств и связей объекта directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="178ac-105">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="178ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="178ac-106">Permissions</span></span>
<span data-ttu-id="178ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="178ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="178ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="178ac-109">Permission type</span></span>      | <span data-ttu-id="178ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="178ac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="178ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="178ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="178ac-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="178ac-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="178ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="178ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="178ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="178ac-114">Not supported.</span></span>    |
|<span data-ttu-id="178ac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="178ac-115">Application</span></span> | <span data-ttu-id="178ac-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="178ac-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="178ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="178ac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="178ac-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="178ac-118">Optional query parameters</span></span>
<span data-ttu-id="178ac-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="178ac-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="178ac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="178ac-120">Request headers</span></span>
| <span data-ttu-id="178ac-121">Имя</span><span class="sxs-lookup"><span data-stu-id="178ac-121">Name</span></span>       | <span data-ttu-id="178ac-122">Тип</span><span class="sxs-lookup"><span data-stu-id="178ac-122">Type</span></span> | <span data-ttu-id="178ac-123">Описание</span><span class="sxs-lookup"><span data-stu-id="178ac-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="178ac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="178ac-124">Authorization</span></span>  | <span data-ttu-id="178ac-125">string</span><span class="sxs-lookup"><span data-stu-id="178ac-125">string</span></span>  | <span data-ttu-id="178ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="178ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="178ac-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="178ac-128">Request body</span></span>
<span data-ttu-id="178ac-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="178ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="178ac-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="178ac-130">Response</span></span>

<span data-ttu-id="178ac-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRoleTemplate](../resources/directoryroletemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="178ac-131">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="178ac-132">Пример</span><span class="sxs-lookup"><span data-stu-id="178ac-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="178ac-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="178ac-133">Request</span></span>
<span data-ttu-id="178ac-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="178ac-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="178ac-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="178ac-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="178ac-136">C#</span><span class="sxs-lookup"><span data-stu-id="178ac-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="178ac-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="178ac-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="178ac-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="178ac-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="178ac-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="178ac-139">Response</span></span>
<span data-ttu-id="178ac-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="178ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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