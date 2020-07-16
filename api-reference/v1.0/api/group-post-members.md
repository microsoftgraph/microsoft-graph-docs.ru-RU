---
title: Добавление участника
description: Добавление члена в группу безопасности Microsoft 365, группу безопасности или группу безопасности с включенной поддержкой почты с помощью свойства навигации **Members** .
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0388d13d0e50c6ffcc415503a75afb8af56fa14f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897150"
---
# <a name="add-member"></a><span data-ttu-id="f87f2-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="f87f2-103">Add member</span></span>

<span data-ttu-id="f87f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f87f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f87f2-105">Добавление члена в группу Microsoft 365 или группу безопасности с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="f87f2-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="f87f2-106">Вы можете добавлять пользователей, организационные контакты, субъекты служб или другие группы.</span><span class="sxs-lookup"><span data-stu-id="f87f2-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="f87f2-107">Вы можете добавлять пользователей только в группы безопасности и Microsoft 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="f87f2-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="f87f2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f87f2-108">Permissions</span></span>
<span data-ttu-id="f87f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f87f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f87f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f87f2-111">Permission type</span></span>      | <span data-ttu-id="f87f2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f87f2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f87f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f87f2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f87f2-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f87f2-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f87f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f87f2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f87f2-116">Not supported.</span></span>    |
|<span data-ttu-id="f87f2-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f87f2-117">Application</span></span> | <span data-ttu-id="f87f2-118">GroupMember.ReadWrite.All, Group.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f87f2-118">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f87f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f87f2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f87f2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f87f2-120">Request headers</span></span>
| <span data-ttu-id="f87f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f87f2-121">Header</span></span>       | <span data-ttu-id="f87f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f87f2-122">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f87f2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f87f2-123">Authorization</span></span>  | <span data-ttu-id="f87f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f87f2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f87f2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f87f2-126">Content-type</span></span>   | <span data-ttu-id="f87f2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f87f2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f87f2-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="f87f2-129">Request body</span></span>
<span data-ttu-id="f87f2-130">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) или [organizational contact](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f87f2-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f87f2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f87f2-131">Response</span></span>
<span data-ttu-id="f87f2-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f87f2-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f87f2-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="f87f2-134">Examples</span></span>
### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="f87f2-135">Пример 1: Добавление участника в группу</span><span class="sxs-lookup"><span data-stu-id="f87f2-135">Example 1: Add a member to a group</span></span>
#### <a name="request"></a><span data-ttu-id="f87f2-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f87f2-136">Request</span></span>
<span data-ttu-id="f87f2-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f87f2-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f87f2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f87f2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="f87f2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f87f2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f87f2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f87f2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f87f2-141">C#</span><span class="sxs-lookup"><span data-stu-id="f87f2-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f87f2-142">Java</span><span class="sxs-lookup"><span data-stu-id="f87f2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f87f2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f87f2-143">Response</span></span>
<span data-ttu-id="f87f2-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f87f2-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="f87f2-145">Пример 2: Добавление нескольких участников в группу в едином запросе</span><span class="sxs-lookup"><span data-stu-id="f87f2-145">Example 2: Add multiple members to a group in a single request</span></span>
<span data-ttu-id="f87f2-146">В этом примере показано, как добавить несколько членов в группу с поддержкой BIND в операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="f87f2-146">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="f87f2-147">Обратите внимание, что в один запрос можно добавить до 20 участников.</span><span class="sxs-lookup"><span data-stu-id="f87f2-147">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="f87f2-148">Операция POST не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f87f2-148">The POST operation is not supported.</span></span>
#### <a name="request"></a><span data-ttu-id="f87f2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f87f2-149">Request</span></span>
<span data-ttu-id="f87f2-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f87f2-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f87f2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="f87f2-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_member_from_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
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
# <a name="javascript"></a>[<span data-ttu-id="f87f2-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f87f2-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f87f2-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f87f2-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f87f2-154">C#</span><span class="sxs-lookup"><span data-stu-id="f87f2-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f87f2-155">Java</span><span class="sxs-lookup"><span data-stu-id="f87f2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f87f2-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f87f2-156">Response</span></span>
<span data-ttu-id="f87f2-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f87f2-157">The following is an example of the response.</span></span>

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
