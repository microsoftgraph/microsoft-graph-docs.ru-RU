---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 868fa7203af4cb8b821d0a69b3fb75e375499b14
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463995"
---
# <a name="list-registeredusers"></a><span data-ttu-id="5852f-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="5852f-103">List registeredUsers</span></span>

<span data-ttu-id="5852f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5852f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5852f-105">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="5852f-105">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="5852f-106">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="5852f-106">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="5852f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5852f-107">Permissions</span></span>
<span data-ttu-id="5852f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5852f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5852f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5852f-110">Permission type</span></span>      | <span data-ttu-id="5852f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5852f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5852f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5852f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5852f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5852f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5852f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5852f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5852f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5852f-115">Not supported.</span></span>    |
|<span data-ttu-id="5852f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5852f-116">Application</span></span> | <span data-ttu-id="5852f-117">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5852f-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5852f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5852f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5852f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5852f-119">Optional query parameters</span></span>
<span data-ttu-id="5852f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5852f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5852f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5852f-121">Request headers</span></span>
| <span data-ttu-id="5852f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5852f-122">Name</span></span>       | <span data-ttu-id="5852f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5852f-123">Type</span></span> | <span data-ttu-id="5852f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5852f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5852f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5852f-125">Authorization</span></span>  | <span data-ttu-id="5852f-126">string</span><span class="sxs-lookup"><span data-stu-id="5852f-126">string</span></span>  | <span data-ttu-id="5852f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5852f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5852f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5852f-129">Request body</span></span>
<span data-ttu-id="5852f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5852f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5852f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5852f-131">Response</span></span>

<span data-ttu-id="5852f-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5852f-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5852f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5852f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5852f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5852f-134">Request</span></span>
<span data-ttu-id="5852f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5852f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5852f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5852f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
# <a name="c"></a>[<span data-ttu-id="5852f-137">C#</span><span class="sxs-lookup"><span data-stu-id="5852f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5852f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5852f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5852f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5852f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5852f-140">Java</span><span class="sxs-lookup"><span data-stu-id="5852f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5852f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="5852f-141">Response</span></span>
<span data-ttu-id="5852f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5852f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
