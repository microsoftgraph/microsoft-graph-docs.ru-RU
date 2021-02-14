---
title: Проверка групп элементов
description: Проверка членства в указанном списке групп и возврат из этого списка этих групп
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a1daa0e3abe6badb8349806bd8af66adeafd02c7
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176227"
---
# <a name="check-member-groups"></a><span data-ttu-id="51304-103">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="51304-103">Check member groups</span></span>

<span data-ttu-id="51304-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51304-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51304-p101">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="51304-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="51304-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51304-107">Permissions</span></span>
<span data-ttu-id="51304-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51304-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51304-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51304-110">Permission type</span></span>      | <span data-ttu-id="51304-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51304-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51304-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51304-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51304-113">User.ReadBasic.All, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="51304-113">User.ReadBasic.All, User.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="51304-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51304-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51304-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51304-115">Not supported.</span></span>    |
|<span data-ttu-id="51304-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51304-116">Application</span></span> | <span data-ttu-id="51304-117">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="51304-117">User.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="51304-118">Используйте рекомендации по следующим сценариям, чтобы определить, какие типы разрешений использовать:</span><span class="sxs-lookup"><span data-stu-id="51304-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="51304-119">Используйте разрешения User.Read и GroupMember.Read.All или User.Read и Group.Read.All, чтобы получить членство в группах для во доступного пользователя.</span><span class="sxs-lookup"><span data-stu-id="51304-119">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="51304-120">Используйте разрешения User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All или User.Read.All и Group.Read.All для получения членства в группах для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="51304-120">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="51304-121">Используйте разрешение GroupMember.Read.All или Group.Read.All, чтобы получить членство в группе.</span><span class="sxs-lookup"><span data-stu-id="51304-121">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="51304-122">Используйте разрешение Directory.Read.All для проверки членства в группах для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="51304-122">Use Directory.Read.All permission to check group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="51304-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51304-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="51304-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51304-124">Request headers</span></span>
| <span data-ttu-id="51304-125">Имя</span><span class="sxs-lookup"><span data-stu-id="51304-125">Name</span></span>       | <span data-ttu-id="51304-126">Тип</span><span class="sxs-lookup"><span data-stu-id="51304-126">Type</span></span> | <span data-ttu-id="51304-127">Описание</span><span class="sxs-lookup"><span data-stu-id="51304-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51304-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="51304-128">Authorization</span></span>  | <span data-ttu-id="51304-129">string</span><span class="sxs-lookup"><span data-stu-id="51304-129">string</span></span>  | <span data-ttu-id="51304-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51304-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51304-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51304-132">Content-Type</span></span>  | <span data-ttu-id="51304-133">string</span><span class="sxs-lookup"><span data-stu-id="51304-133">string</span></span> | <span data-ttu-id="51304-134">application/json</span><span class="sxs-lookup"><span data-stu-id="51304-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51304-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51304-135">Request body</span></span>
<span data-ttu-id="51304-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="51304-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51304-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="51304-137">Parameter</span></span>    | <span data-ttu-id="51304-138">Тип</span><span class="sxs-lookup"><span data-stu-id="51304-138">Type</span></span>   |<span data-ttu-id="51304-139">Описание</span><span class="sxs-lookup"><span data-stu-id="51304-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51304-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="51304-140">groupIds</span></span>|<span data-ttu-id="51304-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="51304-141">String collection</span></span>|<span data-ttu-id="51304-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="51304-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="51304-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="51304-144">Response</span></span>

<span data-ttu-id="51304-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51304-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51304-146">Пример</span><span class="sxs-lookup"><span data-stu-id="51304-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="51304-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="51304-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51304-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="51304-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="51304-149">C#</span><span class="sxs-lookup"><span data-stu-id="51304-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51304-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51304-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51304-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51304-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51304-152">Java</span><span class="sxs-lookup"><span data-stu-id="51304-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="51304-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="51304-153">Response</span></span>
<span data-ttu-id="51304-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51304-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

