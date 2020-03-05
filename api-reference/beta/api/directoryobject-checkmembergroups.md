---
title: Проверка групп элементов
description: Проверяет членство в указанном списке групп и возвращает из этого списка эти группы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2650bfb80fdb4da4b65afbd13566d3bde2b8c367
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435054"
---
# <a name="check-member-groups"></a><span data-ttu-id="becab-103">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="becab-103">Check member groups</span></span>

<span data-ttu-id="becab-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="becab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="becab-105">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которые входит указанный пользователь, группа, субъект-служба или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="becab-105">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="becab-106">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="becab-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="becab-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="becab-107">Permissions</span></span>
<span data-ttu-id="becab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="becab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="becab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="becab-110">Permission type</span></span>      | <span data-ttu-id="becab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="becab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="becab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="becab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="becab-113">User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="becab-113">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="becab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="becab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="becab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="becab-115">Not supported.</span></span>    |
|<span data-ttu-id="becab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="becab-116">Application</span></span> | <span data-ttu-id="becab-117">User. Read. ALL и Граупмембер. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="becab-117">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="becab-118">Используйте приведенные ниже рекомендации по сценариям, чтобы определить, какие типы разрешений следует использовать:</span><span class="sxs-lookup"><span data-stu-id="becab-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="becab-119">Используйте User. Read и Граупмембер. Read. ALL или User. Read. ALL или User. Read и Group. Read. ALL для получения сведений о членстве в группах для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="becab-119">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="becab-120">Используйте User. ReadBasic. ALL и Граупмембер. Read. ALL, User. Read. ALL и Граупмембер. Read. ALL, User. ReadBasic. ALL и Group. Read. ALL или User. Read. ALL и Group. Read. ALL, чтобы получить сведения о членстве в группах для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="becab-120">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="becab-121">Используйте Граупмембер. Read. ALL или Group. Read. ALL для получения сведений о членстве в группах для группы.</span><span class="sxs-lookup"><span data-stu-id="becab-121">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="becab-122">Используйте Application. ReadWrite. ALL и Граупмембер. Read. ALL или Application. ReadWrite. ALL и Group. Read. ALL для получения сведений о членстве в группах для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="becab-122">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="becab-123">Используйте разрешение Directory. Read. ALL для получения сведений о членстве в группах для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="becab-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="becab-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="becab-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servicePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="becab-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="becab-125">Request headers</span></span>
| <span data-ttu-id="becab-126">Имя</span><span class="sxs-lookup"><span data-stu-id="becab-126">Name</span></span>       | <span data-ttu-id="becab-127">Тип</span><span class="sxs-lookup"><span data-stu-id="becab-127">Type</span></span> | <span data-ttu-id="becab-128">Описание</span><span class="sxs-lookup"><span data-stu-id="becab-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="becab-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="becab-129">Authorization</span></span>  | <span data-ttu-id="becab-130">string</span><span class="sxs-lookup"><span data-stu-id="becab-130">string</span></span>  | <span data-ttu-id="becab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="becab-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="becab-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="becab-133">Content-Type</span></span>  | <span data-ttu-id="becab-134">application/json</span><span class="sxs-lookup"><span data-stu-id="becab-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="becab-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="becab-135">Request body</span></span>
<span data-ttu-id="becab-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="becab-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="becab-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="becab-137">Parameter</span></span>    | <span data-ttu-id="becab-138">Тип</span><span class="sxs-lookup"><span data-stu-id="becab-138">Type</span></span>   |<span data-ttu-id="becab-139">Описание</span><span class="sxs-lookup"><span data-stu-id="becab-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="becab-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="becab-140">groupIds</span></span>|<span data-ttu-id="becab-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="becab-141">String collection</span></span> |<span data-ttu-id="becab-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="becab-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="becab-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="becab-144">Response</span></span>

<span data-ttu-id="becab-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="becab-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="becab-146">Пример</span><span class="sxs-lookup"><span data-stu-id="becab-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="becab-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="becab-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="becab-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="becab-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="becab-149">C#</span><span class="sxs-lookup"><span data-stu-id="becab-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="becab-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="becab-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="becab-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="becab-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="becab-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="becab-152">Response</span></span>
<span data-ttu-id="becab-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="becab-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
