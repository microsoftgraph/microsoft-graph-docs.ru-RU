---
title: Вывод групп элементов
description: Возврат всех групп, членом которых является указанный пользователь, группа, субъект или объект службы каталогов. Это транзитивная функция.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 55c065ccaf468104405120ca30ee632e3c18c031
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434681"
---
# <a name="get-member-groups"></a><span data-ttu-id="72a4e-104">Вывод групп пользователя</span><span class="sxs-lookup"><span data-stu-id="72a4e-104">Get member groups</span></span>

<span data-ttu-id="72a4e-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72a4e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72a4e-106">Возврат всех групп, членом которых является указанный пользователь, группа, субъект или объект службы каталогов.</span><span class="sxs-lookup"><span data-stu-id="72a4e-106">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="72a4e-107">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="72a4e-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="72a4e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72a4e-108">Permissions</span></span>
<span data-ttu-id="72a4e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72a4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="72a4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72a4e-111">Permission type</span></span>      | <span data-ttu-id="72a4e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72a4e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72a4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72a4e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="72a4e-114">User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="72a4e-114">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="72a4e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72a4e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72a4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a4e-116">Not supported.</span></span>    |
|<span data-ttu-id="72a4e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72a4e-117">Application</span></span> | <span data-ttu-id="72a4e-118">User. Read. ALL и Граупмембер. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="72a4e-118">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="72a4e-119">Используйте приведенные ниже рекомендации по сценариям, чтобы определить, какие типы разрешений следует использовать:</span><span class="sxs-lookup"><span data-stu-id="72a4e-119">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="72a4e-120">Используйте User. Read и Граупмембер. Read. ALL или User. Read. ALL или User. Read и Group. Read. ALL для получения сведений о членстве в группах для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="72a4e-120">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="72a4e-121">Используйте User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL или User. Read. ALL и Group. Read. ALL, чтобы получить сведения о членстве в группах для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="72a4e-121">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="72a4e-122">Используйте Граупмембер. Read. ALL или Group. Read. ALL для получения сведений о членстве в группах для группы.</span><span class="sxs-lookup"><span data-stu-id="72a4e-122">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="72a4e-123">Используйте Application. ReadWrite. ALL и Граупмембер. Read. ALL или Application. ReadWrite. ALL и Group. Read. ALL для получения сведений о членстве в группах для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="72a4e-123">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="72a4e-124">Используйте разрешение Directory. Read. ALL для получения сведений о членстве в группах для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="72a4e-124">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="72a4e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72a4e-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="72a4e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72a4e-126">Request headers</span></span>
| <span data-ttu-id="72a4e-127">Имя</span><span class="sxs-lookup"><span data-stu-id="72a4e-127">Name</span></span>       | <span data-ttu-id="72a4e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="72a4e-128">Type</span></span> | <span data-ttu-id="72a4e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="72a4e-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="72a4e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="72a4e-130">Authorization</span></span>  | <span data-ttu-id="72a4e-131">string</span><span class="sxs-lookup"><span data-stu-id="72a4e-131">string</span></span>  | <span data-ttu-id="72a4e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72a4e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72a4e-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72a4e-134">Content-Type</span></span>  | <span data-ttu-id="72a4e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="72a4e-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72a4e-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72a4e-136">Request body</span></span>
<span data-ttu-id="72a4e-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="72a4e-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="72a4e-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="72a4e-138">Parameter</span></span>    | <span data-ttu-id="72a4e-139">Тип</span><span class="sxs-lookup"><span data-stu-id="72a4e-139">Type</span></span>   |<span data-ttu-id="72a4e-140">Описание</span><span class="sxs-lookup"><span data-stu-id="72a4e-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72a4e-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="72a4e-141">securityEnabledOnly</span></span>|<span data-ttu-id="72a4e-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="72a4e-142">Boolean</span></span>| <span data-ttu-id="72a4e-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="72a4e-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="72a4e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a4e-145">Response</span></span>

<span data-ttu-id="72a4e-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72a4e-146">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72a4e-147">Пример</span><span class="sxs-lookup"><span data-stu-id="72a4e-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="72a4e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="72a4e-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="72a4e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="72a4e-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="72a4e-150">C#</span><span class="sxs-lookup"><span data-stu-id="72a4e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72a4e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72a4e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72a4e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72a4e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72a4e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a4e-153">Response</span></span>
<span data-ttu-id="72a4e-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72a4e-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
