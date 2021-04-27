---
title: 'group: getMemberObjects'
description: Возвращаем все группы и административные единицы, в которые входит группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 39ee632ad54608f9e662309365abfb5d994d2312
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041808"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="55909-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="55909-105">group: getMemberObjects</span></span>

<span data-ttu-id="55909-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55909-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55909-107">Возвращаем все группы и административные единицы, в которые входит группа.</span><span class="sxs-lookup"><span data-stu-id="55909-107">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="55909-108">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="55909-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="55909-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55909-109">Permissions</span></span>
<span data-ttu-id="55909-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55909-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55909-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55909-112">Permission type</span></span>      | <span data-ttu-id="55909-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55909-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55909-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55909-114">Delegated (work or school account)</span></span> | <span data-ttu-id="55909-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55909-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55909-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55909-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55909-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55909-117">Not supported.</span></span>    |
|<span data-ttu-id="55909-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55909-118">Application</span></span> | <span data-ttu-id="55909-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55909-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55909-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55909-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="55909-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55909-121">Request headers</span></span>
| <span data-ttu-id="55909-122">Имя</span><span class="sxs-lookup"><span data-stu-id="55909-122">Name</span></span>       | <span data-ttu-id="55909-123">Тип</span><span class="sxs-lookup"><span data-stu-id="55909-123">Type</span></span> | <span data-ttu-id="55909-124">Описание</span><span class="sxs-lookup"><span data-stu-id="55909-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55909-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="55909-125">Authorization</span></span>  | <span data-ttu-id="55909-126">string</span><span class="sxs-lookup"><span data-stu-id="55909-126">string</span></span>  | <span data-ttu-id="55909-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55909-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55909-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55909-129">Request body</span></span>
<span data-ttu-id="55909-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="55909-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55909-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="55909-131">Parameter</span></span>    | <span data-ttu-id="55909-132">Тип</span><span class="sxs-lookup"><span data-stu-id="55909-132">Type</span></span>   |<span data-ttu-id="55909-133">Описание</span><span class="sxs-lookup"><span data-stu-id="55909-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55909-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="55909-134">securityEnabledOnly</span></span>|<span data-ttu-id="55909-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="55909-135">Boolean</span></span>|<span data-ttu-id="55909-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="55909-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="55909-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="55909-138">Response</span></span>
<span data-ttu-id="55909-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="55909-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="55909-140">Пример</span><span class="sxs-lookup"><span data-stu-id="55909-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="55909-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="55909-141">Request</span></span>
<span data-ttu-id="55909-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55909-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55909-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="55909-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="55909-144">C#</span><span class="sxs-lookup"><span data-stu-id="55909-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55909-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55909-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55909-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55909-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55909-147">Java</span><span class="sxs-lookup"><span data-stu-id="55909-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55909-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="55909-148">Response</span></span>
<span data-ttu-id="55909-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55909-149">The following is an example of the response.</span></span>
><span data-ttu-id="55909-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="55909-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


