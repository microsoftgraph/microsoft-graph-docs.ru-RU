---
title: 'group: getMemberObjects'
description: Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ab08cd3d4abcaef15b27db676fa5d4bc9d0495ed
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42927020"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="83d61-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="83d61-105">group: getMemberObjects</span></span>

<span data-ttu-id="83d61-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d61-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83d61-p102">Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="83d61-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="83d61-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83d61-110">Permissions</span></span>
<span data-ttu-id="83d61-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d61-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d61-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83d61-113">Permission type</span></span>      | <span data-ttu-id="83d61-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83d61-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83d61-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83d61-115">Delegated (work or school account)</span></span> | <span data-ttu-id="83d61-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83d61-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83d61-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83d61-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83d61-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83d61-118">Not supported.</span></span>    |
|<span data-ttu-id="83d61-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83d61-119">Application</span></span> | <span data-ttu-id="83d61-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d61-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83d61-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83d61-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="83d61-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83d61-122">Request headers</span></span>
| <span data-ttu-id="83d61-123">Имя</span><span class="sxs-lookup"><span data-stu-id="83d61-123">Name</span></span>       | <span data-ttu-id="83d61-124">Тип</span><span class="sxs-lookup"><span data-stu-id="83d61-124">Type</span></span> | <span data-ttu-id="83d61-125">Описание</span><span class="sxs-lookup"><span data-stu-id="83d61-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83d61-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="83d61-126">Authorization</span></span>  | <span data-ttu-id="83d61-127">string</span><span class="sxs-lookup"><span data-stu-id="83d61-127">string</span></span>  | <span data-ttu-id="83d61-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83d61-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83d61-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83d61-130">Request body</span></span>
<span data-ttu-id="83d61-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="83d61-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83d61-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="83d61-132">Parameter</span></span>    | <span data-ttu-id="83d61-133">Тип</span><span class="sxs-lookup"><span data-stu-id="83d61-133">Type</span></span>   |<span data-ttu-id="83d61-134">Описание</span><span class="sxs-lookup"><span data-stu-id="83d61-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83d61-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="83d61-135">securityEnabledOnly</span></span>|<span data-ttu-id="83d61-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="83d61-136">Boolean</span></span>| <span data-ttu-id="83d61-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="83d61-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="83d61-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="83d61-139">Response</span></span>
<span data-ttu-id="83d61-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="83d61-140">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="83d61-141">Пример</span><span class="sxs-lookup"><span data-stu-id="83d61-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="83d61-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="83d61-142">Request</span></span>
<span data-ttu-id="83d61-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83d61-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83d61-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="83d61-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="83d61-145">C#</span><span class="sxs-lookup"><span data-stu-id="83d61-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83d61-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83d61-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83d61-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83d61-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83d61-148">Java</span><span class="sxs-lookup"><span data-stu-id="83d61-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="83d61-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="83d61-149">Response</span></span>
<span data-ttu-id="83d61-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83d61-150">The following is an example of the response.</span></span>
><span data-ttu-id="83d61-151">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="83d61-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="83d61-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83d61-152">All the properties will be returned from an actual call.</span></span>
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
