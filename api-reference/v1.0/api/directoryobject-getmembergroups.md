---
title: Вывод групп элементов
description: Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a4d216c23b52a539611e4e160e2236d66cc9ca3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274874"
---
# <a name="get-member-groups"></a><span data-ttu-id="ee5ff-104">Вывод групп элементов</span><span class="sxs-lookup"><span data-stu-id="ee5ff-104">Get member groups</span></span>

<span data-ttu-id="ee5ff-p102">Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="ee5ff-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee5ff-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee5ff-107">Permissions</span></span>
<span data-ttu-id="ee5ff-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee5ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee5ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee5ff-110">Permission type</span></span>      | <span data-ttu-id="ee5ff-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee5ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee5ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee5ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee5ff-113">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee5ff-113">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="ee5ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee5ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee5ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee5ff-115">Not supported.</span></span>    |
|<span data-ttu-id="ee5ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee5ff-116">Application</span></span> | <span data-ttu-id="ee5ff-117">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee5ff-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee5ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee5ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="ee5ff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee5ff-119">Request headers</span></span>
| <span data-ttu-id="ee5ff-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ee5ff-120">Name</span></span>       | <span data-ttu-id="ee5ff-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ee5ff-121">Type</span></span> | <span data-ttu-id="ee5ff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ee5ff-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ee5ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee5ff-123">Authorization</span></span>  | <span data-ttu-id="ee5ff-124">string</span><span class="sxs-lookup"><span data-stu-id="ee5ff-124">string</span></span>  | <span data-ttu-id="ee5ff-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee5ff-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee5ff-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee5ff-127">Content-Type</span></span>   | <span data-ttu-id="ee5ff-128">string</span><span class="sxs-lookup"><span data-stu-id="ee5ff-128">string</span></span>  | <span data-ttu-id="ee5ff-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ee5ff-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee5ff-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee5ff-130">Request body</span></span>
<span data-ttu-id="ee5ff-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ee5ff-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ee5ff-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="ee5ff-132">Parameter</span></span>    | <span data-ttu-id="ee5ff-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ee5ff-133">Type</span></span>   |<span data-ttu-id="ee5ff-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ee5ff-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee5ff-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ee5ff-135">securityEnabledOnly</span></span>|<span data-ttu-id="ee5ff-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="ee5ff-136">Boolean</span></span>| <span data-ttu-id="ee5ff-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="ee5ff-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="ee5ff-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee5ff-139">Response</span></span>

<span data-ttu-id="ee5ff-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee5ff-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee5ff-141">Пример</span><span class="sxs-lookup"><span data-stu-id="ee5ff-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee5ff-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee5ff-142">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="ee5ff-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee5ff-143">Response</span></span>
<span data-ttu-id="ee5ff-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee5ff-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ee5ff-146">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ee5ff-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ee5ff-147">C#</span><span class="sxs-lookup"><span data-stu-id="ee5ff-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee5ff-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee5ff-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ee5ff-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ee5ff-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
