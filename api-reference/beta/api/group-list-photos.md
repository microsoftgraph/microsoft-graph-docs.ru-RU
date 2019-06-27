---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 57676cff7fd85cb12c46f7da1294da3653766ca0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263030"
---
# <a name="list-photos"></a><span data-ttu-id="6d85c-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="6d85c-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d85c-104">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="6d85c-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d85c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d85c-105">Permissions</span></span>
<span data-ttu-id="6d85c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d85c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d85c-108">Permission type</span></span>      | <span data-ttu-id="6d85c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d85c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d85c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d85c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d85c-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d85c-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d85c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d85c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d85c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d85c-113">Not supported.</span></span>    |
|<span data-ttu-id="6d85c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d85c-114">Application</span></span> | <span data-ttu-id="6d85c-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d85c-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d85c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d85c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d85c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d85c-117">Optional query parameters</span></span>
<span data-ttu-id="6d85c-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6d85c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d85c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d85c-119">Request headers</span></span>
| <span data-ttu-id="6d85c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6d85c-120">Name</span></span>       | <span data-ttu-id="6d85c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6d85c-121">Type</span></span> | <span data-ttu-id="6d85c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6d85c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d85c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d85c-123">Authorization</span></span>  | <span data-ttu-id="6d85c-124">string</span><span class="sxs-lookup"><span data-stu-id="6d85c-124">string</span></span>  | <span data-ttu-id="6d85c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d85c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d85c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d85c-127">Request body</span></span>
<span data-ttu-id="6d85c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d85c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d85c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d85c-129">Response</span></span>
<span data-ttu-id="6d85c-130">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6d85c-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d85c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6d85c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6d85c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d85c-132">Request</span></span>
<span data-ttu-id="6d85c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d85c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="6d85c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d85c-134">Response</span></span>
<span data-ttu-id="6d85c-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d85c-135">The following is an example of the response.</span></span>
><span data-ttu-id="6d85c-136">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6d85c-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d85c-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d85c-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6d85c-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6d85c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6d85c-139">C#</span><span class="sxs-lookup"><span data-stu-id="6d85c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photos-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d85c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d85c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photos-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6d85c-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6d85c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photos-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
