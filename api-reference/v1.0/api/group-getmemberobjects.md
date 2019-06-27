---
title: 'group: getMemberObjects'
description: Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 99344b834ac1f7cfd3d0ed02a9bdfc91a23163e2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273551"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="3c7f6-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="3c7f6-105">group: getMemberObjects</span></span>
<span data-ttu-id="3c7f6-p102">Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c7f6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c7f6-109">Permissions</span></span>
<span data-ttu-id="3c7f6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c7f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c7f6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c7f6-112">Permission type</span></span>      | <span data-ttu-id="3c7f6-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c7f6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c7f6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c7f6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3c7f6-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c7f6-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c7f6-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c7f6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c7f6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-117">Not supported.</span></span>    |
|<span data-ttu-id="3c7f6-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c7f6-118">Application</span></span> | <span data-ttu-id="3c7f6-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c7f6-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c7f6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c7f6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="3c7f6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c7f6-121">Request headers</span></span>
| <span data-ttu-id="3c7f6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3c7f6-122">Name</span></span>       | <span data-ttu-id="3c7f6-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3c7f6-123">Type</span></span> | <span data-ttu-id="3c7f6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3c7f6-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c7f6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c7f6-125">Authorization</span></span>  | <span data-ttu-id="3c7f6-126">string</span><span class="sxs-lookup"><span data-stu-id="3c7f6-126">string</span></span>  | <span data-ttu-id="3c7f6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c7f6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c7f6-129">Request body</span></span>
<span data-ttu-id="3c7f6-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c7f6-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3c7f6-131">Parameter</span></span>    | <span data-ttu-id="3c7f6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3c7f6-132">Type</span></span>   |<span data-ttu-id="3c7f6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3c7f6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c7f6-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="3c7f6-134">securityEnabledOnly</span></span>|<span data-ttu-id="3c7f6-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="3c7f6-135">Boolean</span></span>| <span data-ttu-id="3c7f6-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="3c7f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c7f6-138">Response</span></span>
<span data-ttu-id="3c7f6-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="3c7f6-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3c7f6-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3c7f6-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c7f6-141">Request</span></span>
<span data-ttu-id="3c7f6-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="3c7f6-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c7f6-143">Response</span></span>
<span data-ttu-id="3c7f6-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-144">The following is an example of the response.</span></span>
><span data-ttu-id="3c7f6-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c7f6-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c7f6-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c7f6-147">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="3c7f6-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c7f6-148">C#</span><span class="sxs-lookup"><span data-stu-id="3c7f6-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c7f6-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c7f6-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_getmemberobjects-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3c7f6-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c7f6-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_getmemberobjects-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
