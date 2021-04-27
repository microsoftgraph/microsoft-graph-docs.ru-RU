---
title: Список ownedDevices
description: Получение списка устройств, принадлежащих пользователю.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 08103ed5e2aac34a721ebc6f6b529e2d2a328b17
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048885"
---
# <a name="list-owneddevices"></a><span data-ttu-id="e8c66-103">Список ownedDevices</span><span class="sxs-lookup"><span data-stu-id="e8c66-103">List ownedDevices</span></span>

<span data-ttu-id="e8c66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8c66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8c66-105">Получение списка устройств, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="e8c66-105">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8c66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8c66-106">Permissions</span></span>
<span data-ttu-id="e8c66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8c66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8c66-109">Permission type</span></span>      | <span data-ttu-id="e8c66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8c66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8c66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8c66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e8c66-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8c66-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8c66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8c66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8c66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8c66-114">Not supported.</span></span>    |
|<span data-ttu-id="e8c66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8c66-115">Application</span></span> | <span data-ttu-id="e8c66-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8c66-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e8c66-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8c66-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8c66-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8c66-118">Optional query parameters</span></span>
<span data-ttu-id="e8c66-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8c66-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8c66-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8c66-120">Request headers</span></span>
| <span data-ttu-id="e8c66-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8c66-121">Header</span></span>       | <span data-ttu-id="e8c66-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8c66-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8c66-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8c66-123">Authorization</span></span>  | <span data-ttu-id="e8c66-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8c66-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8c66-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e8c66-126">Accept</span></span>  | <span data-ttu-id="e8c66-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8c66-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8c66-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8c66-128">Request body</span></span>
<span data-ttu-id="e8c66-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8c66-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8c66-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8c66-130">Response</span></span>

<span data-ttu-id="e8c66-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8c66-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8c66-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e8c66-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8c66-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8c66-133">Request</span></span>
<span data-ttu-id="e8c66-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8c66-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8c66-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8c66-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/ownedDevices
```
# <a name="c"></a>[<span data-ttu-id="e8c66-136">C#</span><span class="sxs-lookup"><span data-stu-id="e8c66-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owneddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8c66-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8c66-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owneddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8c66-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8c66-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owneddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8c66-139">Java</span><span class="sxs-lookup"><span data-stu-id="e8c66-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-owneddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8c66-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8c66-140">Response</span></span>
<span data-ttu-id="e8c66-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8c66-141">Here is an example of the response.</span></span> <span data-ttu-id="e8c66-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8c66-142">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
