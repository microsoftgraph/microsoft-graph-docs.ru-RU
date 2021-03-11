---
title: Удаление пользователя — API Microsoft Graph
description: Описан метод удаления ресурса (объекта) user из API Microsoft Graph (REST).
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 705899489cb754fac5bbaac17fb75417195a484f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721770"
---
# <a name="delete-a-user"></a><span data-ttu-id="6365c-103">Удалить пользователя</span><span class="sxs-lookup"><span data-stu-id="6365c-103">Delete a user</span></span>

<span data-ttu-id="6365c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6365c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6365c-105">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="6365c-105">Delete user.</span></span>  

<span data-ttu-id="6365c-106">При удалении ресурсы user перемещаются во временный контейнер, и их можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="6365c-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="6365c-107">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="6365c-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="6365c-108">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="6365c-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6365c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6365c-109">Permissions</span></span>

<span data-ttu-id="6365c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6365c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6365c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6365c-112">Permission type</span></span>      | <span data-ttu-id="6365c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6365c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6365c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6365c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6365c-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6365c-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6365c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6365c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6365c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6365c-117">Not supported.</span></span>    |
|<span data-ttu-id="6365c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6365c-118">Application</span></span> | <span data-ttu-id="6365c-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6365c-119">User.ReadWrite.All</span></span> |

<span data-ttu-id="6365c-120">Рабочая или учебная учетная запись должна использоваться в одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="6365c-120">The work or school account must be in one of the following roles:</span></span>
+ <span data-ttu-id="6365c-121">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6365c-121">Global Administrator</span></span>
+ <span data-ttu-id="6365c-122">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="6365c-122">User Administrator</span></span>

<span data-ttu-id="6365c-123">Только глобальный администратор может удалить пользователя в роли глобального администратора или _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6365c-123">Only a Global Administrator can delete a user in a Global Administrator role or _any_ user in the tenant.</span></span> <span data-ttu-id="6365c-124">Администратор пользователей может удалять только тех пользователей, которые не являются администраторами, или пользователей в роли с ограниченными правами.</span><span class="sxs-lookup"><span data-stu-id="6365c-124">A User Administrator can only delete users who are non-administrators or in specific limited roles.</span></span> <span data-ttu-id="6365c-125">Дополнительные сведения см. в разделе [Разрешения для роли администратора в Azure AD](/azure/active-directory/roles/permissions-reference#available-roles)</span><span class="sxs-lookup"><span data-stu-id="6365c-125">For more details, see [Administrator role permissions in Azure AD](/azure/active-directory/roles/permissions-reference#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="6365c-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6365c-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="6365c-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6365c-127">Request headers</span></span>

| <span data-ttu-id="6365c-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6365c-128">Header</span></span>       | <span data-ttu-id="6365c-129">Значение</span><span class="sxs-lookup"><span data-stu-id="6365c-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6365c-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6365c-130">Authorization</span></span>  | <span data-ttu-id="6365c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6365c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6365c-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6365c-133">Request body</span></span>

<span data-ttu-id="6365c-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6365c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6365c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6365c-135">Response</span></span>

<span data-ttu-id="6365c-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6365c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6365c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6365c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6365c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6365c-139">Request</span></span>

<span data-ttu-id="6365c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6365c-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6365c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6365c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
# <a name="c"></a>[<span data-ttu-id="6365c-142">C#</span><span class="sxs-lookup"><span data-stu-id="6365c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6365c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6365c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6365c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6365c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6365c-145">Java</span><span class="sxs-lookup"><span data-stu-id="6365c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6365c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6365c-146">Response</span></span>

<span data-ttu-id="6365c-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6365c-147">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


