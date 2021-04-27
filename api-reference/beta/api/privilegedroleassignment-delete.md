---
title: Удаление privilegedRoleAssignment
description: Удаление privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a28842b23825db7b010e2d597d592f1fd5ec5db2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055241"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="3ce4c-103">Удаление privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3ce4c-103">Delete privilegedRoleAssignment</span></span>

<span data-ttu-id="3ce4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ce4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ce4c-105">Удаление [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3ce4c-105">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3ce4c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ce4c-106">Permissions</span></span>
<span data-ttu-id="3ce4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ce4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3ce4c-109">Запросчику должна быть роль _администратора привилегированных_ ролей.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="3ce4c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ce4c-110">Permission type</span></span>      | <span data-ttu-id="3ce4c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ce4c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ce4c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ce4c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ce4c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ce4c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ce4c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ce4c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ce4c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-115">Not supported.</span></span>    |
|<span data-ttu-id="3ce4c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ce4c-116">Application</span></span> | <span data-ttu-id="3ce4c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ce4c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ce4c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="3ce4c-119">Обратите внимание, что в формате "userId_roleId", где userId — это строка GUID для пользовательского id Azure AD, а roleId — это строка GUID для id роли администратора ``{id}`` Azure.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-119">Note that ``{id}`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ce4c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ce4c-120">Request headers</span></span>
| <span data-ttu-id="3ce4c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3ce4c-121">Name</span></span>       | <span data-ttu-id="3ce4c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3ce4c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ce4c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ce4c-123">Authorization</span></span>  | <span data-ttu-id="3ce4c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ce4c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ce4c-126">Request body</span></span>
<span data-ttu-id="3ce4c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ce4c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ce4c-128">Response</span></span>

<span data-ttu-id="3ce4c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="3ce4c-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3ce4c-132">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="3ce4c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3ce4c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ce4c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ce4c-134">Request</span></span>
<span data-ttu-id="3ce4c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ce4c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ce4c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="3ce4c-137">C#</span><span class="sxs-lookup"><span data-stu-id="3ce4c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ce4c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ce4c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ce4c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ce4c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ce4c-140">Java</span><span class="sxs-lookup"><span data-stu-id="3ce4c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-privilegedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3ce4c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ce4c-141">Response</span></span>
<span data-ttu-id="3ce4c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-142">Here is an example of the response.</span></span> <span data-ttu-id="3ce4c-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3ce4c-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


