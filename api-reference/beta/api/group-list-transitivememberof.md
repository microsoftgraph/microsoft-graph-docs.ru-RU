---
title: Список транзитивных групп memberOf
description: Получение групп и административных единиц, участником которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 87d0daf1f7b42666a19bffec3576ab68380333f7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592824"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="95438-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="95438-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95438-106">Получение групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="95438-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="95438-107">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="95438-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="95438-108">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="95438-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="95438-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95438-109">Permissions</span></span>

<span data-ttu-id="95438-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95438-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95438-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95438-112">Permission type</span></span>      | <span data-ttu-id="95438-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95438-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95438-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95438-114">Delegated (work or school account)</span></span> | <span data-ttu-id="95438-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95438-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95438-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95438-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95438-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95438-117">Not supported.</span></span>    |
|<span data-ttu-id="95438-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95438-118">Application</span></span> | <span data-ttu-id="95438-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95438-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95438-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95438-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95438-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="95438-121">Optional query parameters</span></span>
<span data-ttu-id="95438-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="95438-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95438-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95438-123">Request headers</span></span>
| <span data-ttu-id="95438-124">Имя</span><span class="sxs-lookup"><span data-stu-id="95438-124">Name</span></span>       | <span data-ttu-id="95438-125">Тип</span><span class="sxs-lookup"><span data-stu-id="95438-125">Type</span></span> | <span data-ttu-id="95438-126">Описание</span><span class="sxs-lookup"><span data-stu-id="95438-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="95438-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="95438-127">Authorization</span></span>  | <span data-ttu-id="95438-128">string</span><span class="sxs-lookup"><span data-stu-id="95438-128">string</span></span>  | <span data-ttu-id="95438-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95438-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95438-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95438-131">Request body</span></span>
<span data-ttu-id="95438-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95438-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95438-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="95438-133">Response</span></span>
<span data-ttu-id="95438-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95438-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95438-135">Пример</span><span class="sxs-lookup"><span data-stu-id="95438-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="95438-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="95438-136">Request</span></span>
<span data-ttu-id="95438-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95438-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="95438-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="95438-138">Response</span></span>

<span data-ttu-id="95438-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95438-139">The following is an example of the response.</span></span>
><span data-ttu-id="95438-140">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95438-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95438-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95438-141">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="95438-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="95438-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="95438-143">Языках</span><span class="sxs-lookup"><span data-stu-id="95438-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95438-144">Язык</span><span class="sxs-lookup"><span data-stu-id="95438-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_transitivememberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
