---
title: Создание устройства
description: Создание и регистрация нового устройства в организации.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 37371e90bab46082c86664b3f6883a203e2448d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370692"
---
# <a name="create-device"></a><span data-ttu-id="3ef93-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="3ef93-103">Create device</span></span>

<span data-ttu-id="3ef93-104">Создание и регистрация нового устройства в организации.</span><span class="sxs-lookup"><span data-stu-id="3ef93-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ef93-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ef93-105">Permissions</span></span>
<span data-ttu-id="3ef93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ef93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ef93-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ef93-108">Permission type</span></span>      | <span data-ttu-id="3ef93-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ef93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ef93-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ef93-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ef93-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ef93-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ef93-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ef93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ef93-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ef93-113">Not supported.</span></span>    |
|<span data-ttu-id="3ef93-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ef93-114">Application</span></span> | <span data-ttu-id="3ef93-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ef93-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ef93-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ef93-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="3ef93-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ef93-117">Request headers</span></span>
| <span data-ttu-id="3ef93-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3ef93-118">Name</span></span>       | <span data-ttu-id="3ef93-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3ef93-119">Type</span></span> | <span data-ttu-id="3ef93-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3ef93-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ef93-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ef93-121">Authorization</span></span>  | <span data-ttu-id="3ef93-122">string</span><span class="sxs-lookup"><span data-stu-id="3ef93-122">string</span></span>  | <span data-ttu-id="3ef93-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ef93-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ef93-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ef93-125">Content-type</span></span> | <span data-ttu-id="3ef93-126">string</span><span class="sxs-lookup"><span data-stu-id="3ef93-126">string</span></span> | <span data-ttu-id="3ef93-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3ef93-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ef93-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ef93-128">Request body</span></span>
<span data-ttu-id="3ef93-129">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ef93-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ef93-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ef93-130">Response</span></span>

<span data-ttu-id="3ef93-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ef93-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ef93-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3ef93-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ef93-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ef93-133">Request</span></span>
<span data-ttu-id="3ef93-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ef93-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3ef93-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef93-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ef93-136">C#</span><span class="sxs-lookup"><span data-stu-id="3ef93-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ef93-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef93-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ef93-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3ef93-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3ef93-139">Java</span><span class="sxs-lookup"><span data-stu-id="3ef93-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3ef93-140">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ef93-140">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3ef93-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ef93-141">Response</span></span>
<span data-ttu-id="3ef93-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ef93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
