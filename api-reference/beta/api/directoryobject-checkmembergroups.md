---
title: Проверка групп элементов
description: Проверка членства в указанном списке групп и возврат из этого списка этих групп
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 549a8ac05895ffd149971a6c34297b126c7ea2da
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176558"
---
# <a name="check-member-groups"></a><span data-ttu-id="eb24a-103">Проверка членства в группах</span><span class="sxs-lookup"><span data-stu-id="eb24a-103">Check member groups</span></span>

<span data-ttu-id="eb24a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb24a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb24a-105">Проверьте членство в указанном списке групп и возвращает из него группы, участником которых является указанный пользователь, группа, участник службы или объект каталога.</span><span class="sxs-lookup"><span data-stu-id="eb24a-105">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="eb24a-106">Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="eb24a-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb24a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb24a-107">Permissions</span></span>
<span data-ttu-id="eb24a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb24a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eb24a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb24a-110">Permission type</span></span>      | <span data-ttu-id="eb24a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb24a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb24a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb24a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb24a-113">User.ReadBasic.All, User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb24a-113">User.ReadBasic.All, User.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="eb24a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb24a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb24a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb24a-115">Not supported.</span></span>    |
|<span data-ttu-id="eb24a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb24a-116">Application</span></span> | <span data-ttu-id="eb24a-117">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb24a-117">User.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="eb24a-118">Используйте рекомендации по следующим сценариям, чтобы определить, какие типы разрешений использовать:</span><span class="sxs-lookup"><span data-stu-id="eb24a-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="eb24a-119">Используйте разрешения User.Read и GroupMember.Read.All или User.Read и Group.Read.All, чтобы получить членство в группах для во доступного пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb24a-119">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="eb24a-120">Используйте разрешения User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All или User.Read.All и Group.Read.All, чтобы получить членство в группах для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb24a-120">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="eb24a-121">Используйте разрешение GroupMember.Read.All или Group.Read.All, чтобы получить членство в группе.</span><span class="sxs-lookup"><span data-stu-id="eb24a-121">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="eb24a-122">Используйте разрешения Application.ReadWrite.All и GroupMember.Read.All или Application.ReadWrite.All и Group.Read.All для получения членства в группах для участников-служб.</span><span class="sxs-lookup"><span data-stu-id="eb24a-122">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="eb24a-123">Используйте разрешение Directory.Read.All для получения членства в группах для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="eb24a-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="eb24a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb24a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servicePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="eb24a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb24a-125">Request headers</span></span>
| <span data-ttu-id="eb24a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="eb24a-126">Name</span></span>       | <span data-ttu-id="eb24a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="eb24a-127">Type</span></span> | <span data-ttu-id="eb24a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="eb24a-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb24a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb24a-129">Authorization</span></span>  | <span data-ttu-id="eb24a-130">string</span><span class="sxs-lookup"><span data-stu-id="eb24a-130">string</span></span>  | <span data-ttu-id="eb24a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb24a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb24a-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb24a-133">Content-Type</span></span>  | <span data-ttu-id="eb24a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="eb24a-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eb24a-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb24a-135">Request body</span></span>
<span data-ttu-id="eb24a-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="eb24a-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb24a-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="eb24a-137">Parameter</span></span>    | <span data-ttu-id="eb24a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="eb24a-138">Type</span></span>   |<span data-ttu-id="eb24a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="eb24a-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb24a-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="eb24a-140">groupIds</span></span>|<span data-ttu-id="eb24a-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eb24a-141">String collection</span></span> |<span data-ttu-id="eb24a-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="eb24a-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="eb24a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb24a-144">Response</span></span>

<span data-ttu-id="eb24a-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb24a-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb24a-146">Пример</span><span class="sxs-lookup"><span data-stu-id="eb24a-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb24a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb24a-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eb24a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb24a-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eb24a-149">C#</span><span class="sxs-lookup"><span data-stu-id="eb24a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb24a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb24a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb24a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb24a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb24a-152">Java</span><span class="sxs-lookup"><span data-stu-id="eb24a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eb24a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb24a-153">Response</span></span>
<span data-ttu-id="eb24a-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb24a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


