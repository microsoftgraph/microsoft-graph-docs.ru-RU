---
title: Создание устройства
description: Создание и регистрация нового устройства в организации.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 97203f2367b03a48d6cbf89f7ffaeb4d9d529795
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518093"
---
# <a name="create-device"></a><span data-ttu-id="e3b26-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="e3b26-103">Create device</span></span>

<span data-ttu-id="e3b26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3b26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3b26-105">Создание и регистрация нового устройства в организации.</span><span class="sxs-lookup"><span data-stu-id="e3b26-105">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3b26-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3b26-106">Permissions</span></span>
<span data-ttu-id="e3b26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3b26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e3b26-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3b26-109">Permission type</span></span>      | <span data-ttu-id="e3b26-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3b26-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3b26-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3b26-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e3b26-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3b26-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3b26-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3b26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3b26-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3b26-114">Not supported.</span></span>    |
|<span data-ttu-id="e3b26-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3b26-115">Application</span></span> | <span data-ttu-id="e3b26-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3b26-116">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3b26-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3b26-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="e3b26-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3b26-118">Request headers</span></span>
| <span data-ttu-id="e3b26-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e3b26-119">Name</span></span>       | <span data-ttu-id="e3b26-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e3b26-120">Type</span></span> | <span data-ttu-id="e3b26-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e3b26-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3b26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3b26-122">Authorization</span></span>  | <span data-ttu-id="e3b26-123">string</span><span class="sxs-lookup"><span data-stu-id="e3b26-123">string</span></span>  | <span data-ttu-id="e3b26-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3b26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3b26-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3b26-126">Content-type</span></span> | <span data-ttu-id="e3b26-127">string</span><span class="sxs-lookup"><span data-stu-id="e3b26-127">string</span></span> | <span data-ttu-id="e3b26-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e3b26-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3b26-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3b26-129">Request body</span></span>
<span data-ttu-id="e3b26-130">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3b26-130">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e3b26-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3b26-131">Response</span></span>

<span data-ttu-id="e3b26-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3b26-132">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3b26-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e3b26-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3b26-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3b26-134">Request</span></span>
<span data-ttu-id="e3b26-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3b26-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3b26-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3b26-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e3b26-137">C#</span><span class="sxs-lookup"><span data-stu-id="e3b26-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3b26-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3b26-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3b26-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3b26-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3b26-140">Java</span><span class="sxs-lookup"><span data-stu-id="e3b26-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e3b26-141">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3b26-141">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e3b26-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3b26-142">Response</span></span>
<span data-ttu-id="e3b26-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3b26-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
