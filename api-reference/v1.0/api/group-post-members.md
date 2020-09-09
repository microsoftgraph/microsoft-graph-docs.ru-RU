---
title: Добавление участника
description: Добавление члена в группу безопасности Microsoft 365, группу безопасности или группу безопасности с включенной поддержкой почты с помощью свойства навигации **Members** .
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f3ad60b441bbccd5b71df0634033ee0a4eeae46e
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413359"
---
# <a name="add-member"></a><span data-ttu-id="74bf8-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="74bf8-103">Add member</span></span>

<span data-ttu-id="74bf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74bf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74bf8-105">Добавление члена в группу Microsoft 365 или группу безопасности с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="74bf8-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="74bf8-106">Вы можете добавлять пользователей, организационные контакты, субъекты служб или другие группы.</span><span class="sxs-lookup"><span data-stu-id="74bf8-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="74bf8-107">Вы можете добавлять пользователей только в группы безопасности и Microsoft 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="74bf8-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="74bf8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74bf8-108">Permissions</span></span>

<span data-ttu-id="74bf8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74bf8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74bf8-111">Permission type</span></span>      | <span data-ttu-id="74bf8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74bf8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74bf8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74bf8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="74bf8-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74bf8-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74bf8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74bf8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74bf8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74bf8-116">Not supported.</span></span>    |
|<span data-ttu-id="74bf8-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="74bf8-117">Application</span></span> | <span data-ttu-id="74bf8-118">GroupMember.ReadWrite.All, Group.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74bf8-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74bf8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74bf8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="74bf8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74bf8-120">Request headers</span></span>

| <span data-ttu-id="74bf8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74bf8-121">Header</span></span>       | <span data-ttu-id="74bf8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74bf8-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="74bf8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74bf8-123">Authorization</span></span>  | <span data-ttu-id="74bf8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74bf8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74bf8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74bf8-126">Content-type</span></span>   | <span data-ttu-id="74bf8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74bf8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74bf8-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="74bf8-129">Request body</span></span>

<span data-ttu-id="74bf8-130">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) или [organizational contact](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74bf8-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="74bf8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="74bf8-131">Response</span></span>

<span data-ttu-id="74bf8-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="74bf8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74bf8-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="74bf8-134">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="74bf8-135">Пример 1: Добавление участника в группу</span><span class="sxs-lookup"><span data-stu-id="74bf8-135">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="74bf8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="74bf8-136">Request</span></span>

<span data-ttu-id="74bf8-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74bf8-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="74bf8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="74bf8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_member_to_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{group-id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="74bf8-139">C#</span><span class="sxs-lookup"><span data-stu-id="74bf8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74bf8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74bf8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74bf8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74bf8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74bf8-142">Java</span><span class="sxs-lookup"><span data-stu-id="74bf8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="74bf8-143">В тексте запроса добавьте представление идентификатора объекта directoryObject, пользователя или группы, который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74bf8-143">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="74bf8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="74bf8-144">Response</span></span>

<span data-ttu-id="74bf8-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="74bf8-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="74bf8-146">Пример 2: Добавление нескольких участников в группу в едином запросе</span><span class="sxs-lookup"><span data-stu-id="74bf8-146">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="74bf8-147">В этом примере показано, как добавить несколько членов в группу с поддержкой BIND в операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="74bf8-147">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="74bf8-148">Обратите внимание, что в один запрос можно добавить до 20 участников.</span><span class="sxs-lookup"><span data-stu-id="74bf8-148">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="74bf8-149">Операция POST не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74bf8-149">The POST operation is not supported.</span></span>

#### <a name="request"></a><span data-ttu-id="74bf8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="74bf8-150">Request</span></span>

<span data-ttu-id="74bf8-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74bf8-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="74bf8-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="74bf8-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_multiple_members_to_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{group-id}
Content-type: application/json
Content-length: 30

{
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="74bf8-153">C#</span><span class="sxs-lookup"><span data-stu-id="74bf8-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74bf8-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74bf8-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74bf8-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74bf8-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74bf8-156">Java</span><span class="sxs-lookup"><span data-stu-id="74bf8-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="74bf8-157">В тексте запроса добавьте представление идентификатора объекта directoryObject, пользователя или группы, который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74bf8-157">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="74bf8-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="74bf8-158">Response</span></span>
<span data-ttu-id="74bf8-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="74bf8-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
