---
title: 'group: getMemberObjects'
description: Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1a391c8c30fc2dc38893a980ee73006e0960e715
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014885"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="dbf47-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="dbf47-105">group: getMemberObjects</span></span>
<span data-ttu-id="dbf47-p102">Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="dbf47-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbf47-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbf47-109">Permissions</span></span>
<span data-ttu-id="dbf47-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbf47-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbf47-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbf47-112">Permission type</span></span>      | <span data-ttu-id="dbf47-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbf47-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbf47-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbf47-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dbf47-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dbf47-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dbf47-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbf47-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbf47-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbf47-117">Not supported.</span></span>    |
|<span data-ttu-id="dbf47-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbf47-118">Application</span></span> | <span data-ttu-id="dbf47-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf47-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbf47-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbf47-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="dbf47-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbf47-121">Request headers</span></span>
| <span data-ttu-id="dbf47-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dbf47-122">Name</span></span>       | <span data-ttu-id="dbf47-123">Тип</span><span class="sxs-lookup"><span data-stu-id="dbf47-123">Type</span></span> | <span data-ttu-id="dbf47-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf47-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbf47-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbf47-125">Authorization</span></span>  | <span data-ttu-id="dbf47-126">string</span><span class="sxs-lookup"><span data-stu-id="dbf47-126">string</span></span>  | <span data-ttu-id="dbf47-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbf47-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbf47-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbf47-129">Request body</span></span>
<span data-ttu-id="dbf47-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dbf47-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbf47-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="dbf47-131">Parameter</span></span>    | <span data-ttu-id="dbf47-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dbf47-132">Type</span></span>   |<span data-ttu-id="dbf47-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf47-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbf47-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="dbf47-134">securityEnabledOnly</span></span>|<span data-ttu-id="dbf47-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="dbf47-135">Boolean</span></span>| <span data-ttu-id="dbf47-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="dbf47-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="dbf47-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbf47-138">Response</span></span>
<span data-ttu-id="dbf47-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="dbf47-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="dbf47-140">Пример</span><span class="sxs-lookup"><span data-stu-id="dbf47-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dbf47-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbf47-141">Request</span></span>
<span data-ttu-id="dbf47-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbf47-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dbf47-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbf47-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbf47-144">C#</span><span class="sxs-lookup"><span data-stu-id="dbf47-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbf47-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="dbf47-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbf47-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dbf47-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dbf47-147">Java</span><span class="sxs-lookup"><span data-stu-id="dbf47-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dbf47-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbf47-148">Response</span></span>
<span data-ttu-id="dbf47-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dbf47-149">The following is an example of the response.</span></span>
><span data-ttu-id="dbf47-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dbf47-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dbf47-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbf47-151">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
