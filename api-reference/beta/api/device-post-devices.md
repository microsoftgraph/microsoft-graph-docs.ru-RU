---
title: Создание устройства
description: Создание нового устройства.
author: tfitzmac
ms.openlocfilehash: e2b52c67ee34df9a609fbb53972ee8b859e6889f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336143"
---
# <a name="create-device"></a><span data-ttu-id="6da04-103">Создание устройства</span><span class="sxs-lookup"><span data-stu-id="6da04-103">Create device</span></span>

> <span data-ttu-id="6da04-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6da04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6da04-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6da04-106">Создание нового устройства.</span><span class="sxs-lookup"><span data-stu-id="6da04-106">Create a new device.</span></span>
## <a name="permissions"></a><span data-ttu-id="6da04-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6da04-107">Permissions</span></span>
<span data-ttu-id="6da04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6da04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6da04-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6da04-110">Permission type</span></span>      | <span data-ttu-id="6da04-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6da04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6da04-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6da04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6da04-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6da04-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6da04-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6da04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6da04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da04-115">Not supported.</span></span>    |
|<span data-ttu-id="6da04-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6da04-116">Application</span></span> | <span data-ttu-id="6da04-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da04-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6da04-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6da04-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="6da04-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6da04-119">Request headers</span></span>
| <span data-ttu-id="6da04-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6da04-120">Name</span></span>       | <span data-ttu-id="6da04-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6da04-121">Type</span></span> | <span data-ttu-id="6da04-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6da04-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6da04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6da04-123">Authorization</span></span>  | <span data-ttu-id="6da04-124">string</span><span class="sxs-lookup"><span data-stu-id="6da04-124">string</span></span>  | <span data-ttu-id="6da04-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6da04-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6da04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6da04-127">Request body</span></span>
<span data-ttu-id="6da04-128">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6da04-128">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

<span data-ttu-id="6da04-129">Поскольку ресурсов **устройство** поддерживает [расширения](/graph/extensibility-overview), можно использовать `POST` операции и Добавление настраиваемых свойств с собственными данными в экземпляр устройства при его создании.</span><span class="sxs-lookup"><span data-stu-id="6da04-129">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the device instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="6da04-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6da04-130">Response</span></span>

<span data-ttu-id="6da04-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6da04-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6da04-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6da04-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6da04-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6da04-133">Request</span></span>
<span data-ttu-id="6da04-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6da04-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="6da04-135">Предоставьте в тексте запроса описание объекта [device](../resources/device.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6da04-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6da04-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6da04-136">Response</span></span>
<span data-ttu-id="6da04-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6da04-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6da04-140">См. также</span><span class="sxs-lookup"><span data-stu-id="6da04-140">See also</span></span>

- [<span data-ttu-id="6da04-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="6da04-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6da04-142">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6da04-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="6da04-143">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="6da04-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->