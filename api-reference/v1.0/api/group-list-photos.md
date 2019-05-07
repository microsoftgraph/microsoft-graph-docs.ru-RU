---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c7790daade10154732675835d80e212afb610e3d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614086"
---
# <a name="list-photos"></a><span data-ttu-id="d8810-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="d8810-103">List photos</span></span>
<span data-ttu-id="d8810-104">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="d8810-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8810-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8810-105">Permissions</span></span>
<span data-ttu-id="d8810-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8810-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8810-108">Permission type</span></span>      | <span data-ttu-id="d8810-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8810-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8810-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8810-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d8810-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8810-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="d8810-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8810-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8810-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8810-113">Not supported.</span></span>    |
|<span data-ttu-id="d8810-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8810-114">Application</span></span> | <span data-ttu-id="d8810-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8810-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8810-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8810-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8810-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8810-117">Optional query parameters</span></span>
<span data-ttu-id="d8810-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8810-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8810-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8810-119">Request headers</span></span>
| <span data-ttu-id="d8810-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d8810-120">Name</span></span>       | <span data-ttu-id="d8810-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d8810-121">Type</span></span> | <span data-ttu-id="d8810-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d8810-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8810-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8810-123">Authorization</span></span>  | <span data-ttu-id="d8810-124">string</span><span class="sxs-lookup"><span data-stu-id="d8810-124">string</span></span>  | <span data-ttu-id="d8810-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8810-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8810-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8810-127">Request body</span></span>
<span data-ttu-id="d8810-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8810-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8810-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8810-129">Response</span></span>
<span data-ttu-id="d8810-130">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d8810-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8810-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d8810-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d8810-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8810-132">Request</span></span>
<span data-ttu-id="d8810-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8810-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="d8810-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8810-134">Response</span></span>
<span data-ttu-id="d8810-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8810-135">The following is an example of the response.</span></span>
><span data-ttu-id="d8810-136">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8810-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8810-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8810-137">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d8810-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="d8810-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d8810-139">Языках</span><span class="sxs-lookup"><span data-stu-id="d8810-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photos-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8810-140">Язык</span><span class="sxs-lookup"><span data-stu-id="d8810-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photos-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
