---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f0d56f9ada36261739e14c340b714eef1996f6b0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953885"
---
# <a name="list-photos"></a><span data-ttu-id="99918-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="99918-103">List photos</span></span>

<span data-ttu-id="99918-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99918-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99918-105">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="99918-105">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="99918-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99918-106">Permissions</span></span>
<span data-ttu-id="99918-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99918-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99918-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99918-109">Permission type</span></span>      | <span data-ttu-id="99918-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99918-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99918-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99918-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99918-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99918-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="99918-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99918-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99918-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99918-114">Not supported.</span></span>    |
|<span data-ttu-id="99918-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99918-115">Application</span></span> | <span data-ttu-id="99918-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99918-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99918-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99918-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99918-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="99918-118">Optional query parameters</span></span>
<span data-ttu-id="99918-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="99918-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99918-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99918-120">Request headers</span></span>
| <span data-ttu-id="99918-121">Имя</span><span class="sxs-lookup"><span data-stu-id="99918-121">Name</span></span>       | <span data-ttu-id="99918-122">Тип</span><span class="sxs-lookup"><span data-stu-id="99918-122">Type</span></span> | <span data-ttu-id="99918-123">Описание</span><span class="sxs-lookup"><span data-stu-id="99918-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99918-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="99918-124">Authorization</span></span>  | <span data-ttu-id="99918-125">string</span><span class="sxs-lookup"><span data-stu-id="99918-125">string</span></span>  | <span data-ttu-id="99918-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99918-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99918-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99918-128">Request body</span></span>
<span data-ttu-id="99918-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99918-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99918-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="99918-130">Response</span></span>
<span data-ttu-id="99918-131">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="99918-131">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99918-132">Пример</span><span class="sxs-lookup"><span data-stu-id="99918-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="99918-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="99918-133">Request</span></span>
<span data-ttu-id="99918-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99918-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99918-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="99918-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="c"></a>[<span data-ttu-id="99918-136">C#</span><span class="sxs-lookup"><span data-stu-id="99918-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99918-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99918-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99918-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99918-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99918-139">Java</span><span class="sxs-lookup"><span data-stu-id="99918-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photos-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="99918-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="99918-140">Response</span></span>
<span data-ttu-id="99918-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="99918-141">The following is an example of the response.</span></span>
><span data-ttu-id="99918-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99918-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


