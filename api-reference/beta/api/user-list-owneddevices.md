---
title: Список ownedDevices
description: Получение списка устройств, принадлежащих пользователю.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: f4750a0ad3dbf4c98bb3b65cc354416b67fefc0d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967335"
---
# <a name="list-owneddevices"></a><span data-ttu-id="1c84e-103">Список ownedDevices</span><span class="sxs-lookup"><span data-stu-id="1c84e-103">List ownedDevices</span></span>

<span data-ttu-id="1c84e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c84e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c84e-105">Получение списка устройств, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="1c84e-105">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c84e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c84e-106">Permissions</span></span>
<span data-ttu-id="1c84e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c84e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c84e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c84e-109">Permission type</span></span>      | <span data-ttu-id="1c84e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c84e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c84e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c84e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c84e-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c84e-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c84e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c84e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c84e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c84e-114">Not supported.</span></span>    |
|<span data-ttu-id="1c84e-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1c84e-115">Application</span></span> | <span data-ttu-id="1c84e-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c84e-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1c84e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c84e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c84e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1c84e-118">Optional query parameters</span></span>
<span data-ttu-id="1c84e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1c84e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c84e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c84e-120">Request headers</span></span>
| <span data-ttu-id="1c84e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c84e-121">Header</span></span>       | <span data-ttu-id="1c84e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c84e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c84e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c84e-123">Authorization</span></span>  | <span data-ttu-id="1c84e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c84e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1c84e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1c84e-126">Accept</span></span>  | <span data-ttu-id="1c84e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1c84e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c84e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c84e-128">Request body</span></span>
<span data-ttu-id="1c84e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c84e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c84e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c84e-130">Response</span></span>

<span data-ttu-id="1c84e-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c84e-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c84e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1c84e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c84e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c84e-133">Request</span></span>
<span data-ttu-id="1c84e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c84e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c84e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c84e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/ownedDevices
```
# <a name="c"></a>[<span data-ttu-id="1c84e-136">C#</span><span class="sxs-lookup"><span data-stu-id="1c84e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owneddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c84e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c84e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owneddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c84e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c84e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owneddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c84e-139">Java</span><span class="sxs-lookup"><span data-stu-id="1c84e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-owneddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1c84e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c84e-140">Response</span></span>
<span data-ttu-id="1c84e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c84e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
