---
title: Список транзитивных групп memberOf
description: Получение групп и административных единиц, участником которых является группа.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6d8907752b2350e018df879e825d38a944de3da8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396826"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="e777e-103">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="e777e-103">List group transitive memberOf</span></span>

<span data-ttu-id="e777e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e777e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e777e-105">Получение групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="e777e-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="e777e-106">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="e777e-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="e777e-107">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="e777e-107">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e777e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e777e-108">Permissions</span></span>

<span data-ttu-id="e777e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e777e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e777e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e777e-111">Permission type</span></span>      | <span data-ttu-id="e777e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e777e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e777e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e777e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e777e-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e777e-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e777e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e777e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e777e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e777e-116">Not supported.</span></span>    |
|<span data-ttu-id="e777e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e777e-117">Application</span></span> | <span data-ttu-id="e777e-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e777e-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e777e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e777e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e777e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e777e-120">Optional query parameters</span></span>
<span data-ttu-id="e777e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e777e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e777e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e777e-122">Request headers</span></span>
| <span data-ttu-id="e777e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e777e-123">Name</span></span>       | <span data-ttu-id="e777e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e777e-124">Type</span></span> | <span data-ttu-id="e777e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e777e-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e777e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e777e-126">Authorization</span></span>  | <span data-ttu-id="e777e-127">string</span><span class="sxs-lookup"><span data-stu-id="e777e-127">string</span></span>  | <span data-ttu-id="e777e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e777e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e777e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e777e-130">Request body</span></span>
<span data-ttu-id="e777e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e777e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e777e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e777e-132">Response</span></span>
<span data-ttu-id="e777e-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e777e-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e777e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e777e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e777e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e777e-135">Request</span></span>
<span data-ttu-id="e777e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e777e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e777e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e777e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="e777e-138">C#</span><span class="sxs-lookup"><span data-stu-id="e777e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e777e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e777e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e777e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e777e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e777e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e777e-141">Response</span></span>

<span data-ttu-id="e777e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e777e-142">The following is an example of the response.</span></span>
><span data-ttu-id="e777e-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e777e-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e777e-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e777e-144">All the properties will be returned from an actual call.</span></span>
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
