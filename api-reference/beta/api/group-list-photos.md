---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 959c25bc9904a8145240f76baaf3271e29e17eef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502058"
---
# <a name="list-photos"></a><span data-ttu-id="c81b0-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="c81b0-103">List photos</span></span>
<span data-ttu-id="c81b0-104">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="c81b0-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c81b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c81b0-105">Permissions</span></span>
<span data-ttu-id="c81b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c81b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c81b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c81b0-108">Permission type</span></span>      | <span data-ttu-id="c81b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c81b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c81b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c81b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c81b0-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c81b0-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="c81b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c81b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c81b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c81b0-113">Not supported.</span></span>    |
|<span data-ttu-id="c81b0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c81b0-114">Application</span></span> | <span data-ttu-id="c81b0-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c81b0-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c81b0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c81b0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c81b0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c81b0-117">Optional query parameters</span></span>
<span data-ttu-id="c81b0-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c81b0-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c81b0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c81b0-119">Request headers</span></span>
| <span data-ttu-id="c81b0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c81b0-120">Name</span></span>       | <span data-ttu-id="c81b0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c81b0-121">Type</span></span> | <span data-ttu-id="c81b0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c81b0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c81b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c81b0-123">Authorization</span></span>  | <span data-ttu-id="c81b0-124">string</span><span class="sxs-lookup"><span data-stu-id="c81b0-124">string</span></span>  | <span data-ttu-id="c81b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c81b0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c81b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c81b0-127">Request body</span></span>
<span data-ttu-id="c81b0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c81b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c81b0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c81b0-129">Response</span></span>
<span data-ttu-id="c81b0-130">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c81b0-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c81b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c81b0-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c81b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c81b0-132">Request</span></span>
<span data-ttu-id="c81b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c81b0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="c81b0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c81b0-134">Response</span></span>
<span data-ttu-id="c81b0-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c81b0-135">The following is an example of the response.</span></span>
><span data-ttu-id="c81b0-136">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c81b0-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c81b0-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c81b0-137">All the properties will be returned from an actual call.</span></span>
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
