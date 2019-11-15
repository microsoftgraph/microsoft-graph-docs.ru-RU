---
title: Вывод групп элементов
description: Возврат всех групп, членом которых является указанный пользователь, группа, субъект или объект службы каталогов. Это транзитивная функция.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32b2aaee30e75db3bf383e6368764e476cfbcd33
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657774"
---
# <a name="get-member-groups"></a><span data-ttu-id="6d7c6-104">Вывод групп пользователя</span><span class="sxs-lookup"><span data-stu-id="6d7c6-104">Get member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d7c6-105">Возврат всех групп, членом которых является указанный пользователь, группа, субъект или объект службы каталогов.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-105">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="6d7c6-106">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d7c6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d7c6-107">Permissions</span></span>
<span data-ttu-id="6d7c6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d7c6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6d7c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d7c6-110">Permission type</span></span>      | <span data-ttu-id="6d7c6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d7c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d7c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d7c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d7c6-113">User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6d7c6-113">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="6d7c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d7c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d7c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-115">Not supported.</span></span>    |
|<span data-ttu-id="6d7c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d7c6-116">Application</span></span> | <span data-ttu-id="6d7c6-117">User. Read. ALL и Граупмембер. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6d7c6-117">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="6d7c6-118">Используйте приведенные ниже рекомендации по сценариям, чтобы определить, какие типы разрешений следует использовать:</span><span class="sxs-lookup"><span data-stu-id="6d7c6-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="6d7c6-119">Используйте User. Read и Граупмембер. Read. ALL или User. Read. ALL или User. Read и Group. Read. ALL для получения сведений о членстве в группах для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-119">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="6d7c6-120">Используйте User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL или User. Read. ALL и Group. Read. ALL, чтобы получить сведения о членстве в группах для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-120">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="6d7c6-121">Используйте Граупмембер. Read. ALL или Group. Read. ALL для получения сведений о членстве в группах для группы.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-121">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="6d7c6-122">Используйте Application. ReadWrite. ALL и Граупмембер. Read. ALL или Application. ReadWrite. ALL и Group. Read. ALL для получения сведений о членстве в группах для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-122">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="6d7c6-123">Используйте разрешение Directory. Read. ALL для получения сведений о членстве в группах для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="6d7c6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d7c6-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="6d7c6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d7c6-125">Request headers</span></span>
| <span data-ttu-id="6d7c6-126">Имя</span><span class="sxs-lookup"><span data-stu-id="6d7c6-126">Name</span></span>       | <span data-ttu-id="6d7c6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6d7c6-127">Type</span></span> | <span data-ttu-id="6d7c6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6d7c6-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d7c6-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d7c6-129">Authorization</span></span>  | <span data-ttu-id="6d7c6-130">string</span><span class="sxs-lookup"><span data-stu-id="6d7c6-130">string</span></span>  | <span data-ttu-id="6d7c6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6d7c6-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d7c6-133">Content-Type</span></span>  | <span data-ttu-id="6d7c6-134">application/json</span><span class="sxs-lookup"><span data-stu-id="6d7c6-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d7c6-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d7c6-135">Request body</span></span>
<span data-ttu-id="6d7c6-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6d7c6-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="6d7c6-137">Parameter</span></span>    | <span data-ttu-id="6d7c6-138">Тип</span><span class="sxs-lookup"><span data-stu-id="6d7c6-138">Type</span></span>   |<span data-ttu-id="6d7c6-139">Описание</span><span class="sxs-lookup"><span data-stu-id="6d7c6-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d7c6-140">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6d7c6-140">securityEnabledOnly</span></span>|<span data-ttu-id="6d7c6-141">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d7c6-141">Boolean</span></span>| <span data-ttu-id="6d7c6-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="6d7c6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d7c6-144">Response</span></span>

<span data-ttu-id="6d7c6-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d7c6-146">Пример</span><span class="sxs-lookup"><span data-stu-id="6d7c6-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6d7c6-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d7c6-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d7c6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d7c6-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d7c6-149">C#</span><span class="sxs-lookup"><span data-stu-id="6d7c6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d7c6-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d7c6-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d7c6-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d7c6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d7c6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d7c6-152">Response</span></span>
<span data-ttu-id="6d7c6-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d7c6-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
