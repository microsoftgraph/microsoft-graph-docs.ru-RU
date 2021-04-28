---
title: Вывод групп элементов
description: Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 399868d281b5e4a6eac7ead0ed31209236a26f7f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051489"
---
# <a name="get-member-groups"></a><span data-ttu-id="98e05-104">Вывод групп пользователя</span><span class="sxs-lookup"><span data-stu-id="98e05-104">Get member groups</span></span>

<span data-ttu-id="98e05-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98e05-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="98e05-p102">Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="98e05-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="98e05-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98e05-108">Permissions</span></span>
<span data-ttu-id="98e05-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98e05-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98e05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98e05-111">Permission type</span></span>      | <span data-ttu-id="98e05-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98e05-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98e05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98e05-113">Delegated (work or school account)</span></span> | <span data-ttu-id="98e05-114">User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All, User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="98e05-114">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="98e05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98e05-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98e05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98e05-116">Not supported.</span></span>    |
|<span data-ttu-id="98e05-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98e05-117">Application</span></span> | <span data-ttu-id="98e05-118">User.Read.All и GroupMember.Read.All, User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="98e05-118">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="98e05-119">Используйте руководство по следующим сценариям, чтобы определить, какие типы разрешений использовать:</span><span class="sxs-lookup"><span data-stu-id="98e05-119">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="98e05-120">Используйте разрешения User.Read и GroupMember.Read.All или User.Read и Group.Read.All для получения членства в группах для пользователя, вступив в группу.</span><span class="sxs-lookup"><span data-stu-id="98e05-120">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="98e05-121">Используйте user.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All или User.Read.All и Group.Read.All для получения членства в группе для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="98e05-121">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="98e05-122">Чтобы получить членство в группе, используйте разрешение GroupMember.Read.All или Group.Read.All.</span><span class="sxs-lookup"><span data-stu-id="98e05-122">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="98e05-123">Используйте разрешение Directory.Read.All для получения членства в группе для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="98e05-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>


## <a name="http-request"></a><span data-ttu-id="98e05-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98e05-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="98e05-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98e05-125">Request headers</span></span>
| <span data-ttu-id="98e05-126">Имя</span><span class="sxs-lookup"><span data-stu-id="98e05-126">Name</span></span>       | <span data-ttu-id="98e05-127">Тип</span><span class="sxs-lookup"><span data-stu-id="98e05-127">Type</span></span> | <span data-ttu-id="98e05-128">Описание</span><span class="sxs-lookup"><span data-stu-id="98e05-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="98e05-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="98e05-129">Authorization</span></span>  | <span data-ttu-id="98e05-130">string</span><span class="sxs-lookup"><span data-stu-id="98e05-130">string</span></span>  | <span data-ttu-id="98e05-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98e05-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98e05-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98e05-133">Content-Type</span></span>   | <span data-ttu-id="98e05-134">string</span><span class="sxs-lookup"><span data-stu-id="98e05-134">string</span></span>  | <span data-ttu-id="98e05-135">application/json</span><span class="sxs-lookup"><span data-stu-id="98e05-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98e05-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98e05-136">Request body</span></span>
<span data-ttu-id="98e05-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="98e05-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98e05-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="98e05-138">Parameter</span></span>    | <span data-ttu-id="98e05-139">Тип</span><span class="sxs-lookup"><span data-stu-id="98e05-139">Type</span></span>   |<span data-ttu-id="98e05-140">Описание</span><span class="sxs-lookup"><span data-stu-id="98e05-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98e05-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="98e05-141">securityEnabledOnly</span></span>|<span data-ttu-id="98e05-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="98e05-142">Boolean</span></span>| <span data-ttu-id="98e05-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="98e05-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="98e05-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="98e05-145">Response</span></span>

<span data-ttu-id="98e05-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98e05-146">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98e05-147">Пример</span><span class="sxs-lookup"><span data-stu-id="98e05-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98e05-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="98e05-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="98e05-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="98e05-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="98e05-150">C#</span><span class="sxs-lookup"><span data-stu-id="98e05-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98e05-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98e05-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98e05-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98e05-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98e05-153">Java</span><span class="sxs-lookup"><span data-stu-id="98e05-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98e05-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="98e05-154">Response</span></span>
<span data-ttu-id="98e05-155">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="98e05-155">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

