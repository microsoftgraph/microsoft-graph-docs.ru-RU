---
title: Создание устройства
description: Создание и регистрация нового устройства в организации.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 396d74e2ef423b8efd61877b1a2b1fd8fdeee371
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466713"
---
# <a name="create-device"></a><span data-ttu-id="e2065-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="e2065-103">Create device</span></span>

<span data-ttu-id="e2065-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2065-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e2065-105">Создание и регистрация нового устройства в организации.</span><span class="sxs-lookup"><span data-stu-id="e2065-105">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2065-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2065-106">Permissions</span></span>
<span data-ttu-id="e2065-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e2065-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2065-109">Permission type</span></span>      | <span data-ttu-id="e2065-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2065-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2065-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2065-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2065-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2065-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2065-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2065-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2065-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2065-114">Not supported.</span></span>    |
|<span data-ttu-id="e2065-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2065-115">Application</span></span> | <span data-ttu-id="e2065-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2065-116">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2065-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2065-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="e2065-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2065-118">Request headers</span></span>
| <span data-ttu-id="e2065-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e2065-119">Name</span></span>       | <span data-ttu-id="e2065-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e2065-120">Type</span></span> | <span data-ttu-id="e2065-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e2065-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2065-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2065-122">Authorization</span></span>  | <span data-ttu-id="e2065-123">string</span><span class="sxs-lookup"><span data-stu-id="e2065-123">string</span></span>  | <span data-ttu-id="e2065-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2065-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2065-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2065-126">Content-type</span></span> | <span data-ttu-id="e2065-127">string</span><span class="sxs-lookup"><span data-stu-id="e2065-127">string</span></span> | <span data-ttu-id="e2065-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2065-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2065-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2065-129">Request body</span></span>
<span data-ttu-id="e2065-130">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2065-130">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2065-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2065-131">Response</span></span>

<span data-ttu-id="e2065-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2065-132">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2065-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e2065-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2065-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2065-134">Request</span></span>
<span data-ttu-id="e2065-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2065-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2065-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2065-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
# <a name="c"></a>[<span data-ttu-id="e2065-137">C#</span><span class="sxs-lookup"><span data-stu-id="e2065-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2065-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2065-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2065-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2065-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2065-140">Java</span><span class="sxs-lookup"><span data-stu-id="e2065-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e2065-141">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2065-141">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e2065-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2065-142">Response</span></span>
<span data-ttu-id="e2065-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2065-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
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
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
