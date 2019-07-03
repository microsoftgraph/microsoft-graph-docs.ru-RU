---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb9ab8f0176dc825222bd97d92f9fe69b356a494
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437252"
---
# <a name="list-registeredusers"></a><span data-ttu-id="c0fa1-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="c0fa1-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0fa1-104">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="c0fa1-105">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0fa1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0fa1-106">Permissions</span></span>
<span data-ttu-id="c0fa1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0fa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0fa1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0fa1-109">Permission type</span></span>      | <span data-ttu-id="c0fa1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0fa1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0fa1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0fa1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0fa1-112">Directory. Read. ALL или Directory. ReadWrite. ALL или Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c0fa1-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0fa1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0fa1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0fa1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-114">Not supported.</span></span> |
|<span data-ttu-id="c0fa1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0fa1-115">Application</span></span> | <span data-ttu-id="c0fa1-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fa1-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0fa1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0fa1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="c0fa1-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c0fa1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0fa1-119">Optional query parameters</span></span>
<span data-ttu-id="c0fa1-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c0fa1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0fa1-121">Request headers</span></span>
| <span data-ttu-id="c0fa1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c0fa1-122">Name</span></span>       | <span data-ttu-id="c0fa1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c0fa1-123">Type</span></span> | <span data-ttu-id="c0fa1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c0fa1-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0fa1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0fa1-125">Authorization</span></span>  | <span data-ttu-id="c0fa1-126">string</span><span class="sxs-lookup"><span data-stu-id="c0fa1-126">string</span></span>  | <span data-ttu-id="c0fa1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0fa1-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0fa1-129">Request body</span></span>
<span data-ttu-id="c0fa1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0fa1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0fa1-131">Response</span></span>

<span data-ttu-id="c0fa1-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0fa1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c0fa1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0fa1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0fa1-134">Request</span></span>
<span data-ttu-id="c0fa1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0fa1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0fa1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0fa1-137">C#</span><span class="sxs-lookup"><span data-stu-id="c0fa1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0fa1-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0fa1-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0fa1-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c0fa1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0fa1-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0fa1-140">Response</span></span>
<span data-ttu-id="c0fa1-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0fa1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
