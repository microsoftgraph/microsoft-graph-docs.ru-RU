---
title: Список registeredDevices
description: Получение списка зарегистрированных устройств пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e11b39156f7a1c2a6f807c19b6ee474ca6113cbb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048878"
---
# <a name="list-registereddevices"></a><span data-ttu-id="eeaf4-103">Список registeredDevices</span><span class="sxs-lookup"><span data-stu-id="eeaf4-103">List registeredDevices</span></span>

<span data-ttu-id="eeaf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeaf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeaf4-105">Получение списка зарегистрированных устройств пользователя.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-105">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="eeaf4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eeaf4-106">Permissions</span></span>
<span data-ttu-id="eeaf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeaf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeaf4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeaf4-109">Permission type</span></span>      | <span data-ttu-id="eeaf4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeaf4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeaf4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeaf4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eeaf4-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eeaf4-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eeaf4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeaf4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeaf4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-114">Not supported.</span></span>    |
|<span data-ttu-id="eeaf4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeaf4-115">Application</span></span> | <span data-ttu-id="eeaf4-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeaf4-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="eeaf4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeaf4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eeaf4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eeaf4-118">Optional query parameters</span></span>
<span data-ttu-id="eeaf4-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eeaf4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eeaf4-120">Request headers</span></span>
| <span data-ttu-id="eeaf4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eeaf4-121">Header</span></span>       | <span data-ttu-id="eeaf4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eeaf4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eeaf4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeaf4-123">Authorization</span></span>  | <span data-ttu-id="eeaf4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eeaf4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="eeaf4-126">Accept</span></span>  | <span data-ttu-id="eeaf4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eeaf4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeaf4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eeaf4-128">Request body</span></span>
<span data-ttu-id="eeaf4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeaf4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeaf4-130">Response</span></span>

<span data-ttu-id="eeaf4-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eeaf4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="eeaf4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeaf4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeaf4-133">Request</span></span>
<span data-ttu-id="eeaf4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eeaf4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eeaf4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/registeredDevices
```
# <a name="c"></a>[<span data-ttu-id="eeaf4-136">C#</span><span class="sxs-lookup"><span data-stu-id="eeaf4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registereddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eeaf4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eeaf4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registereddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eeaf4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eeaf4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registereddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eeaf4-139">Java</span><span class="sxs-lookup"><span data-stu-id="eeaf4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registereddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eeaf4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeaf4-140">Response</span></span>
<span data-ttu-id="eeaf4-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-141">Here is an example of the response.</span></span> <span data-ttu-id="eeaf4-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eeaf4-142">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
