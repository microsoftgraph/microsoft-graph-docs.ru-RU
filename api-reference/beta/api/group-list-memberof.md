---
title: Группа списка memberOf
description: Получение групп и административных единиц, непосредственным участником которых является группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 35b715e0ef24ad199b5d77d909a8561a97d176f2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263002"
---
# <a name="list-group-memberof"></a><span data-ttu-id="d7490-103">Группа списка memberOf</span><span class="sxs-lookup"><span data-stu-id="d7490-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7490-104">Получение групп и административных единиц, непосредственным участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="d7490-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="d7490-p101">Эта операция не является транзитивным. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="d7490-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d7490-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7490-107">Permissions</span></span>

<span data-ttu-id="d7490-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7490-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7490-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7490-110">Permission type</span></span>      | <span data-ttu-id="d7490-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7490-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7490-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7490-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7490-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7490-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7490-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7490-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7490-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7490-115">Not supported.</span></span>    |
|<span data-ttu-id="d7490-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7490-116">Application</span></span> | <span data-ttu-id="d7490-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7490-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7490-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7490-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7490-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7490-119">Optional query parameters</span></span>
<span data-ttu-id="d7490-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7490-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7490-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7490-121">Request headers</span></span>
| <span data-ttu-id="d7490-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d7490-122">Name</span></span>       | <span data-ttu-id="d7490-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d7490-123">Type</span></span> | <span data-ttu-id="d7490-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d7490-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7490-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7490-125">Authorization</span></span>  | <span data-ttu-id="d7490-126">string</span><span class="sxs-lookup"><span data-stu-id="d7490-126">string</span></span>  | <span data-ttu-id="d7490-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7490-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7490-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7490-129">Request body</span></span>
<span data-ttu-id="d7490-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7490-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7490-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7490-131">Response</span></span>
<span data-ttu-id="d7490-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7490-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7490-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d7490-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7490-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7490-134">Request</span></span>

<span data-ttu-id="d7490-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7490-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="d7490-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7490-136">Response</span></span>

<span data-ttu-id="d7490-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7490-137">The following is an example of the response.</span></span>
><span data-ttu-id="d7490-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d7490-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d7490-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7490-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d7490-140">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="d7490-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d7490-141">C#</span><span class="sxs-lookup"><span data-stu-id="d7490-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7490-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="d7490-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_memberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d7490-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d7490-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_memberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
