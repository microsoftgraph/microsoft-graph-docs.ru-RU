---
title: Список устройств
description: Получение списка объектов устройств, зарегистрированных в организации.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 432d7e263faab60a95084ca3d7aef6cb42f5884d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973409"
---
# <a name="list-devices"></a><span data-ttu-id="c37b1-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="c37b1-103">List devices</span></span>

<span data-ttu-id="c37b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c37b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c37b1-105">Получение списка объектов устройств, зарегистрированных в организации.</span><span class="sxs-lookup"><span data-stu-id="c37b1-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c37b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c37b1-106">Permissions</span></span>
<span data-ttu-id="c37b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c37b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c37b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c37b1-109">Permission type</span></span>      | <span data-ttu-id="c37b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c37b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c37b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c37b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c37b1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c37b1-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c37b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c37b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c37b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c37b1-114">Not supported.</span></span>    |
|<span data-ttu-id="c37b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c37b1-115">Application</span></span> | <span data-ttu-id="c37b1-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37b1-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c37b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c37b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c37b1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c37b1-118">Optional query parameters</span></span>
<span data-ttu-id="c37b1-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c37b1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c37b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c37b1-120">Request headers</span></span>
| <span data-ttu-id="c37b1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c37b1-121">Name</span></span>       | <span data-ttu-id="c37b1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c37b1-122">Type</span></span> | <span data-ttu-id="c37b1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c37b1-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c37b1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c37b1-124">Authorization</span></span>  | <span data-ttu-id="c37b1-125">string</span><span class="sxs-lookup"><span data-stu-id="c37b1-125">string</span></span>  | <span data-ttu-id="c37b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c37b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c37b1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c37b1-128">Request body</span></span>
<span data-ttu-id="c37b1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c37b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c37b1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c37b1-130">Response</span></span>

<span data-ttu-id="c37b1-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c37b1-131">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c37b1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c37b1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c37b1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c37b1-133">Request</span></span>
<span data-ttu-id="c37b1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c37b1-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c37b1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c37b1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="c37b1-136">C#</span><span class="sxs-lookup"><span data-stu-id="c37b1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c37b1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c37b1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c37b1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c37b1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c37b1-139">Java</span><span class="sxs-lookup"><span data-stu-id="c37b1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c37b1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c37b1-140">Response</span></span>
<span data-ttu-id="c37b1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c37b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

