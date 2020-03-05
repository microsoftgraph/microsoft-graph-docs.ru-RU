---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dacef0feb1e97ad52502b0ad456bbf7cd2c92209
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419368"
---
# <a name="list-photos"></a><span data-ttu-id="146c4-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="146c4-103">List photos</span></span>

<span data-ttu-id="146c4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="146c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="146c4-105">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="146c4-105">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="146c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="146c4-106">Permissions</span></span>
<span data-ttu-id="146c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="146c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="146c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="146c4-109">Permission type</span></span>      | <span data-ttu-id="146c4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="146c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="146c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="146c4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="146c4-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="146c4-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="146c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="146c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="146c4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="146c4-114">Not supported.</span></span>    |
|<span data-ttu-id="146c4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="146c4-115">Application</span></span> | <span data-ttu-id="146c4-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="146c4-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="146c4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="146c4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="146c4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="146c4-118">Optional query parameters</span></span>
<span data-ttu-id="146c4-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="146c4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="146c4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="146c4-120">Request headers</span></span>
| <span data-ttu-id="146c4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="146c4-121">Name</span></span>       | <span data-ttu-id="146c4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="146c4-122">Type</span></span> | <span data-ttu-id="146c4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="146c4-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="146c4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="146c4-124">Authorization</span></span>  | <span data-ttu-id="146c4-125">string</span><span class="sxs-lookup"><span data-stu-id="146c4-125">string</span></span>  | <span data-ttu-id="146c4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="146c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="146c4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="146c4-128">Request body</span></span>
<span data-ttu-id="146c4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="146c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="146c4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="146c4-130">Response</span></span>
<span data-ttu-id="146c4-131">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="146c4-131">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="146c4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="146c4-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="146c4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="146c4-133">Request</span></span>
<span data-ttu-id="146c4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="146c4-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="146c4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="146c4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="c"></a>[<span data-ttu-id="146c4-136">C#</span><span class="sxs-lookup"><span data-stu-id="146c4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="146c4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="146c4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="146c4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="146c4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="146c4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="146c4-139">Response</span></span>
<span data-ttu-id="146c4-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="146c4-140">The following is an example of the response.</span></span>
><span data-ttu-id="146c4-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="146c4-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="146c4-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="146c4-142">All the properties will be returned from an actual call.</span></span>
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
