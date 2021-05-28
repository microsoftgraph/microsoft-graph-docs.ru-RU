---
title: Добавление участника
description: Добавление члена в группу Microsoft 365 или группу безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **members**.
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a9337c18b25e37711e9e7d9ec14d9ee65eccac39
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681979"
---
# <a name="add-member"></a><span data-ttu-id="a5b92-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="a5b92-103">Add member</span></span>

<span data-ttu-id="a5b92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5b92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5b92-105">Добавляйте участника в группу Microsoft 365 или группу безопасности через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="a5b92-105">Add a member to a Microsoft 365 group or a security group through the **members** navigation property.</span></span>

<span data-ttu-id="a5b92-106">Вы можете добавлять пользователей, контакты организации, cубъект-службы или другие группы.</span><span class="sxs-lookup"><span data-stu-id="a5b92-106">You can add users, organizational contacts, service principals or other groups.</span></span> 

> [!IMPORTANT]
> + <span data-ttu-id="a5b92-107">Вы можете добавлять пользователей только в группы безопасности и группы Microsoft 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="a5b92-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>
> + <span data-ttu-id="a5b92-108">Вы не можете добавлять группы безопасности в группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a5b92-108">You cannot add security groups to Microsoft 365 groups.</span></span>
> + <span data-ttu-id="a5b92-109">Вы не можете добавлять группы Microsoft 365 в группы безопасности или другие группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a5b92-109">You cannot add Microsoft 365 groups to security groups or other Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5b92-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5b92-110">Permissions</span></span>

<span data-ttu-id="a5b92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5b92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5b92-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5b92-113">Permission type</span></span>      | <span data-ttu-id="a5b92-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5b92-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5b92-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5b92-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a5b92-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5b92-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5b92-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5b92-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5b92-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5b92-118">Not supported.</span></span>    |
|<span data-ttu-id="a5b92-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a5b92-119">Application</span></span> | <span data-ttu-id="a5b92-120">GroupMember.ReadWrite.All, Group.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b92-120">GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5b92-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5b92-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a5b92-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5b92-122">Request headers</span></span>

| <span data-ttu-id="a5b92-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5b92-123">Header</span></span>       | <span data-ttu-id="a5b92-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a5b92-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a5b92-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5b92-125">Authorization</span></span>  | <span data-ttu-id="a5b92-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5b92-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5b92-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5b92-128">Content-type</span></span>   | <span data-ttu-id="a5b92-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5b92-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5b92-131">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5b92-131">Request body</span></span>

<span data-ttu-id="a5b92-132">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) или [organizational contact](../resources/orgcontact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5b92-132">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md), or [organizational contact](../resources/orgcontact.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a5b92-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5b92-133">Response</span></span>

<span data-ttu-id="a5b92-134">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5b92-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="a5b92-135">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5b92-135">It does not return anything in the response body.</span></span> <span data-ttu-id="a5b92-136">Если объект уже является членом группы, этот метод возвращает код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="a5b92-136">This method returns a `400 Bad Request` response code when the object is already a member of the group.</span></span> <span data-ttu-id="a5b92-137">Если добавляемый объект не существует, этот метод возвращает код отклика `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="a5b92-137">This method returns a `404 Not Found` response code when the object being added doesn't exist.</span></span>

## <a name="examples"></a><span data-ttu-id="a5b92-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5b92-138">Examples</span></span>

### <a name="example-1-add-a-member-to-a-group"></a><span data-ttu-id="a5b92-139">Пример 1. Добавление участника группы</span><span class="sxs-lookup"><span data-stu-id="a5b92-139">Example 1: Add a member to a group</span></span>

#### <a name="request"></a><span data-ttu-id="a5b92-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5b92-140">Request</span></span>

<span data-ttu-id="a5b92-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5b92-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5b92-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5b92-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a5b92-143">C#</span><span class="sxs-lookup"><span data-stu-id="a5b92-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5b92-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5b92-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5b92-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5b92-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5b92-146">Java</span><span class="sxs-lookup"><span data-stu-id="a5b92-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a5b92-147">Укажите в тексте запроса свойство добавляемого объекта идентификатор directoryObject, user или group, представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5b92-147">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="a5b92-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5b92-148">Response</span></span>

<span data-ttu-id="a5b92-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5b92-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a><span data-ttu-id="a5b92-150">Пример 2. Добавление нескольких участников в группу одним запросом</span><span class="sxs-lookup"><span data-stu-id="a5b92-150">Example 2: Add multiple members to a group in a single request</span></span>

<span data-ttu-id="a5b92-151">В этом примере показано, как добавить нескольких участников в группу с поддержкой с привязкой к ОData в операции PATCH.</span><span class="sxs-lookup"><span data-stu-id="a5b92-151">This example shows how to add multiple members to a group with OData bind support in a PATCH operation.</span></span> <span data-ttu-id="a5b92-152">Обратите внимание, что одним запросом можно добавить до 20 участников.</span><span class="sxs-lookup"><span data-stu-id="a5b92-152">Note that up to 20 members can be added in a single request.</span></span> <span data-ttu-id="a5b92-153">Операция POST не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5b92-153">The POST operation is not supported.</span></span> <span data-ttu-id="a5b92-154">Если в тексте запроса существует условие ошибки, элементы не добавляются и возвращается соответствующий код отклика.</span><span class="sxs-lookup"><span data-stu-id="a5b92-154">If an error condition exists in the request body, no members are added and the appropriate response code is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="a5b92-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5b92-155">Request</span></span>

<span data-ttu-id="a5b92-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5b92-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5b92-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5b92-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a5b92-158">C#</span><span class="sxs-lookup"><span data-stu-id="a5b92-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5b92-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5b92-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5b92-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5b92-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5b92-161">Java</span><span class="sxs-lookup"><span data-stu-id="a5b92-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a5b92-162">Укажите в тексте запроса свойство добавляемого объекта идентификатор directoryObject, user или group, представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5b92-162">In the request body, supply a JSON representation of the id of the directoryObject, user, or group object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="a5b92-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5b92-163">Response</span></span>
<span data-ttu-id="a5b92-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5b92-164">The following is an example of the response.</span></span>

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

