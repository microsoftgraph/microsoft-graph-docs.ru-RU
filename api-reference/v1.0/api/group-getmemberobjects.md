---
title: 'group: getMemberObjects'
description: Возвращает все группы, в которых входит эта группа.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c1da59fa3644b8ca1ab3d06f71cfba3f61f5abcf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094696"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="a0a14-103">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a0a14-103">group: getMemberObjects</span></span>

<span data-ttu-id="a0a14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0a14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0a14-p101">Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="a0a14-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0a14-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0a14-108">Permissions</span></span>
<span data-ttu-id="a0a14-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0a14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0a14-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0a14-111">Permission type</span></span>      | <span data-ttu-id="a0a14-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0a14-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0a14-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0a14-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a0a14-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0a14-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0a14-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0a14-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0a14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a14-116">Not supported.</span></span>    |
|<span data-ttu-id="a0a14-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0a14-117">Application</span></span> | <span data-ttu-id="a0a14-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a14-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0a14-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0a14-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="a0a14-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0a14-120">Request headers</span></span>
| <span data-ttu-id="a0a14-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a0a14-121">Name</span></span>       | <span data-ttu-id="a0a14-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a0a14-122">Type</span></span> | <span data-ttu-id="a0a14-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a14-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0a14-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0a14-124">Authorization</span></span>  | <span data-ttu-id="a0a14-125">string</span><span class="sxs-lookup"><span data-stu-id="a0a14-125">string</span></span>  | <span data-ttu-id="a0a14-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0a14-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0a14-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0a14-128">Request body</span></span>
<span data-ttu-id="a0a14-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a0a14-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a0a14-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="a0a14-130">Parameter</span></span>    | <span data-ttu-id="a0a14-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a0a14-131">Type</span></span>   |<span data-ttu-id="a0a14-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a14-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0a14-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a0a14-133">securityEnabledOnly</span></span>|<span data-ttu-id="a0a14-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="a0a14-134">Boolean</span></span>| <span data-ttu-id="a0a14-p104">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="a0a14-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="a0a14-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0a14-137">Response</span></span>
<span data-ttu-id="a0a14-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="a0a14-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a0a14-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a0a14-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0a14-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0a14-140">Request</span></span>
<span data-ttu-id="a0a14-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0a14-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0a14-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0a14-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a0a14-143">C#</span><span class="sxs-lookup"><span data-stu-id="a0a14-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0a14-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0a14-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0a14-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0a14-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0a14-146">Java</span><span class="sxs-lookup"><span data-stu-id="a0a14-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a0a14-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0a14-147">Response</span></span>
<span data-ttu-id="a0a14-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a0a14-148">The following is an example of the response.</span></span>
><span data-ttu-id="a0a14-149">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a0a14-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a0a14-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0a14-150">All the properties will be returned from an actual call.</span></span>
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

