---
title: Перечисление фотографий
description: Получение списка объектов profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 51c8ba85aa183b07c8e7497dbd2b64ded0b87ad0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951070"
---
# <a name="list-photos"></a><span data-ttu-id="aa373-103">Перечисление фотографий</span><span class="sxs-lookup"><span data-stu-id="aa373-103">List photos</span></span>

> <span data-ttu-id="aa373-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa373-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa373-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa373-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa373-106">Получение списка объектов [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="aa373-106">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa373-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa373-107">Permissions</span></span>
<span data-ttu-id="aa373-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa373-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa373-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa373-110">Permission type</span></span>      | <span data-ttu-id="aa373-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa373-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa373-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa373-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aa373-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa373-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa373-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa373-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa373-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa373-115">Not supported.</span></span>    |
|<span data-ttu-id="aa373-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa373-116">Application</span></span> | <span data-ttu-id="aa373-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa373-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa373-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa373-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa373-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa373-119">Optional query parameters</span></span>
<span data-ttu-id="aa373-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa373-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa373-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa373-121">Request headers</span></span>
| <span data-ttu-id="aa373-122">Имя</span><span class="sxs-lookup"><span data-stu-id="aa373-122">Name</span></span>       | <span data-ttu-id="aa373-123">Тип</span><span class="sxs-lookup"><span data-stu-id="aa373-123">Type</span></span> | <span data-ttu-id="aa373-124">Описание</span><span class="sxs-lookup"><span data-stu-id="aa373-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa373-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa373-125">Authorization</span></span>  | <span data-ttu-id="aa373-126">string</span><span class="sxs-lookup"><span data-stu-id="aa373-126">string</span></span>  | <span data-ttu-id="aa373-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa373-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa373-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa373-129">Request body</span></span>
<span data-ttu-id="aa373-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa373-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa373-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa373-131">Response</span></span>
<span data-ttu-id="aa373-132">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [profilePhoto](../resources/profilephoto.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aa373-132">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa373-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aa373-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aa373-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa373-134">Request</span></span>
<span data-ttu-id="aa373-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa373-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="aa373-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa373-136">Response</span></span>
<span data-ttu-id="aa373-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aa373-137">The following is an example of the response.</span></span>
><span data-ttu-id="aa373-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="aa373-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aa373-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa373-139">All the properties will be returned from an actual call.</span></span>
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
