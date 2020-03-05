---
title: Список транзитивных групп memberOf
description: Получение групп и административных единиц, участником которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a8fe1349787819f6a3c97f6e23fa349603bde0f3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419249"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="25e91-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="25e91-105">List group transitive memberOf</span></span>

<span data-ttu-id="25e91-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="25e91-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25e91-107">Получение групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="25e91-107">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="25e91-108">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="25e91-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="25e91-109">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="25e91-109">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="25e91-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25e91-110">Permissions</span></span>

<span data-ttu-id="25e91-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25e91-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25e91-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25e91-113">Permission type</span></span>      | <span data-ttu-id="25e91-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25e91-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25e91-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25e91-115">Delegated (work or school account)</span></span> | <span data-ttu-id="25e91-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="25e91-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="25e91-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25e91-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25e91-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25e91-118">Not supported.</span></span>    |
|<span data-ttu-id="25e91-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25e91-119">Application</span></span> | <span data-ttu-id="25e91-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e91-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="25e91-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25e91-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25e91-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25e91-122">Optional query parameters</span></span>
<span data-ttu-id="25e91-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="25e91-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25e91-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25e91-124">Request headers</span></span>
| <span data-ttu-id="25e91-125">Имя</span><span class="sxs-lookup"><span data-stu-id="25e91-125">Name</span></span>       | <span data-ttu-id="25e91-126">Тип</span><span class="sxs-lookup"><span data-stu-id="25e91-126">Type</span></span> | <span data-ttu-id="25e91-127">Описание</span><span class="sxs-lookup"><span data-stu-id="25e91-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="25e91-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="25e91-128">Authorization</span></span>  | <span data-ttu-id="25e91-129">string</span><span class="sxs-lookup"><span data-stu-id="25e91-129">string</span></span>  | <span data-ttu-id="25e91-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25e91-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25e91-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25e91-132">Request body</span></span>
<span data-ttu-id="25e91-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25e91-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25e91-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="25e91-134">Response</span></span>
<span data-ttu-id="25e91-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25e91-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25e91-136">Пример</span><span class="sxs-lookup"><span data-stu-id="25e91-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="25e91-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="25e91-137">Request</span></span>
<span data-ttu-id="25e91-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25e91-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25e91-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="25e91-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="25e91-140">C#</span><span class="sxs-lookup"><span data-stu-id="25e91-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25e91-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25e91-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25e91-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25e91-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25e91-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="25e91-143">Response</span></span>

<span data-ttu-id="25e91-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25e91-144">The following is an example of the response.</span></span>
><span data-ttu-id="25e91-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="25e91-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="25e91-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25e91-146">All the properties will be returned from an actual call.</span></span>
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
