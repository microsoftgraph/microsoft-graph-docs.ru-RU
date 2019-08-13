---
title: Создание объекта appRoleAssignment
description: Используйте этот API для создания нового Аппролеассигнмент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5e78229f1e23afc185def38e4dc2b615e2714dbc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363916"
---
# <a name="create-approleassignment"></a><span data-ttu-id="4919e-103">Создание объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4919e-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4919e-104">Используйте этот API для создания нового Аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="4919e-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4919e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4919e-105">Permissions</span></span>
<span data-ttu-id="4919e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4919e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4919e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4919e-108">Permission type</span></span>      | <span data-ttu-id="4919e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4919e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4919e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4919e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4919e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4919e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4919e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4919e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4919e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4919e-113">Not supported.</span></span>    |
|<span data-ttu-id="4919e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4919e-114">Application</span></span> | <span data-ttu-id="4919e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4919e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4919e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4919e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="4919e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4919e-117">Request headers</span></span>
| <span data-ttu-id="4919e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4919e-118">Name</span></span>       | <span data-ttu-id="4919e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4919e-119">Type</span></span> | <span data-ttu-id="4919e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4919e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4919e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4919e-121">Authorization</span></span>  | <span data-ttu-id="4919e-122">string</span><span class="sxs-lookup"><span data-stu-id="4919e-122">string</span></span>  | <span data-ttu-id="4919e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4919e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4919e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4919e-125">Request body</span></span>
<span data-ttu-id="4919e-126">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4919e-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4919e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4919e-127">Response</span></span>

<span data-ttu-id="4919e-128">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4919e-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4919e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4919e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4919e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4919e-130">Request</span></span>
<span data-ttu-id="4919e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4919e-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4919e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4919e-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4919e-133">C#</span><span class="sxs-lookup"><span data-stu-id="4919e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-approleassignment-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4919e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4919e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-approleassignment-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4919e-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4919e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-approleassignment-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4919e-136">Java</span><span class="sxs-lookup"><span data-stu-id="4919e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-approleassignment-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4919e-137">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4919e-137">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4919e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4919e-138">Response</span></span>
<span data-ttu-id="4919e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4919e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
