---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e679baba5dcdac47fb2a14d45555707afadddc7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434554"
---
# <a name="list-registeredusers"></a><span data-ttu-id="04322-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="04322-103">List registeredUsers</span></span>

<span data-ttu-id="04322-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04322-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04322-105">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="04322-105">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="04322-106">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="04322-106">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="04322-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04322-107">Permissions</span></span>
<span data-ttu-id="04322-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04322-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04322-110">Permission type</span></span>      | <span data-ttu-id="04322-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04322-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04322-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04322-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04322-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04322-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04322-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04322-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04322-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04322-115">Not supported.</span></span>    |
|<span data-ttu-id="04322-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04322-116">Application</span></span> | <span data-ttu-id="04322-117">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04322-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="04322-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04322-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="04322-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="04322-119">Optional query parameters</span></span>
<span data-ttu-id="04322-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="04322-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="04322-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04322-121">Request headers</span></span>
| <span data-ttu-id="04322-122">Имя</span><span class="sxs-lookup"><span data-stu-id="04322-122">Name</span></span>       | <span data-ttu-id="04322-123">Тип</span><span class="sxs-lookup"><span data-stu-id="04322-123">Type</span></span> | <span data-ttu-id="04322-124">Описание</span><span class="sxs-lookup"><span data-stu-id="04322-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="04322-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="04322-125">Authorization</span></span>  | <span data-ttu-id="04322-126">string</span><span class="sxs-lookup"><span data-stu-id="04322-126">string</span></span>  | <span data-ttu-id="04322-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04322-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04322-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04322-129">Request body</span></span>
<span data-ttu-id="04322-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04322-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04322-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="04322-131">Response</span></span>

<span data-ttu-id="04322-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04322-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04322-133">Пример</span><span class="sxs-lookup"><span data-stu-id="04322-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04322-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="04322-134">Request</span></span>
<span data-ttu-id="04322-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04322-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04322-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="04322-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
# <a name="c"></a>[<span data-ttu-id="04322-137">C#</span><span class="sxs-lookup"><span data-stu-id="04322-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04322-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04322-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04322-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04322-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04322-140">Java</span><span class="sxs-lookup"><span data-stu-id="04322-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="04322-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="04322-141">Response</span></span>
<span data-ttu-id="04322-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04322-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
