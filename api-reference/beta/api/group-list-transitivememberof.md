---
title: Список транзитивных групп memberOf
description: Получение групп и административных единиц, участником которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f93d4e812dc4673a72d8e4aa6ed324710819a510
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953649"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="21857-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="21857-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21857-106">Получение групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="21857-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="21857-107">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="21857-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="21857-108">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="21857-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="21857-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21857-109">Permissions</span></span>

<span data-ttu-id="21857-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21857-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21857-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21857-112">Permission type</span></span>      | <span data-ttu-id="21857-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21857-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21857-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21857-114">Delegated (work or school account)</span></span> | <span data-ttu-id="21857-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21857-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="21857-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21857-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21857-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21857-117">Not supported.</span></span>    |
|<span data-ttu-id="21857-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21857-118">Application</span></span> | <span data-ttu-id="21857-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21857-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21857-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21857-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21857-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="21857-121">Optional query parameters</span></span>
<span data-ttu-id="21857-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="21857-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21857-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21857-123">Request headers</span></span>
| <span data-ttu-id="21857-124">Имя</span><span class="sxs-lookup"><span data-stu-id="21857-124">Name</span></span>       | <span data-ttu-id="21857-125">Тип</span><span class="sxs-lookup"><span data-stu-id="21857-125">Type</span></span> | <span data-ttu-id="21857-126">Описание</span><span class="sxs-lookup"><span data-stu-id="21857-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="21857-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="21857-127">Authorization</span></span>  | <span data-ttu-id="21857-128">string</span><span class="sxs-lookup"><span data-stu-id="21857-128">string</span></span>  | <span data-ttu-id="21857-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21857-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21857-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21857-131">Request body</span></span>
<span data-ttu-id="21857-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21857-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21857-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="21857-133">Response</span></span>
<span data-ttu-id="21857-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21857-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21857-135">Пример</span><span class="sxs-lookup"><span data-stu-id="21857-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="21857-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="21857-136">Request</span></span>
<span data-ttu-id="21857-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21857-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="21857-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="21857-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21857-139">C#</span><span class="sxs-lookup"><span data-stu-id="21857-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21857-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="21857-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21857-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="21857-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="21857-142">Java</span><span class="sxs-lookup"><span data-stu-id="21857-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21857-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="21857-143">Response</span></span>

<span data-ttu-id="21857-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21857-144">The following is an example of the response.</span></span>
><span data-ttu-id="21857-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="21857-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21857-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21857-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
