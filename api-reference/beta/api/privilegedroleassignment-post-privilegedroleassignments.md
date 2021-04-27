---
title: Создание privilegedRoleAssignment
description: Используйте этот API для создания нового привилегированного API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: ae11f0c21a4dcb314d12f4b74e570ea4cafc03a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052903"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="20f54-103">Создание privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="20f54-103">Create privilegedRoleAssignment</span></span>

<span data-ttu-id="20f54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20f54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20f54-105">Используйте этот API для создания нового [привилегированного API.](../resources/privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="20f54-105">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="20f54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20f54-106">Permissions</span></span>
<span data-ttu-id="20f54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20f54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="20f54-109">Запросчику должна быть роль _администратора привилегированных_ ролей.</span><span class="sxs-lookup"><span data-stu-id="20f54-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="20f54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20f54-110">Permission type</span></span>      | <span data-ttu-id="20f54-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20f54-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20f54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20f54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20f54-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20f54-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20f54-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20f54-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20f54-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20f54-115">Not supported.</span></span>    |
|<span data-ttu-id="20f54-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20f54-116">Application</span></span> | <span data-ttu-id="20f54-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20f54-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20f54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20f54-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="20f54-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20f54-119">Request headers</span></span>
| <span data-ttu-id="20f54-120">Имя</span><span class="sxs-lookup"><span data-stu-id="20f54-120">Name</span></span>       | <span data-ttu-id="20f54-121">Описание</span><span class="sxs-lookup"><span data-stu-id="20f54-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20f54-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20f54-122">Authorization</span></span>  | <span data-ttu-id="20f54-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20f54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20f54-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20f54-125">Request body</span></span>
<span data-ttu-id="20f54-126">В теле запроса поставляем представление JSON объекта [privilegedRoleAssignment.](../resources/privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="20f54-126">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="20f54-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="20f54-127">Response</span></span>

<span data-ttu-id="20f54-128">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="20f54-128">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="20f54-129">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="20f54-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="20f54-130">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="20f54-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="20f54-131">Пример</span><span class="sxs-lookup"><span data-stu-id="20f54-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20f54-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="20f54-132">Request</span></span>
<span data-ttu-id="20f54-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20f54-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20f54-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="20f54-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="20f54-135">C#</span><span class="sxs-lookup"><span data-stu-id="20f54-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20f54-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20f54-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20f54-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20f54-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20f54-138">Java</span><span class="sxs-lookup"><span data-stu-id="20f54-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedroleassignment-from-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="20f54-139">В теле запроса поставляем представление JSON объекта [privilegedRoleAssignment.](../resources/privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="20f54-139">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="20f54-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="20f54-140">Response</span></span>
<span data-ttu-id="20f54-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20f54-141">Here is an example of the response.</span></span> <span data-ttu-id="20f54-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="20f54-142">Note: The response object shown here might be shortened for readability.</span></span>
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


