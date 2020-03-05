---
title: 'group: getMemberObjects'
description: 'Возврат всех групп и административных единиц, участником которых является группа. Это транзитивная проверка. Note: группы не могут быть членами ролей каталогов, поэтому роли каталогов не будут возвращены.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e111ef7885f0e288d3b59356c791fca5081308e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419865"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="407e4-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="407e4-105">group: getMemberObjects</span></span>

<span data-ttu-id="407e4-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="407e4-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="407e4-107">Возврат всех групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="407e4-107">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="407e4-108">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="407e4-108">The check is transitive.</span></span> <span data-ttu-id="407e4-109">Note: группы не могут быть членами ролей каталогов, поэтому роли каталогов не будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="407e4-109">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="407e4-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="407e4-110">Permissions</span></span>
<span data-ttu-id="407e4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="407e4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="407e4-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="407e4-113">Permission type</span></span>      | <span data-ttu-id="407e4-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="407e4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="407e4-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="407e4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="407e4-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="407e4-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="407e4-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="407e4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="407e4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="407e4-118">Not supported.</span></span>    |
|<span data-ttu-id="407e4-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="407e4-119">Application</span></span> | <span data-ttu-id="407e4-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="407e4-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="407e4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="407e4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="407e4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="407e4-122">Request headers</span></span>
| <span data-ttu-id="407e4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="407e4-123">Name</span></span>       | <span data-ttu-id="407e4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="407e4-124">Type</span></span> | <span data-ttu-id="407e4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="407e4-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="407e4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="407e4-126">Authorization</span></span>  | <span data-ttu-id="407e4-127">string</span><span class="sxs-lookup"><span data-stu-id="407e4-127">string</span></span>  | <span data-ttu-id="407e4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="407e4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="407e4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="407e4-130">Request body</span></span>
<span data-ttu-id="407e4-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="407e4-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="407e4-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="407e4-132">Parameter</span></span>    | <span data-ttu-id="407e4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="407e4-133">Type</span></span>   |<span data-ttu-id="407e4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="407e4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="407e4-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="407e4-135">securityEnabledOnly</span></span>|<span data-ttu-id="407e4-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="407e4-136">Boolean</span></span>|<span data-ttu-id="407e4-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="407e4-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="407e4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="407e4-139">Response</span></span>
<span data-ttu-id="407e4-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="407e4-140">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="407e4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="407e4-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="407e4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="407e4-142">Request</span></span>
<span data-ttu-id="407e4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="407e4-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="407e4-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="407e4-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="407e4-145">C#</span><span class="sxs-lookup"><span data-stu-id="407e4-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="407e4-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="407e4-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="407e4-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="407e4-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="407e4-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="407e4-148">Response</span></span>
<span data-ttu-id="407e4-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="407e4-149">The following is an example of the response.</span></span>
><span data-ttu-id="407e4-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="407e4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
