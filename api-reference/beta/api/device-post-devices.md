---
title: Создание устройства
description: Создайте новое устройство.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bf003c6337e600810d4bc37f4b8bb97506d9348a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260916"
---
# <a name="create-device"></a><span data-ttu-id="e6d13-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="e6d13-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6d13-104">Создайте новое устройство.</span><span class="sxs-lookup"><span data-stu-id="e6d13-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6d13-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6d13-105">Permissions</span></span>
<span data-ttu-id="e6d13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6d13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e6d13-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6d13-108">Permission type</span></span>      | <span data-ttu-id="e6d13-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6d13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6d13-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6d13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6d13-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6d13-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6d13-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6d13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6d13-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6d13-113">Not supported.</span></span>    |
|<span data-ttu-id="e6d13-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6d13-114">Application</span></span> | <span data-ttu-id="e6d13-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6d13-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6d13-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6d13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="e6d13-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6d13-117">Request headers</span></span>
| <span data-ttu-id="e6d13-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e6d13-118">Name</span></span>       | <span data-ttu-id="e6d13-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e6d13-119">Type</span></span> | <span data-ttu-id="e6d13-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e6d13-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6d13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6d13-121">Authorization</span></span>  | <span data-ttu-id="e6d13-122">string</span><span class="sxs-lookup"><span data-stu-id="e6d13-122">string</span></span>  | <span data-ttu-id="e6d13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6d13-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6d13-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6d13-125">Request body</span></span>
<span data-ttu-id="e6d13-126">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6d13-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="e6d13-127">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавить настраиваемые свойства с собственными данными к экземпляру устройства при его создании.</span><span class="sxs-lookup"><span data-stu-id="e6d13-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="e6d13-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6d13-128">Response</span></span>

<span data-ttu-id="e6d13-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6d13-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6d13-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e6d13-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6d13-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6d13-131">Request</span></span>
<span data-ttu-id="e6d13-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6d13-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="e6d13-133">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6d13-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e6d13-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6d13-134">Response</span></span>
<span data-ttu-id="e6d13-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6d13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e6d13-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e6d13-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e6d13-139">C#</span><span class="sxs-lookup"><span data-stu-id="e6d13-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_device_from_devices-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6d13-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6d13-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_device_from_devices-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e6d13-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e6d13-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_device_from_devices-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="e6d13-142">См. также</span><span class="sxs-lookup"><span data-stu-id="e6d13-142">See also</span></span>

- [<span data-ttu-id="e6d13-143">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e6d13-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e6d13-144">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e6d13-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e6d13-145">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e6d13-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/device-post-devices.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/device-post-devices.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-post-devices.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
