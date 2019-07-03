---
title: Создание объекта appRoleAssignment
description: Используйте этот API для создания нового Аппролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: 5f47d1d7809182f963469b02e6781462997e5d67
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457214"
---
# <a name="create-approleassignment"></a><span data-ttu-id="38968-103">Создание объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="38968-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38968-104">Используйте этот API для создания нового Аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="38968-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="38968-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38968-105">Permissions</span></span>
<span data-ttu-id="38968-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38968-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38968-108">Permission type</span></span>      | <span data-ttu-id="38968-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38968-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38968-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38968-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38968-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38968-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38968-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38968-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38968-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38968-113">Not supported.</span></span>    |
|<span data-ttu-id="38968-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38968-114">Application</span></span> | <span data-ttu-id="38968-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38968-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38968-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38968-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="38968-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38968-117">Request headers</span></span>
| <span data-ttu-id="38968-118">Имя</span><span class="sxs-lookup"><span data-stu-id="38968-118">Name</span></span>       | <span data-ttu-id="38968-119">Тип</span><span class="sxs-lookup"><span data-stu-id="38968-119">Type</span></span> | <span data-ttu-id="38968-120">Описание</span><span class="sxs-lookup"><span data-stu-id="38968-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38968-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38968-121">Authorization</span></span>  | <span data-ttu-id="38968-122">string</span><span class="sxs-lookup"><span data-stu-id="38968-122">string</span></span>  | <span data-ttu-id="38968-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38968-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38968-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38968-125">Request body</span></span>
<span data-ttu-id="38968-126">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38968-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="38968-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="38968-127">Response</span></span>

<span data-ttu-id="38968-128">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38968-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38968-129">Пример</span><span class="sxs-lookup"><span data-stu-id="38968-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38968-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="38968-130">Request</span></span>
<span data-ttu-id="38968-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38968-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="38968-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="38968-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="38968-133">C#</span><span class="sxs-lookup"><span data-stu-id="38968-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-approleassignment-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38968-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="38968-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-approleassignment-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38968-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="38968-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-approleassignment-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="38968-136">В тексте запроса добавьте представление объекта [аппролеассигнмент](../resources/approleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38968-136">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="38968-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="38968-137">Response</span></span>
<span data-ttu-id="38968-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38968-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
