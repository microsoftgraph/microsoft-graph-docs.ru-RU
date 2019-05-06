---
title: Группа списка memberOf
description: Получение групп и административных единиц, непосредственным участником которых является группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 311837236f20039178ee4865489a83baa9fd8c1a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592950"
---
# <a name="list-group-memberof"></a><span data-ttu-id="2b8b2-103">Группа списка memberOf</span><span class="sxs-lookup"><span data-stu-id="2b8b2-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b8b2-104">Получение групп и административных единиц, непосредственным участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="2b8b2-p101">Эта операция не является транзитивным. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2b8b2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b8b2-107">Permissions</span></span>

<span data-ttu-id="2b8b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b8b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b8b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b8b2-110">Permission type</span></span>      | <span data-ttu-id="2b8b2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b8b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b8b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b8b2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b8b2-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b8b2-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b8b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b8b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b8b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-115">Not supported.</span></span>    |
|<span data-ttu-id="2b8b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b8b2-116">Application</span></span> | <span data-ttu-id="2b8b2-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b8b2-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b8b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b8b2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b8b2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b8b2-119">Optional query parameters</span></span>
<span data-ttu-id="2b8b2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b8b2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b8b2-121">Request headers</span></span>
| <span data-ttu-id="2b8b2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2b8b2-122">Name</span></span>       | <span data-ttu-id="2b8b2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2b8b2-123">Type</span></span> | <span data-ttu-id="2b8b2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2b8b2-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b8b2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b8b2-125">Authorization</span></span>  | <span data-ttu-id="2b8b2-126">string</span><span class="sxs-lookup"><span data-stu-id="2b8b2-126">string</span></span>  | <span data-ttu-id="2b8b2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b8b2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b8b2-129">Request body</span></span>
<span data-ttu-id="2b8b2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b8b2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b8b2-131">Response</span></span>
<span data-ttu-id="2b8b2-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b8b2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2b8b2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b8b2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b8b2-134">Request</span></span>

<span data-ttu-id="2b8b2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="2b8b2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b8b2-136">Response</span></span>

<span data-ttu-id="2b8b2-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-137">The following is an example of the response.</span></span>
><span data-ttu-id="2b8b2-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2b8b2-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b8b2-139">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2b8b2-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="2b8b2-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2b8b2-141">Языках</span><span class="sxs-lookup"><span data-stu-id="2b8b2-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b8b2-142">Язык</span><span class="sxs-lookup"><span data-stu-id="2b8b2-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_memberof-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
