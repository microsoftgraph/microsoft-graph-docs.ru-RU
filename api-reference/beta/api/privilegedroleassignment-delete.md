---
title: Удаление privilegedRoleAssignment
description: Удаление Привилежедролеассигнмент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e5940dd45d318d2537bf00f647779381ad53b2a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455391"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="3117b-103">Удаление privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3117b-103">Delete privilegedRoleAssignment</span></span>

<span data-ttu-id="3117b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3117b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3117b-105">Удаление [привилежедролеассигнмент](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3117b-105">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3117b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3117b-106">Permissions</span></span>
<span data-ttu-id="3117b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3117b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3117b-109">Запрашивающая сторона должна иметь _привилегированную роль администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="3117b-109">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="3117b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3117b-110">Permission type</span></span>      | <span data-ttu-id="3117b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3117b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3117b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3117b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3117b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3117b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3117b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3117b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3117b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3117b-115">Not supported.</span></span>    |
|<span data-ttu-id="3117b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3117b-116">Application</span></span> | <span data-ttu-id="3117b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3117b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3117b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3117b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="3117b-119">Обратите ``{id}`` внимание, что используется формат "userId_roleId", где UserID — это строка GUID для идентификатора пользователя Azure AD, а roleId — строка GUID для идентификатора роли администратора Azure.</span><span class="sxs-lookup"><span data-stu-id="3117b-119">Note that ``{id}`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3117b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3117b-120">Request headers</span></span>
| <span data-ttu-id="3117b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3117b-121">Name</span></span>       | <span data-ttu-id="3117b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3117b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3117b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3117b-123">Authorization</span></span>  | <span data-ttu-id="3117b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3117b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3117b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3117b-126">Request body</span></span>
<span data-ttu-id="3117b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3117b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3117b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3117b-128">Response</span></span>

<span data-ttu-id="3117b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3117b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="3117b-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="3117b-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3117b-132">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="3117b-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="3117b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3117b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3117b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3117b-134">Request</span></span>
<span data-ttu-id="3117b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3117b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3117b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3117b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="3117b-137">C#</span><span class="sxs-lookup"><span data-stu-id="3117b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3117b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3117b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3117b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3117b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3117b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3117b-140">Response</span></span>
<span data-ttu-id="3117b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3117b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
