---
title: Список registeredDevices
description: Получение списка зарегистрированных устройств пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: dde29d94209f29413cce5ddab5e67e89188803fb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721511"
---
# <a name="list-registereddevices"></a><span data-ttu-id="473bd-103">Список registeredDevices</span><span class="sxs-lookup"><span data-stu-id="473bd-103">List registeredDevices</span></span>

<span data-ttu-id="473bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="473bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="473bd-105">Получение списка зарегистрированных устройств пользователя.</span><span class="sxs-lookup"><span data-stu-id="473bd-105">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="473bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="473bd-106">Permissions</span></span>
<span data-ttu-id="473bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="473bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="473bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="473bd-109">Permission type</span></span>      | <span data-ttu-id="473bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="473bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="473bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="473bd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="473bd-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="473bd-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="473bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="473bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="473bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="473bd-114">Not supported.</span></span>    |
|<span data-ttu-id="473bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="473bd-115">Application</span></span> | <span data-ttu-id="473bd-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473bd-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="473bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="473bd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="473bd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="473bd-118">Optional query parameters</span></span>
<span data-ttu-id="473bd-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="473bd-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="473bd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="473bd-120">Request headers</span></span>
| <span data-ttu-id="473bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="473bd-121">Header</span></span>       | <span data-ttu-id="473bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="473bd-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="473bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="473bd-123">Authorization</span></span>  | <span data-ttu-id="473bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="473bd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="473bd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="473bd-126">Accept</span></span>  | <span data-ttu-id="473bd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="473bd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="473bd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="473bd-128">Request body</span></span>
<span data-ttu-id="473bd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="473bd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="473bd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="473bd-130">Response</span></span>

<span data-ttu-id="473bd-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="473bd-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="473bd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="473bd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="473bd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="473bd-133">Request</span></span>
<span data-ttu-id="473bd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="473bd-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="473bd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="473bd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/registeredDevices
```
# <a name="c"></a>[<span data-ttu-id="473bd-136">C#</span><span class="sxs-lookup"><span data-stu-id="473bd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registereddevices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="473bd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="473bd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registereddevices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="473bd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="473bd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registereddevices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="473bd-139">Java</span><span class="sxs-lookup"><span data-stu-id="473bd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registereddevices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="473bd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="473bd-140">Response</span></span>
<span data-ttu-id="473bd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="473bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
