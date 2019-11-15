---
title: Проверка групп элементов
description: Проверяет членство в указанном списке групп и возвращает из этого списка эти группы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 188ef3bfee8f8f0b57844d922a1e73596cbe9474
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657781"
---
# <a name="check-member-groups"></a><span data-ttu-id="dbc37-103">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="dbc37-103">Check member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbc37-104">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которые входит указанный пользователь, группа, субъект-служба или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="dbc37-104">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="dbc37-105">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="dbc37-105">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbc37-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbc37-106">Permissions</span></span>
<span data-ttu-id="dbc37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbc37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dbc37-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbc37-109">Permission type</span></span>      | <span data-ttu-id="dbc37-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbc37-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbc37-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbc37-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbc37-112">User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="dbc37-112">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="dbc37-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbc37-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbc37-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbc37-114">Not supported.</span></span>    |
|<span data-ttu-id="dbc37-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbc37-115">Application</span></span> | <span data-ttu-id="dbc37-116">User. Read. ALL и Граупмембер. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="dbc37-116">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="dbc37-117">Используйте приведенные ниже рекомендации по сценариям, чтобы определить, какие типы разрешений следует использовать:</span><span class="sxs-lookup"><span data-stu-id="dbc37-117">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="dbc37-118">Используйте User. Read и Граупмембер. Read. ALL или User. Read. ALL или User. Read и Group. Read. ALL для получения сведений о членстве в группах для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="dbc37-118">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="dbc37-119">Используйте User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL или User. Read. ALL и Group. Read. ALL, чтобы получить сведения о членстве в группах для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="dbc37-119">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="dbc37-120">Используйте Граупмембер. Read. ALL или Group. Read. ALL для получения сведений о членстве в группах для группы.</span><span class="sxs-lookup"><span data-stu-id="dbc37-120">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="dbc37-121">Используйте Application. ReadWrite. ALL и Граупмембер. Read. ALL или Application. ReadWrite. ALL и Group. Read. ALL для получения сведений о членстве в группах для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="dbc37-121">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="dbc37-122">Используйте разрешение Directory. Read. ALL для получения сведений о членстве в группах для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="dbc37-122">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="dbc37-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbc37-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servicePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="dbc37-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbc37-124">Request headers</span></span>
| <span data-ttu-id="dbc37-125">Имя</span><span class="sxs-lookup"><span data-stu-id="dbc37-125">Name</span></span>       | <span data-ttu-id="dbc37-126">Тип</span><span class="sxs-lookup"><span data-stu-id="dbc37-126">Type</span></span> | <span data-ttu-id="dbc37-127">Описание</span><span class="sxs-lookup"><span data-stu-id="dbc37-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbc37-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbc37-128">Authorization</span></span>  | <span data-ttu-id="dbc37-129">string</span><span class="sxs-lookup"><span data-stu-id="dbc37-129">string</span></span>  | <span data-ttu-id="dbc37-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbc37-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbc37-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbc37-132">Content-Type</span></span>  | <span data-ttu-id="dbc37-133">application/json</span><span class="sxs-lookup"><span data-stu-id="dbc37-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dbc37-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbc37-134">Request body</span></span>
<span data-ttu-id="dbc37-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dbc37-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbc37-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="dbc37-136">Parameter</span></span>    | <span data-ttu-id="dbc37-137">Тип</span><span class="sxs-lookup"><span data-stu-id="dbc37-137">Type</span></span>   |<span data-ttu-id="dbc37-138">Описание</span><span class="sxs-lookup"><span data-stu-id="dbc37-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbc37-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="dbc37-139">groupIds</span></span>|<span data-ttu-id="dbc37-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dbc37-140">String collection</span></span> |<span data-ttu-id="dbc37-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="dbc37-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="dbc37-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbc37-143">Response</span></span>

<span data-ttu-id="dbc37-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dbc37-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbc37-145">Пример</span><span class="sxs-lookup"><span data-stu-id="dbc37-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dbc37-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbc37-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dbc37-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbc37-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbc37-148">C#</span><span class="sxs-lookup"><span data-stu-id="dbc37-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbc37-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbc37-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbc37-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbc37-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dbc37-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbc37-151">Response</span></span>
<span data-ttu-id="dbc37-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbc37-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
