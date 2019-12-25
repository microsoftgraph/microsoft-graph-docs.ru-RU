---
title: Список ownedDevices
description: Получение списка устройств, принадлежащих пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1641bef934890ea74176965df0f6af7313951799
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870696"
---
# <a name="list-owneddevices"></a><span data-ttu-id="bbd75-103">Список ownedDevices</span><span class="sxs-lookup"><span data-stu-id="bbd75-103">List ownedDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbd75-104">Получение списка устройств, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="bbd75-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="bbd75-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd75-105">Permissions</span></span>
<span data-ttu-id="bbd75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbd75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbd75-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd75-108">Permission type</span></span>      | <span data-ttu-id="bbd75-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbd75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbd75-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbd75-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbd75-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bbd75-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bbd75-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbd75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbd75-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd75-113">Not supported.</span></span>    |
|<span data-ttu-id="bbd75-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbd75-114">Application</span></span> | <span data-ttu-id="bbd75-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbd75-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="bbd75-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbd75-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bbd75-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bbd75-117">Optional query parameters</span></span>
<span data-ttu-id="bbd75-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bbd75-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bbd75-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbd75-119">Request headers</span></span>
| <span data-ttu-id="bbd75-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbd75-120">Header</span></span>       | <span data-ttu-id="bbd75-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bbd75-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bbd75-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbd75-122">Authorization</span></span>  | <span data-ttu-id="bbd75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbd75-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bbd75-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bbd75-125">Accept</span></span>  | <span data-ttu-id="bbd75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbd75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbd75-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bbd75-127">Request body</span></span>
<span data-ttu-id="bbd75-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbd75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbd75-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbd75-129">Response</span></span>

<span data-ttu-id="bbd75-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bbd75-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bbd75-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bbd75-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbd75-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbd75-132">Request</span></span>
<span data-ttu-id="bbd75-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbd75-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bbd75-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbd75-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/ownedDevices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbd75-135">C#</span><span class="sxs-lookup"><span data-stu-id="bbd75-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owneddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbd75-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbd75-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owneddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bbd75-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbd75-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owneddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bbd75-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbd75-138">Response</span></span>
<span data-ttu-id="bbd75-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbd75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
