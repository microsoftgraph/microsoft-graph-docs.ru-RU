---
title: Список транзитивных групп memberOf
description: Получение групп, членом которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.
author: anchanda
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c66aa31dbd8f561b343d65247bb7394e71c6d6e1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720783"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="f7e9f-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="f7e9f-105">List group transitive memberOf</span></span>

<span data-ttu-id="f7e9f-106">Получение групп, членом которых является группа.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-106">Get groups that the group is a member of.</span></span>  <span data-ttu-id="f7e9f-107">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="f7e9f-108">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e9f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e9f-109">Permissions</span></span>

<span data-ttu-id="f7e9f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e9f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e9f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7e9f-112">Permission type</span></span>      | <span data-ttu-id="f7e9f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7e9f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7e9f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7e9f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f7e9f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7e9f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7e9f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7e9f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7e9f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-117">Not supported.</span></span>    |
|<span data-ttu-id="f7e9f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7e9f-118">Application</span></span> | <span data-ttu-id="f7e9f-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e9f-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7e9f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7e9f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7e9f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7e9f-121">Optional query parameters</span></span>
<span data-ttu-id="f7e9f-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7e9f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7e9f-123">Request headers</span></span>
| <span data-ttu-id="f7e9f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f7e9f-124">Name</span></span>       | <span data-ttu-id="f7e9f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f7e9f-125">Type</span></span> | <span data-ttu-id="f7e9f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f7e9f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f7e9f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e9f-127">Authorization</span></span>  | <span data-ttu-id="f7e9f-128">string</span><span class="sxs-lookup"><span data-stu-id="f7e9f-128">string</span></span>  | <span data-ttu-id="f7e9f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7e9f-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7e9f-131">Request body</span></span>
<span data-ttu-id="f7e9f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7e9f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7e9f-133">Response</span></span>
<span data-ttu-id="f7e9f-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e9f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f7e9f-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7e9f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7e9f-136">Request</span></span>
<span data-ttu-id="f7e9f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7e9f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7e9f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7e9f-139">C#</span><span class="sxs-lookup"><span data-stu-id="f7e9f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7e9f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7e9f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7e9f-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f7e9f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7e9f-142">Java</span><span class="sxs-lookup"><span data-stu-id="f7e9f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7e9f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7e9f-143">Response</span></span>

<span data-ttu-id="f7e9f-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-144">The following is an example of the response.</span></span>
><span data-ttu-id="f7e9f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7e9f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
