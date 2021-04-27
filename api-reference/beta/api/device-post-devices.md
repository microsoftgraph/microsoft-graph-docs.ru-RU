---
title: Создание устройства
description: Создание нового устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2c316b2c6a4eac5e37d94b1182c3b3f5bfbce7c9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046946"
---
# <a name="create-device"></a><span data-ttu-id="bccee-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="bccee-103">Create device</span></span>

<span data-ttu-id="bccee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bccee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bccee-105">Создание нового устройства.</span><span class="sxs-lookup"><span data-stu-id="bccee-105">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="bccee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bccee-106">Permissions</span></span>
<span data-ttu-id="bccee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bccee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bccee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bccee-109">Permission type</span></span>      | <span data-ttu-id="bccee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bccee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bccee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bccee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bccee-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bccee-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bccee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bccee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bccee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bccee-114">Not supported.</span></span>    |
|<span data-ttu-id="bccee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bccee-115">Application</span></span> | <span data-ttu-id="bccee-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bccee-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bccee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bccee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="bccee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bccee-118">Request headers</span></span>
| <span data-ttu-id="bccee-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bccee-119">Name</span></span>       | <span data-ttu-id="bccee-120">Тип</span><span class="sxs-lookup"><span data-stu-id="bccee-120">Type</span></span> | <span data-ttu-id="bccee-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bccee-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bccee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bccee-122">Authorization</span></span>  | <span data-ttu-id="bccee-123">string</span><span class="sxs-lookup"><span data-stu-id="bccee-123">string</span></span>  | <span data-ttu-id="bccee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bccee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bccee-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bccee-126">Request body</span></span>
<span data-ttu-id="bccee-127">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bccee-127">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="bccee-128">Так как **ресурс устройства** поддерживает [расширения,](/graph/extensibility-overview)можно использовать операцию и добавлять настраиваемые свойства с собственными данными в экземпляр устройства `POST` при его создании.</span><span class="sxs-lookup"><span data-stu-id="bccee-128">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="bccee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bccee-129">Response</span></span>

<span data-ttu-id="bccee-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bccee-130">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bccee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bccee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bccee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bccee-132">Request</span></span>
<span data-ttu-id="bccee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bccee-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bccee-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bccee-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bccee-135">C#</span><span class="sxs-lookup"><span data-stu-id="bccee-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-device-from-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bccee-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bccee-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-device-from-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bccee-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bccee-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-device-from-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bccee-138">Java</span><span class="sxs-lookup"><span data-stu-id="bccee-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-device-from-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bccee-139">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bccee-139">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bccee-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bccee-140">Response</span></span>
<span data-ttu-id="bccee-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bccee-141">Here is an example of the response.</span></span> <span data-ttu-id="bccee-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bccee-142">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bccee-143">См. также</span><span class="sxs-lookup"><span data-stu-id="bccee-143">See also</span></span>

- [<span data-ttu-id="bccee-144">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="bccee-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bccee-145">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="bccee-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bccee-146">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="bccee-146">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


