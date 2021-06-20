---
title: 'group: getMemberObjects'
description: Верни все группы, в которые входит эта группа.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a5f71a53fba79da14674328760081a51fbdcea34
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030791"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="2d71f-103">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="2d71f-103">group: getMemberObjects</span></span>

<span data-ttu-id="2d71f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d71f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d71f-105">Верни все группы, в которые входит эта группа.</span><span class="sxs-lookup"><span data-stu-id="2d71f-105">Return all of the groups that this group is a member of.</span></span> <span data-ttu-id="2d71f-106">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="2d71f-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d71f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d71f-107">Permissions</span></span>
<span data-ttu-id="2d71f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d71f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d71f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d71f-110">Permission type</span></span>      | <span data-ttu-id="2d71f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d71f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d71f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d71f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d71f-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d71f-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2d71f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d71f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d71f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d71f-115">Not supported.</span></span>    |
|<span data-ttu-id="2d71f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d71f-116">Application</span></span> | <span data-ttu-id="2d71f-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d71f-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d71f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d71f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="2d71f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d71f-119">Request headers</span></span>
| <span data-ttu-id="2d71f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2d71f-120">Name</span></span>       | <span data-ttu-id="2d71f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2d71f-121">Type</span></span> | <span data-ttu-id="2d71f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d71f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d71f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d71f-123">Authorization</span></span>  | <span data-ttu-id="2d71f-124">string</span><span class="sxs-lookup"><span data-stu-id="2d71f-124">string</span></span>  | <span data-ttu-id="2d71f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d71f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d71f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d71f-127">Request body</span></span>
<span data-ttu-id="2d71f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2d71f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d71f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="2d71f-129">Parameter</span></span>    | <span data-ttu-id="2d71f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2d71f-130">Type</span></span>   |<span data-ttu-id="2d71f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2d71f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d71f-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2d71f-132">securityEnabledOnly</span></span>|<span data-ttu-id="2d71f-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="2d71f-133">Boolean</span></span>| <span data-ttu-id="2d71f-p104">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="2d71f-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="2d71f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d71f-136">Response</span></span>
<span data-ttu-id="2d71f-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="2d71f-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="2d71f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2d71f-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2d71f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d71f-139">Request</span></span>
<span data-ttu-id="2d71f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d71f-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d71f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d71f-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2d71f-142">C#</span><span class="sxs-lookup"><span data-stu-id="2d71f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d71f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d71f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d71f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d71f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d71f-145">Java</span><span class="sxs-lookup"><span data-stu-id="2d71f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d71f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d71f-146">Response</span></span>
<span data-ttu-id="2d71f-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2d71f-147">The following is an example of the response.</span></span>
><span data-ttu-id="2d71f-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2d71f-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

