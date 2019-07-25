---
title: Создание privilegedRoleAssignment
description: Используйте этот API для создания нового Привилежедролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: 2e0f77b74825ebacedc5647524f38ba32ef14d62
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875636"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="a0f00-103">Создание privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a0f00-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0f00-104">Используйте этот API для создания нового [привилежедролеассигнмент](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0f00-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a0f00-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0f00-105">Permissions</span></span>
<span data-ttu-id="a0f00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a0f00-108">Запрашивающая сторона должна иметь привилегированную роль _администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="a0f00-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="a0f00-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0f00-109">Permission type</span></span>      | <span data-ttu-id="a0f00-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0f00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0f00-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0f00-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a0f00-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0f00-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0f00-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0f00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0f00-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0f00-114">Not supported.</span></span>    |
|<span data-ttu-id="a0f00-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0f00-115">Application</span></span> | <span data-ttu-id="a0f00-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0f00-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0f00-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0f00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="a0f00-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0f00-118">Request headers</span></span>
| <span data-ttu-id="a0f00-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a0f00-119">Name</span></span>       | <span data-ttu-id="a0f00-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a0f00-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a0f00-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0f00-121">Authorization</span></span>  | <span data-ttu-id="a0f00-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0f00-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0f00-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0f00-124">Request body</span></span>
<span data-ttu-id="a0f00-125">В тексте запроса добавьте представление объекта [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0f00-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0f00-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0f00-126">Response</span></span>

<span data-ttu-id="a0f00-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0f00-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="a0f00-128">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="a0f00-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a0f00-129">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="a0f00-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a0f00-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a0f00-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0f00-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0f00-131">Request</span></span>
<span data-ttu-id="a0f00-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0f00-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a0f00-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0f00-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0f00-134">C#</span><span class="sxs-lookup"><span data-stu-id="a0f00-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0f00-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a0f00-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a0f00-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a0f00-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a0f00-137">Java</span><span class="sxs-lookup"><span data-stu-id="a0f00-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedroleassignment-from-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a0f00-138">В тексте запроса добавьте представление объекта [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0f00-138">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a0f00-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0f00-139">Response</span></span>
<span data-ttu-id="a0f00-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0f00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
