---
title: Перечисление пользовательских устройств
description: Получите список пользовательских устройств, поддерживаюных возможности Project Rome. Это включает возможность запуска приложения, сообщения или отправки данных в приложение. После вызова GET для меня или устройств передайте в ID устройства команду на устройство.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b1c2b884b00298fd2b79a85b0ed3fe8f412b2736
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721637"
---
# <a name="list-user-devices"></a><span data-ttu-id="fcda7-105">Перечисление пользовательских устройств</span><span class="sxs-lookup"><span data-stu-id="fcda7-105">List user devices</span></span>

<span data-ttu-id="fcda7-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcda7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcda7-107">Получите список пользовательских устройств, поддерживаюных возможности Project Rome.</span><span class="sxs-lookup"><span data-stu-id="fcda7-107">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="fcda7-108">Это включает возможность запуска приложения, сообщения или отправки данных в приложение.</span><span class="sxs-lookup"><span data-stu-id="fcda7-108">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="fcda7-109">После вызова GET для меня или устройств передайте в ID устройства команду [на](send-device-command.md) устройство.</span><span class="sxs-lookup"><span data-stu-id="fcda7-109">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcda7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcda7-110">Permissions</span></span>

<span data-ttu-id="fcda7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcda7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fcda7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcda7-113">Permission type</span></span>      | <span data-ttu-id="fcda7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcda7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcda7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcda7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fcda7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcda7-116">Not supported.</span></span>    |
|<span data-ttu-id="fcda7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcda7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcda7-118">Device.Read</span><span class="sxs-lookup"><span data-stu-id="fcda7-118">Device.Read</span></span>    |
|<span data-ttu-id="fcda7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcda7-119">Application</span></span> | <span data-ttu-id="fcda7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcda7-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcda7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcda7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="fcda7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcda7-122">Request headers</span></span>

| <span data-ttu-id="fcda7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcda7-123">Header</span></span> |<span data-ttu-id="fcda7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fcda7-124">Value</span></span>
|:----|:------|
|<span data-ttu-id="fcda7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcda7-125">Authorization</span></span>| <span data-ttu-id="fcda7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcda7-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="fcda7-128">Accept</span><span class="sxs-lookup"><span data-stu-id="fcda7-128">Accept</span></span> | <span data-ttu-id="fcda7-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fcda7-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcda7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcda7-130">Request body</span></span>
<span data-ttu-id="fcda7-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcda7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcda7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcda7-132">Response</span></span>

<span data-ttu-id="fcda7-133">В случае успешной работы этот метод возвращает код ответа в 200 и свойства устройства пользователя в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcda7-133">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a><span data-ttu-id="fcda7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="fcda7-134">Example</span></span>
<span data-ttu-id="fcda7-135">В этом примере будет возвращен список устройств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fcda7-135">This example will return the list of devices for a user.</span></span> <span data-ttu-id="fcda7-136">Чтобы командовать устройством с помощью, необходимо получить `me/devices/{id}/command` ID возвращенного устройства.</span><span class="sxs-lookup"><span data-stu-id="fcda7-136">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="fcda7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcda7-137">Request</span></span>

<span data-ttu-id="fcda7-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcda7-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="fcda7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcda7-139">Response</span></span>

<span data-ttu-id="fcda7-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcda7-140">The following is an example of the response.</span></span> <span data-ttu-id="fcda7-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fcda7-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fcda7-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcda7-142">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```


