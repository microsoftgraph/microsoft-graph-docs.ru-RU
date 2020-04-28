---
title: Список registeredDevices
description: Получение списка зарегистрированных устройств пользователя.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 78a91f804b2153ff142a5b75f6b8508c60734459
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107593"
---
# <a name="list-registereddevices"></a><span data-ttu-id="3e2d5-103">Список registeredDevices</span><span class="sxs-lookup"><span data-stu-id="3e2d5-103">List registeredDevices</span></span>

<span data-ttu-id="3e2d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e2d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e2d5-105">Получение списка зарегистрированных устройств пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-105">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e2d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e2d5-106">Permissions</span></span>
<span data-ttu-id="3e2d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e2d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e2d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e2d5-109">Permission type</span></span>      | <span data-ttu-id="3e2d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e2d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e2d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e2d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e2d5-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e2d5-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e2d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e2d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e2d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-114">Not supported.</span></span>    |
|<span data-ttu-id="3e2d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e2d5-115">Application</span></span> | <span data-ttu-id="3e2d5-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e2d5-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3e2d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e2d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e2d5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e2d5-118">Optional query parameters</span></span>
<span data-ttu-id="3e2d5-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3e2d5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e2d5-120">Request headers</span></span>
| <span data-ttu-id="3e2d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e2d5-121">Header</span></span>       | <span data-ttu-id="3e2d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e2d5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e2d5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e2d5-123">Authorization</span></span>  | <span data-ttu-id="3e2d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3e2d5-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3e2d5-126">Accept</span></span>  | <span data-ttu-id="3e2d5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3e2d5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e2d5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e2d5-128">Request body</span></span>
<span data-ttu-id="3e2d5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e2d5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e2d5-130">Response</span></span>

<span data-ttu-id="3e2d5-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e2d5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3e2d5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e2d5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e2d5-133">Request</span></span>
<span data-ttu-id="3e2d5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e2d5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e2d5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/registeredDevices
```
# <a name="c"></a>[<span data-ttu-id="3e2d5-136">C#</span><span class="sxs-lookup"><span data-stu-id="3e2d5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registereddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e2d5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e2d5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registereddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e2d5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e2d5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registereddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3e2d5-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e2d5-139">Response</span></span>
<span data-ttu-id="3e2d5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e2d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
