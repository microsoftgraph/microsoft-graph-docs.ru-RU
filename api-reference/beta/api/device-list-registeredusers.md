---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1cf352b1ba3fcf8c5e76cf200fdfdaa9ef7cc46c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437172"
---
# <a name="list-registeredusers"></a><span data-ttu-id="328da-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="328da-103">List registeredUsers</span></span>

<span data-ttu-id="328da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="328da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="328da-105">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="328da-105">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="328da-106">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="328da-106">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="328da-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="328da-107">Permissions</span></span>
<span data-ttu-id="328da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="328da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="328da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="328da-110">Permission type</span></span>      | <span data-ttu-id="328da-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="328da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="328da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="328da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="328da-113">Directory.Read.All или Directory.ReadWrite.All или Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="328da-113">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="328da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="328da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="328da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="328da-115">Not supported.</span></span> |
|<span data-ttu-id="328da-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="328da-116">Application</span></span> | <span data-ttu-id="328da-117">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="328da-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="328da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="328da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="328da-119">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="328da-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="328da-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="328da-120">Optional query parameters</span></span>
<span data-ttu-id="328da-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="328da-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="328da-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="328da-122">Request headers</span></span>
| <span data-ttu-id="328da-123">Имя</span><span class="sxs-lookup"><span data-stu-id="328da-123">Name</span></span>       | <span data-ttu-id="328da-124">Тип</span><span class="sxs-lookup"><span data-stu-id="328da-124">Type</span></span> | <span data-ttu-id="328da-125">Описание</span><span class="sxs-lookup"><span data-stu-id="328da-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="328da-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="328da-126">Authorization</span></span>  | <span data-ttu-id="328da-127">string</span><span class="sxs-lookup"><span data-stu-id="328da-127">string</span></span>  | <span data-ttu-id="328da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="328da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="328da-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="328da-130">Request body</span></span>
<span data-ttu-id="328da-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="328da-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="328da-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="328da-132">Response</span></span>

<span data-ttu-id="328da-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="328da-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="328da-134">Пример</span><span class="sxs-lookup"><span data-stu-id="328da-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="328da-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="328da-135">Request</span></span>
<span data-ttu-id="328da-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="328da-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="328da-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="328da-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
# <a name="c"></a>[<span data-ttu-id="328da-138">C#</span><span class="sxs-lookup"><span data-stu-id="328da-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="328da-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="328da-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="328da-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="328da-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="328da-141">Java</span><span class="sxs-lookup"><span data-stu-id="328da-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="328da-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="328da-142">Response</span></span>
<span data-ttu-id="328da-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="328da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
