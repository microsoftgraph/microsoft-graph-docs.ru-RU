---
title: Создание объекта appRoleAssignment
description: Используйте этот API для создания нового Аппролеассигнмент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 71148acc2c62572a2f6c7e9f711e3660d5d523ad
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219034"
---
# <a name="create-approleassignment"></a><span data-ttu-id="089a0-103">Создание объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="089a0-103">Create appRoleAssignment</span></span>

<span data-ttu-id="089a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="089a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="089a0-105">Используйте этот API для создания нового Аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="089a0-105">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="089a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="089a0-106">Permissions</span></span>
<span data-ttu-id="089a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="089a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="089a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="089a0-109">Permission type</span></span>      | <span data-ttu-id="089a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="089a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="089a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="089a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="089a0-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="089a0-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="089a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="089a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="089a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="089a0-114">Not supported.</span></span>    |
|<span data-ttu-id="089a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="089a0-115">Application</span></span> | <span data-ttu-id="089a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="089a0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="089a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="089a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="089a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="089a0-118">Request headers</span></span>
| <span data-ttu-id="089a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="089a0-119">Name</span></span>       | <span data-ttu-id="089a0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="089a0-120">Type</span></span> | <span data-ttu-id="089a0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="089a0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="089a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="089a0-122">Authorization</span></span>  | <span data-ttu-id="089a0-123">string</span><span class="sxs-lookup"><span data-stu-id="089a0-123">string</span></span>  | <span data-ttu-id="089a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="089a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="089a0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="089a0-126">Request body</span></span>
<span data-ttu-id="089a0-127">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="089a0-127">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="089a0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="089a0-128">Response</span></span>

<span data-ttu-id="089a0-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="089a0-129">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="089a0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="089a0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="089a0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="089a0-131">Request</span></span>
<span data-ttu-id="089a0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="089a0-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="089a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="089a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="089a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="089a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-approleassignment-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="089a0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="089a0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-approleassignment-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="089a0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="089a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-approleassignment-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="089a0-137">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="089a0-137">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="089a0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="089a0-138">Response</span></span>
<span data-ttu-id="089a0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="089a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
