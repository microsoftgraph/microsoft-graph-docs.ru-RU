---
title: 'group: getMemberObjects'
description: Возвращаем все группы и административные единицы, в которые входит группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 78d240211f38f25a1e59c76634c4dde3b147393b
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869752"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="136e7-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="136e7-105">group: getMemberObjects</span></span>

<span data-ttu-id="136e7-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="136e7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="136e7-107">Возвращаем все группы и административные единицы, в которые входит группа.</span><span class="sxs-lookup"><span data-stu-id="136e7-107">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="136e7-108">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="136e7-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="136e7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="136e7-109">Permissions</span></span>
<span data-ttu-id="136e7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136e7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="136e7-112">Permission type</span></span>      | <span data-ttu-id="136e7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="136e7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="136e7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="136e7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="136e7-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="136e7-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="136e7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="136e7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="136e7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="136e7-117">Not supported.</span></span>    |
|<span data-ttu-id="136e7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="136e7-118">Application</span></span> | <span data-ttu-id="136e7-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136e7-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="136e7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="136e7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="136e7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="136e7-121">Request headers</span></span>
| <span data-ttu-id="136e7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="136e7-122">Name</span></span>       | <span data-ttu-id="136e7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="136e7-123">Type</span></span> | <span data-ttu-id="136e7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="136e7-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="136e7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="136e7-125">Authorization</span></span>  | <span data-ttu-id="136e7-126">string</span><span class="sxs-lookup"><span data-stu-id="136e7-126">string</span></span>  | <span data-ttu-id="136e7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="136e7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="136e7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="136e7-129">Request body</span></span>
<span data-ttu-id="136e7-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="136e7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="136e7-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="136e7-131">Parameter</span></span>    | <span data-ttu-id="136e7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="136e7-132">Type</span></span>   |<span data-ttu-id="136e7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="136e7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="136e7-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="136e7-134">securityEnabledOnly</span></span>|<span data-ttu-id="136e7-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="136e7-135">Boolean</span></span>|<span data-ttu-id="136e7-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="136e7-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="136e7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="136e7-138">Response</span></span>
<span data-ttu-id="136e7-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="136e7-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="136e7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="136e7-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="136e7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="136e7-141">Request</span></span>
<span data-ttu-id="136e7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="136e7-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="136e7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="136e7-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="136e7-144">C#</span><span class="sxs-lookup"><span data-stu-id="136e7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="136e7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="136e7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="136e7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="136e7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="136e7-147">Java</span><span class="sxs-lookup"><span data-stu-id="136e7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="136e7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="136e7-148">Response</span></span>
<span data-ttu-id="136e7-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="136e7-149">The following is an example of the response.</span></span>
><span data-ttu-id="136e7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="136e7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


