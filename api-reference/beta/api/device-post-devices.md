---
title: Создание устройства
description: Создание нового устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ad0400a74deec35daa4e28f91cafde5310c65c1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640520"
---
# <a name="create-device"></a><span data-ttu-id="bf7a1-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="bf7a1-103">Create device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf7a1-104">Создание нового устройства.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-104">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf7a1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf7a1-105">Permissions</span></span>
<span data-ttu-id="bf7a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf7a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bf7a1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf7a1-108">Permission type</span></span>      | <span data-ttu-id="bf7a1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf7a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf7a1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf7a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bf7a1-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf7a1-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf7a1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf7a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf7a1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-113">Not supported.</span></span>    |
|<span data-ttu-id="bf7a1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf7a1-114">Application</span></span> | <span data-ttu-id="bf7a1-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf7a1-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf7a1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf7a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="bf7a1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf7a1-117">Request headers</span></span>
| <span data-ttu-id="bf7a1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bf7a1-118">Name</span></span>       | <span data-ttu-id="bf7a1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bf7a1-119">Type</span></span> | <span data-ttu-id="bf7a1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bf7a1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf7a1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf7a1-121">Authorization</span></span>  | <span data-ttu-id="bf7a1-122">строка</span><span class="sxs-lookup"><span data-stu-id="bf7a1-122">string</span></span>  | <span data-ttu-id="bf7a1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf7a1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf7a1-125">Request body</span></span>
<span data-ttu-id="bf7a1-126">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-126">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="bf7a1-127">Поскольку ресурсов **устройство** поддерживает [расширения](/graph/extensibility-overview), можно использовать `POST` операции и Добавление настраиваемых свойств с собственными данными в экземпляр устройства при его создании.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-127">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="bf7a1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf7a1-128">Response</span></span>

<span data-ttu-id="bf7a1-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-129">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf7a1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bf7a1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf7a1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf7a1-131">Request</span></span>
<span data-ttu-id="bf7a1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-132">Here is an example of the request.</span></span>
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
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```
<span data-ttu-id="bf7a1-133">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-133">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bf7a1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf7a1-134">Response</span></span>
<span data-ttu-id="bf7a1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bf7a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "key": "key-value"
    }
  ],
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="bf7a1-138">См. также</span><span class="sxs-lookup"><span data-stu-id="bf7a1-138">See also</span></span>

- [<span data-ttu-id="bf7a1-139">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="bf7a1-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bf7a1-140">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="bf7a1-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bf7a1-141">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="bf7a1-141">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/device-post-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
