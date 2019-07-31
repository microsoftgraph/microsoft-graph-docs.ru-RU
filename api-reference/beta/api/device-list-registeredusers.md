---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b1c2da5e82a1d054282b2d62085d5a1f56549b4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951402"
---
# <a name="list-registeredusers"></a><span data-ttu-id="786da-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="786da-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="786da-104">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="786da-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="786da-105">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="786da-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="786da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="786da-106">Permissions</span></span>
<span data-ttu-id="786da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="786da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="786da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="786da-109">Permission type</span></span>      | <span data-ttu-id="786da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="786da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="786da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="786da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="786da-112">Directory. Read. ALL или Directory. ReadWrite. ALL или Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="786da-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="786da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="786da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="786da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="786da-114">Not supported.</span></span> |
|<span data-ttu-id="786da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="786da-115">Application</span></span> | <span data-ttu-id="786da-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="786da-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="786da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="786da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="786da-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="786da-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="786da-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="786da-119">Optional query parameters</span></span>
<span data-ttu-id="786da-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="786da-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="786da-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="786da-121">Request headers</span></span>
| <span data-ttu-id="786da-122">Имя</span><span class="sxs-lookup"><span data-stu-id="786da-122">Name</span></span>       | <span data-ttu-id="786da-123">Тип</span><span class="sxs-lookup"><span data-stu-id="786da-123">Type</span></span> | <span data-ttu-id="786da-124">Описание</span><span class="sxs-lookup"><span data-stu-id="786da-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="786da-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="786da-125">Authorization</span></span>  | <span data-ttu-id="786da-126">string</span><span class="sxs-lookup"><span data-stu-id="786da-126">string</span></span>  | <span data-ttu-id="786da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="786da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="786da-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="786da-129">Request body</span></span>
<span data-ttu-id="786da-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="786da-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="786da-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="786da-131">Response</span></span>

<span data-ttu-id="786da-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="786da-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="786da-133">Пример</span><span class="sxs-lookup"><span data-stu-id="786da-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="786da-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="786da-134">Request</span></span>
<span data-ttu-id="786da-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="786da-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="786da-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="786da-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="786da-137">C#</span><span class="sxs-lookup"><span data-stu-id="786da-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="786da-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="786da-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="786da-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="786da-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="786da-140">Java</span><span class="sxs-lookup"><span data-stu-id="786da-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="786da-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="786da-141">Response</span></span>
<span data-ttu-id="786da-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="786da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
