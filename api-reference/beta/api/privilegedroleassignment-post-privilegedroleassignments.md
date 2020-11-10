---
title: Создание privilegedRoleAssignment
description: Используйте этот API для создания нового Привилежедролеассигнмент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 3bb20ddcc8d1746ce1e567f6ce951d9e4c57ed62
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981977"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="ac099-103">Создание privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ac099-103">Create privilegedRoleAssignment</span></span>

<span data-ttu-id="ac099-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac099-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac099-105">Используйте этот API для создания нового  [привилежедролеассигнмент](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ac099-105">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ac099-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac099-106">Permissions</span></span>
<span data-ttu-id="ac099-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ac099-109">Запрашивающая сторона должна иметь _привилегированную роль администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="ac099-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="ac099-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac099-110">Permission type</span></span>      | <span data-ttu-id="ac099-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac099-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac099-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac099-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ac099-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac099-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac099-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac099-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac099-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac099-115">Not supported.</span></span>    |
|<span data-ttu-id="ac099-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac099-116">Application</span></span> | <span data-ttu-id="ac099-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac099-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac099-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac099-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="ac099-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac099-119">Request headers</span></span>
| <span data-ttu-id="ac099-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ac099-120">Name</span></span>       | <span data-ttu-id="ac099-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ac099-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ac099-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac099-122">Authorization</span></span>  | <span data-ttu-id="ac099-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac099-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac099-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac099-125">Request body</span></span>
<span data-ttu-id="ac099-126">В тексте запроса добавьте представление объекта [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac099-126">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ac099-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac099-127">Response</span></span>

<span data-ttu-id="ac099-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac099-128">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ac099-129">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="ac099-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ac099-130">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="ac099-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ac099-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ac099-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac099-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac099-132">Request</span></span>
<span data-ttu-id="ac099-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac099-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac099-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac099-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac099-135">C#</span><span class="sxs-lookup"><span data-stu-id="ac099-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac099-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac099-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac099-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac099-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac099-138">Java</span><span class="sxs-lookup"><span data-stu-id="ac099-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedroleassignment-from-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ac099-139">В тексте запроса добавьте представление объекта [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac099-139">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ac099-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac099-140">Response</span></span>
<span data-ttu-id="ac099-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac099-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


