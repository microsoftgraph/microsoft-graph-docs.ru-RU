---
title: Получение directoryRole
description: Получение свойств объекта directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87c781f0f7edefbebc525d4b461ec3422bc002c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434499"
---
# <a name="get-directoryrole"></a><span data-ttu-id="ec9d5-103">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="ec9d5-103">Get directoryRole</span></span>

<span data-ttu-id="ec9d5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ec9d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec9d5-105">Получение свойств объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="ec9d5-105">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec9d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec9d5-106">Permissions</span></span>
<span data-ttu-id="ec9d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec9d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec9d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec9d5-109">Permission type</span></span>      | <span data-ttu-id="ec9d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec9d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec9d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec9d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ec9d5-112">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ec9d5-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec9d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec9d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec9d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec9d5-114">Not supported.</span></span>    |
|<span data-ttu-id="ec9d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec9d5-115">Application</span></span> | <span data-ttu-id="ec9d5-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ec9d5-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec9d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec9d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec9d5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec9d5-118">Optional query parameters</span></span>
<span data-ttu-id="ec9d5-119">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="ec9d5-119">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec9d5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec9d5-120">Request headers</span></span>
| <span data-ttu-id="ec9d5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ec9d5-121">Name</span></span>       | <span data-ttu-id="ec9d5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ec9d5-122">Type</span></span> | <span data-ttu-id="ec9d5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ec9d5-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ec9d5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec9d5-124">Authorization</span></span>  | <span data-ttu-id="ec9d5-125">string</span><span class="sxs-lookup"><span data-stu-id="ec9d5-125">string</span></span>  | <span data-ttu-id="ec9d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec9d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec9d5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec9d5-128">Request body</span></span>
<span data-ttu-id="ec9d5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec9d5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec9d5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec9d5-130">Response</span></span>

<span data-ttu-id="ec9d5-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec9d5-131">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec9d5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ec9d5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec9d5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec9d5-133">Request</span></span>
<span data-ttu-id="ec9d5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec9d5-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec9d5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec9d5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="ec9d5-136">C#</span><span class="sxs-lookup"><span data-stu-id="ec9d5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec9d5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec9d5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec9d5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec9d5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec9d5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec9d5-139">Response</span></span>
<span data-ttu-id="ec9d5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec9d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
