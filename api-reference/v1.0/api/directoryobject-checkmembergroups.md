---
title: Проверка групп элементов
description: Проверяет членство в указанном списке групп и возвращает из этого списка эти группы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc858afd18430635d991ce5e564b1a7c7976ad86
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275595"
---
# <a name="check-member-groups"></a><span data-ttu-id="3fae8-103">Проверка групп элементов</span><span class="sxs-lookup"><span data-stu-id="3fae8-103">Check member groups</span></span>

<span data-ttu-id="3fae8-p101">Проверяет членство в указанном списке групп и возвращает из этого списка группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="3fae8-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fae8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fae8-106">Permissions</span></span>
<span data-ttu-id="3fae8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fae8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fae8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fae8-109">Permission type</span></span>      | <span data-ttu-id="3fae8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fae8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fae8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fae8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fae8-112">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fae8-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="3fae8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fae8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fae8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fae8-114">Not supported.</span></span>    |
|<span data-ttu-id="3fae8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fae8-115">Application</span></span> | <span data-ttu-id="3fae8-116">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fae8-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fae8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fae8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="3fae8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fae8-118">Request headers</span></span>
| <span data-ttu-id="3fae8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3fae8-119">Name</span></span>       | <span data-ttu-id="3fae8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3fae8-120">Type</span></span> | <span data-ttu-id="3fae8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3fae8-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3fae8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fae8-122">Authorization</span></span>  | <span data-ttu-id="3fae8-123">string</span><span class="sxs-lookup"><span data-stu-id="3fae8-123">string</span></span>  | <span data-ttu-id="3fae8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fae8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3fae8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3fae8-126">Content-Type</span></span>  | <span data-ttu-id="3fae8-127">string</span><span class="sxs-lookup"><span data-stu-id="3fae8-127">string</span></span> | <span data-ttu-id="3fae8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3fae8-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3fae8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fae8-129">Request body</span></span>
<span data-ttu-id="3fae8-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3fae8-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3fae8-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3fae8-131">Parameter</span></span>    | <span data-ttu-id="3fae8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3fae8-132">Type</span></span>   |<span data-ttu-id="3fae8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3fae8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fae8-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="3fae8-134">groupIds</span></span>|<span data-ttu-id="3fae8-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3fae8-135">String collection</span></span>|<span data-ttu-id="3fae8-p104">Коллекция, содержащая идентификатор объектов групп, членство в которых нужно проверить. Можно указать до 20 групп.</span><span class="sxs-lookup"><span data-stu-id="3fae8-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="3fae8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fae8-138">Response</span></span>

<span data-ttu-id="3fae8-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fae8-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fae8-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3fae8-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3fae8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fae8-141">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="3fae8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fae8-142">Response</span></span>
<span data-ttu-id="3fae8-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fae8-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3fae8-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="3fae8-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3fae8-146">C#</span><span class="sxs-lookup"><span data-stu-id="3fae8-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3fae8-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="3fae8-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3fae8-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3fae8-148">Objective-C</span></span>](#tab/objective-c)
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
