---
title: 'group: getMemberObjects'
description: Верни все группы, в которые входит эта группа.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 697ea12958a6bb206635726a2d0e18649db71378
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869843"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="b94e2-103">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b94e2-103">group: getMemberObjects</span></span>

<span data-ttu-id="b94e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b94e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b94e2-p101">Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="b94e2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b94e2-108">Permissions</span></span>
<span data-ttu-id="b94e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b94e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b94e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b94e2-111">Permission type</span></span>      | <span data-ttu-id="b94e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b94e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b94e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b94e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b94e2-114">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b94e2-114">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b94e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b94e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b94e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b94e2-116">Not supported.</span></span>    |
|<span data-ttu-id="b94e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b94e2-117">Application</span></span> | <span data-ttu-id="b94e2-118">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b94e2-118">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b94e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b94e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="b94e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b94e2-120">Request headers</span></span>
| <span data-ttu-id="b94e2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b94e2-121">Name</span></span>       | <span data-ttu-id="b94e2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b94e2-122">Type</span></span> | <span data-ttu-id="b94e2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b94e2-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b94e2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b94e2-124">Authorization</span></span>  | <span data-ttu-id="b94e2-125">string</span><span class="sxs-lookup"><span data-stu-id="b94e2-125">string</span></span>  | <span data-ttu-id="b94e2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b94e2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b94e2-128">Request body</span></span>
<span data-ttu-id="b94e2-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b94e2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b94e2-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="b94e2-130">Parameter</span></span>    | <span data-ttu-id="b94e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b94e2-131">Type</span></span>   |<span data-ttu-id="b94e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b94e2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b94e2-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b94e2-133">securityEnabledOnly</span></span>|<span data-ttu-id="b94e2-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="b94e2-134">Boolean</span></span>| <span data-ttu-id="b94e2-p104">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="b94e2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b94e2-137">Response</span></span>
<span data-ttu-id="b94e2-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="b94e2-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="b94e2-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b94e2-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b94e2-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b94e2-140">Request</span></span>
<span data-ttu-id="b94e2-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b94e2-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b94e2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b94e2-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b94e2-143">C#</span><span class="sxs-lookup"><span data-stu-id="b94e2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b94e2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b94e2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b94e2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b94e2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b94e2-146">Java</span><span class="sxs-lookup"><span data-stu-id="b94e2-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b94e2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b94e2-147">Response</span></span>
<span data-ttu-id="b94e2-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b94e2-148">The following is an example of the response.</span></span>
><span data-ttu-id="b94e2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

