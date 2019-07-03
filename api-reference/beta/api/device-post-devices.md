---
title: Создание устройства
description: Создайте новое устройство.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 88c21a7bc977b499c020fc55e2d4d53b229a01f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437231"
---
# <a name="create-device"></a><span data-ttu-id="53fc5-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="53fc5-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53fc5-104">Создайте новое устройство.</span><span class="sxs-lookup"><span data-stu-id="53fc5-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="53fc5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53fc5-105">Permissions</span></span>
<span data-ttu-id="53fc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="53fc5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53fc5-108">Permission type</span></span>      | <span data-ttu-id="53fc5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53fc5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53fc5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53fc5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53fc5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53fc5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53fc5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53fc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53fc5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53fc5-113">Not supported.</span></span>    |
|<span data-ttu-id="53fc5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53fc5-114">Application</span></span> | <span data-ttu-id="53fc5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53fc5-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53fc5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53fc5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="53fc5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53fc5-117">Request headers</span></span>
| <span data-ttu-id="53fc5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="53fc5-118">Name</span></span>       | <span data-ttu-id="53fc5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="53fc5-119">Type</span></span> | <span data-ttu-id="53fc5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="53fc5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53fc5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53fc5-121">Authorization</span></span>  | <span data-ttu-id="53fc5-122">string</span><span class="sxs-lookup"><span data-stu-id="53fc5-122">string</span></span>  | <span data-ttu-id="53fc5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53fc5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53fc5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53fc5-125">Request body</span></span>
<span data-ttu-id="53fc5-126">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53fc5-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="53fc5-127">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), вы можете использовать `POST` операцию и добавить настраиваемые свойства с собственными данными к экземпляру устройства при его создании.</span><span class="sxs-lookup"><span data-stu-id="53fc5-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="53fc5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="53fc5-128">Response</span></span>

<span data-ttu-id="53fc5-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53fc5-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53fc5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="53fc5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53fc5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="53fc5-131">Request</span></span>
<span data-ttu-id="53fc5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53fc5-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53fc5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="53fc5-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="53fc5-134">C#</span><span class="sxs-lookup"><span data-stu-id="53fc5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53fc5-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="53fc5-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53fc5-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="53fc5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="53fc5-137">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53fc5-137">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="53fc5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="53fc5-138">Response</span></span>
<span data-ttu-id="53fc5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="53fc5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="53fc5-142">См. также</span><span class="sxs-lookup"><span data-stu-id="53fc5-142">See also</span></span>

- [<span data-ttu-id="53fc5-143">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="53fc5-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="53fc5-144">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="53fc5-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="53fc5-145">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="53fc5-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
