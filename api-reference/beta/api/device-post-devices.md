---
title: Создание устройства
description: Создайте новое устройство.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c019e092c102facc19bcf0503d983cd4fb257e77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996194"
---
# <a name="create-device"></a><span data-ttu-id="7d5f2-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="7d5f2-103">Create device</span></span>

<span data-ttu-id="7d5f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d5f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d5f2-105">Создайте новое устройство.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-105">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d5f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d5f2-106">Permissions</span></span>
<span data-ttu-id="7d5f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d5f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d5f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d5f2-109">Permission type</span></span>      | <span data-ttu-id="7d5f2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d5f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d5f2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d5f2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d5f2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d5f2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-114">Not supported.</span></span>    |
|<span data-ttu-id="7d5f2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d5f2-115">Application</span></span> | <span data-ttu-id="7d5f2-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d5f2-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d5f2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d5f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="7d5f2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d5f2-118">Request headers</span></span>
| <span data-ttu-id="7d5f2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d5f2-119">Name</span></span>       | <span data-ttu-id="7d5f2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7d5f2-120">Type</span></span> | <span data-ttu-id="7d5f2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7d5f2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d5f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d5f2-122">Authorization</span></span>  | <span data-ttu-id="7d5f2-123">string</span><span class="sxs-lookup"><span data-stu-id="7d5f2-123">string</span></span>  | <span data-ttu-id="7d5f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d5f2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d5f2-126">Request body</span></span>
<span data-ttu-id="7d5f2-127">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="7d5f2-128">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавить настраиваемые свойства с собственными данными к экземпляру устройства при его создании.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-128">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="7d5f2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d5f2-129">Response</span></span>

<span data-ttu-id="7d5f2-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-130">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d5f2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d5f2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d5f2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d5f2-132">Request</span></span>
<span data-ttu-id="7d5f2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d5f2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d5f2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/beta/devices
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
# <a name="c"></a>[<span data-ttu-id="7d5f2-135">C#</span><span class="sxs-lookup"><span data-stu-id="7d5f2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d5f2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d5f2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d5f2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d5f2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7d5f2-138">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-138">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7d5f2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d5f2-139">Response</span></span>
<span data-ttu-id="7d5f2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 364

{
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "type": 99,
      "identityProvider": "identityProvider-value",
      "key": "base64Y3YxN2E1MWFlYw=="
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="7d5f2-143">См. также</span><span class="sxs-lookup"><span data-stu-id="7d5f2-143">See also</span></span>

- [<span data-ttu-id="7d5f2-144">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7d5f2-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7d5f2-145">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7d5f2-146">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


