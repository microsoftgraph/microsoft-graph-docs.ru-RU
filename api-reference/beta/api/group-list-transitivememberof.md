---
title: Список транзитивных групп memberOf
description: Получение групп и административных единиц, участником которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 787870d802860b76695253931df03e3c873fbcd8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858247"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="35caa-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="35caa-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35caa-106">Получение групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="35caa-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="35caa-107">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="35caa-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="35caa-108">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="35caa-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="35caa-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35caa-109">Permissions</span></span>

<span data-ttu-id="35caa-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35caa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35caa-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35caa-112">Permission type</span></span>      | <span data-ttu-id="35caa-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35caa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35caa-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35caa-114">Delegated (work or school account)</span></span> | <span data-ttu-id="35caa-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35caa-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="35caa-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35caa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35caa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35caa-117">Not supported.</span></span>    |
|<span data-ttu-id="35caa-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35caa-118">Application</span></span> | <span data-ttu-id="35caa-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35caa-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35caa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35caa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35caa-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35caa-121">Optional query parameters</span></span>
<span data-ttu-id="35caa-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35caa-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35caa-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35caa-123">Request headers</span></span>
| <span data-ttu-id="35caa-124">Имя</span><span class="sxs-lookup"><span data-stu-id="35caa-124">Name</span></span>       | <span data-ttu-id="35caa-125">Тип</span><span class="sxs-lookup"><span data-stu-id="35caa-125">Type</span></span> | <span data-ttu-id="35caa-126">Описание</span><span class="sxs-lookup"><span data-stu-id="35caa-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="35caa-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="35caa-127">Authorization</span></span>  | <span data-ttu-id="35caa-128">string</span><span class="sxs-lookup"><span data-stu-id="35caa-128">string</span></span>  | <span data-ttu-id="35caa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35caa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35caa-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35caa-131">Request body</span></span>
<span data-ttu-id="35caa-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35caa-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35caa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="35caa-133">Response</span></span>
<span data-ttu-id="35caa-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35caa-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35caa-135">Пример</span><span class="sxs-lookup"><span data-stu-id="35caa-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="35caa-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="35caa-136">Request</span></span>
<span data-ttu-id="35caa-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35caa-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="35caa-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="35caa-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35caa-139">C#</span><span class="sxs-lookup"><span data-stu-id="35caa-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35caa-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="35caa-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35caa-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="35caa-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="35caa-142">Java</span><span class="sxs-lookup"><span data-stu-id="35caa-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35caa-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="35caa-143">Response</span></span>

<span data-ttu-id="35caa-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35caa-144">The following is an example of the response.</span></span>
><span data-ttu-id="35caa-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35caa-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="35caa-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35caa-146">All the properties will be returned from an actual call.</span></span>
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
