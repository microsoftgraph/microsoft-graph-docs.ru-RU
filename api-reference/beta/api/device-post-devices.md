---
title: Создание устройства
description: Создайте новое устройство.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61570106a40d1635b036673d61e660cb64c2f40b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381807"
---
# <a name="create-device"></a><span data-ttu-id="42268-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="42268-103">Create device</span></span>

<span data-ttu-id="42268-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42268-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42268-105">Создайте новое устройство.</span><span class="sxs-lookup"><span data-stu-id="42268-105">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="42268-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42268-106">Permissions</span></span>
<span data-ttu-id="42268-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="42268-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42268-109">Permission type</span></span>      | <span data-ttu-id="42268-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42268-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42268-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42268-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42268-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42268-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42268-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42268-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42268-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42268-114">Not supported.</span></span>    |
|<span data-ttu-id="42268-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42268-115">Application</span></span> | <span data-ttu-id="42268-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42268-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42268-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42268-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="42268-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42268-118">Request headers</span></span>
| <span data-ttu-id="42268-119">Имя</span><span class="sxs-lookup"><span data-stu-id="42268-119">Name</span></span>       | <span data-ttu-id="42268-120">Тип</span><span class="sxs-lookup"><span data-stu-id="42268-120">Type</span></span> | <span data-ttu-id="42268-121">Описание</span><span class="sxs-lookup"><span data-stu-id="42268-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42268-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42268-122">Authorization</span></span>  | <span data-ttu-id="42268-123">string</span><span class="sxs-lookup"><span data-stu-id="42268-123">string</span></span>  | <span data-ttu-id="42268-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42268-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42268-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42268-126">Request body</span></span>
<span data-ttu-id="42268-127">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42268-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="42268-128">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавить настраиваемые свойства с собственными данными к экземпляру устройства при его создании.</span><span class="sxs-lookup"><span data-stu-id="42268-128">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="42268-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="42268-129">Response</span></span>

<span data-ttu-id="42268-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42268-130">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42268-131">Пример</span><span class="sxs-lookup"><span data-stu-id="42268-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42268-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="42268-132">Request</span></span>
<span data-ttu-id="42268-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42268-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42268-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="42268-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="42268-135">C#</span><span class="sxs-lookup"><span data-stu-id="42268-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42268-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42268-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42268-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42268-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="42268-138">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42268-138">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="42268-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="42268-139">Response</span></span>
<span data-ttu-id="42268-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42268-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="42268-143">См. также</span><span class="sxs-lookup"><span data-stu-id="42268-143">See also</span></span>

- [<span data-ttu-id="42268-144">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="42268-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="42268-145">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="42268-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="42268-146">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="42268-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
