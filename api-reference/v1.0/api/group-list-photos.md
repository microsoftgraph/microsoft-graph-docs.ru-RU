---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: dkershaw10
ms.openlocfilehash: fda70cc81e0a98f8527e8bd00e980a5092804f6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353706"
---
# <a name="list-photos"></a><span data-ttu-id="2255f-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="2255f-103">List photos</span></span>
<span data-ttu-id="2255f-104">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="2255f-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2255f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2255f-105">Permissions</span></span>
<span data-ttu-id="2255f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2255f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2255f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2255f-108">Permission type</span></span>      | <span data-ttu-id="2255f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2255f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2255f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2255f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2255f-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2255f-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="2255f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2255f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2255f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2255f-113">Not supported.</span></span>    |
|<span data-ttu-id="2255f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2255f-114">Application</span></span> | <span data-ttu-id="2255f-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2255f-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2255f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2255f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2255f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2255f-117">Optional query parameters</span></span>
<span data-ttu-id="2255f-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2255f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2255f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2255f-119">Request headers</span></span>
| <span data-ttu-id="2255f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2255f-120">Name</span></span>       | <span data-ttu-id="2255f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2255f-121">Type</span></span> | <span data-ttu-id="2255f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2255f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2255f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2255f-123">Authorization</span></span>  | <span data-ttu-id="2255f-124">string</span><span class="sxs-lookup"><span data-stu-id="2255f-124">string</span></span>  | <span data-ttu-id="2255f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2255f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2255f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2255f-127">Request body</span></span>
<span data-ttu-id="2255f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2255f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2255f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2255f-129">Response</span></span>
<span data-ttu-id="2255f-130">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2255f-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2255f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2255f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2255f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2255f-132">Request</span></span>
<span data-ttu-id="2255f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2255f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="2255f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2255f-134">Response</span></span>
<span data-ttu-id="2255f-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2255f-135">The following is an example of the response.</span></span>
><span data-ttu-id="2255f-136">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="2255f-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2255f-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2255f-137">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
