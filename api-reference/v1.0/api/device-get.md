---
title: Получение устройства
description: Получение свойств и связей объекта устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e68966ebf5ba6b59aefea1b4660045d68e011aff
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434610"
---
# <a name="get-device"></a><span data-ttu-id="2b945-103">Вывод устройства</span><span class="sxs-lookup"><span data-stu-id="2b945-103">Get device</span></span>

<span data-ttu-id="2b945-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b945-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b945-105">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="2b945-105">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b945-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b945-106">Permissions</span></span>
<span data-ttu-id="2b945-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2b945-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b945-109">Permission type</span></span>      | <span data-ttu-id="2b945-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b945-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b945-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b945-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b945-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b945-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b945-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b945-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b945-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b945-114">Not supported.</span></span>    |
|<span data-ttu-id="2b945-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b945-115">Application</span></span> | <span data-ttu-id="2b945-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b945-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b945-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b945-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="2b945-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="2b945-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2b945-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b945-119">Optional query parameters</span></span>
<span data-ttu-id="2b945-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b945-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b945-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b945-121">Request headers</span></span>
| <span data-ttu-id="2b945-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2b945-122">Name</span></span>       | <span data-ttu-id="2b945-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2b945-123">Type</span></span> | <span data-ttu-id="2b945-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2b945-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2b945-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b945-125">Authorization</span></span>  | <span data-ttu-id="2b945-126">string</span><span class="sxs-lookup"><span data-stu-id="2b945-126">string</span></span>  | <span data-ttu-id="2b945-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b945-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b945-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b945-129">Request body</span></span>
<span data-ttu-id="2b945-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b945-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b945-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b945-131">Response</span></span>

<span data-ttu-id="2b945-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b945-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b945-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2b945-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b945-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b945-134">Request</span></span>
<span data-ttu-id="2b945-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b945-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b945-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b945-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="2b945-137">C#</span><span class="sxs-lookup"><span data-stu-id="2b945-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b945-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b945-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b945-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b945-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b945-140">Java</span><span class="sxs-lookup"><span data-stu-id="2b945-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b945-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b945-141">Response</span></span>
<span data-ttu-id="2b945-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b945-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
