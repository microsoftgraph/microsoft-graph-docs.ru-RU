---
title: Проверка групп элементов
description: Проверяет членство в указанном списке групп и возвращает из этого списка эти группы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad25e1e8925135bd5b9760f957d7c755061ad305
ms.sourcegitcommit: 6d8bf390380b9434ba626d6dc5101afcf6ba6f8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2019
ms.locfileid: "35395172"
---
# <a name="check-member-groups"></a><span data-ttu-id="f538d-103">Проверка групп элементов</span><span class="sxs-lookup"><span data-stu-id="f538d-103">Check member groups</span></span>

<span data-ttu-id="f538d-p101">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="f538d-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f538d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f538d-106">Permissions</span></span>
<span data-ttu-id="f538d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f538d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f538d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f538d-109">Permission type</span></span>      | <span data-ttu-id="f538d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f538d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f538d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f538d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f538d-112">User. ReadBasic. ALL и Group. Read. ALL, User. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f538d-112">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="f538d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f538d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f538d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f538d-114">Not supported.</span></span>    |
|<span data-ttu-id="f538d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f538d-115">Application</span></span> | <span data-ttu-id="f538d-116">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f538d-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="f538d-117">Используйте приведенные ниже рекомендации по сценариям, чтобы определить, какие типы разрешений следует использовать:</span><span class="sxs-lookup"><span data-stu-id="f538d-117">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="f538d-118">Используйте разрешения User. Read и Group. Read. ALL, чтобы проверить принадлежность к группам для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="f538d-118">Use User.Read and Group.Read.All permissions to check group memberships for the signed-in user.</span></span>
- <span data-ttu-id="f538d-119">Используйте User. ReadBasic. ALL и Group. Read. ALL или User. Read. ALL и Group. Read. ALL, чтобы проверить принадлежность к группам для любого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f538d-119">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to check group memberships for any user.</span></span>
- <span data-ttu-id="f538d-120">Используйте разрешение Group. Read. ALL, чтобы проверить принадлежность к группам для группы.</span><span class="sxs-lookup"><span data-stu-id="f538d-120">Use Group.Read.All permission to check group memberships for a group.</span></span>
- <span data-ttu-id="f538d-121">Используйте разрешение Directory. Read. ALL, чтобы проверить принадлежность к группам для объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="f538d-121">Use Directory.Read.All permission to check group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="f538d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f538d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="f538d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f538d-123">Request headers</span></span>
| <span data-ttu-id="f538d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f538d-124">Name</span></span>       | <span data-ttu-id="f538d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f538d-125">Type</span></span> | <span data-ttu-id="f538d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f538d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f538d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f538d-127">Authorization</span></span>  | <span data-ttu-id="f538d-128">string</span><span class="sxs-lookup"><span data-stu-id="f538d-128">string</span></span>  | <span data-ttu-id="f538d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f538d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f538d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f538d-131">Content-Type</span></span>  | <span data-ttu-id="f538d-132">string</span><span class="sxs-lookup"><span data-stu-id="f538d-132">string</span></span> | <span data-ttu-id="f538d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f538d-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f538d-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f538d-134">Request body</span></span>
<span data-ttu-id="f538d-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f538d-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f538d-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="f538d-136">Parameter</span></span>    | <span data-ttu-id="f538d-137">Тип</span><span class="sxs-lookup"><span data-stu-id="f538d-137">Type</span></span>   |<span data-ttu-id="f538d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="f538d-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f538d-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="f538d-139">groupIds</span></span>|<span data-ttu-id="f538d-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f538d-140">String collection</span></span>|<span data-ttu-id="f538d-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="f538d-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="f538d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f538d-143">Response</span></span>

<span data-ttu-id="f538d-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f538d-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f538d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="f538d-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f538d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f538d-146">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="f538d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f538d-147">Response</span></span>
<span data-ttu-id="f538d-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f538d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f538d-150">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f538d-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f538d-151">C#</span><span class="sxs-lookup"><span data-stu-id="f538d-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f538d-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="f538d-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f538d-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f538d-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
