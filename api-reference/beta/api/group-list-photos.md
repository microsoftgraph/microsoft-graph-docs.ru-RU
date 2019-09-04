---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7ce86133178a00a936893af2e585515964bf8cf9
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721595"
---
# <a name="list-photos"></a><span data-ttu-id="0e712-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="0e712-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e712-104">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="0e712-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e712-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e712-105">Permissions</span></span>
<span data-ttu-id="0e712-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e712-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e712-108">Permission type</span></span>      | <span data-ttu-id="0e712-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e712-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e712-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e712-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e712-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e712-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e712-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e712-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e712-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e712-113">Not supported.</span></span>    |
|<span data-ttu-id="0e712-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e712-114">Application</span></span> | <span data-ttu-id="0e712-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e712-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e712-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e712-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e712-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e712-117">Optional query parameters</span></span>
<span data-ttu-id="0e712-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0e712-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e712-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e712-119">Request headers</span></span>
| <span data-ttu-id="0e712-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0e712-120">Name</span></span>       | <span data-ttu-id="0e712-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0e712-121">Type</span></span> | <span data-ttu-id="0e712-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0e712-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e712-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e712-123">Authorization</span></span>  | <span data-ttu-id="0e712-124">string</span><span class="sxs-lookup"><span data-stu-id="0e712-124">string</span></span>  | <span data-ttu-id="0e712-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e712-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e712-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e712-127">Request body</span></span>
<span data-ttu-id="0e712-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e712-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e712-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e712-129">Response</span></span>
<span data-ttu-id="0e712-130">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0e712-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e712-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0e712-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0e712-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e712-132">Request</span></span>
<span data-ttu-id="0e712-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e712-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0e712-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e712-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0e712-135">C#</span><span class="sxs-lookup"><span data-stu-id="0e712-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e712-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e712-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0e712-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0e712-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e712-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e712-138">Response</span></span>
<span data-ttu-id="0e712-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e712-139">The following is an example of the response.</span></span>
><span data-ttu-id="0e712-140">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0e712-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0e712-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e712-141">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
