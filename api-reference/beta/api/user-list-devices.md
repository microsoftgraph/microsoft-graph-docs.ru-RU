---
title: Перечисление пользовательских устройств
description: Получите список пользовательских устройств, поддерживаю Project возможностей Рима. Это включает возможность запуска приложения, сообщения или отправки данных в приложение. После вызова GET для меня или устройств передайте в ID устройства команду на устройство.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b116213a285cc334d02a70ed94461b5cf6436eea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036298"
---
# <a name="list-user-devices"></a><span data-ttu-id="d0598-105">Перечисление пользовательских устройств</span><span class="sxs-lookup"><span data-stu-id="d0598-105">List user devices</span></span>

<span data-ttu-id="d0598-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0598-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0598-107">Получите список пользовательских устройств, поддерживаю Project возможностей Рима.</span><span class="sxs-lookup"><span data-stu-id="d0598-107">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="d0598-108">Это включает возможность запуска приложения, сообщения или отправки данных в приложение.</span><span class="sxs-lookup"><span data-stu-id="d0598-108">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="d0598-109">После вызова GET для меня или устройств передайте в ID устройства команду [на](send-device-command.md) устройство.</span><span class="sxs-lookup"><span data-stu-id="d0598-109">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0598-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0598-110">Permissions</span></span>

<span data-ttu-id="d0598-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0598-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d0598-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0598-113">Permission type</span></span>      | <span data-ttu-id="d0598-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0598-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0598-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0598-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d0598-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0598-116">Not supported.</span></span>    |
|<span data-ttu-id="d0598-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0598-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0598-118">Device.Read</span><span class="sxs-lookup"><span data-stu-id="d0598-118">Device.Read</span></span>    |
|<span data-ttu-id="d0598-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0598-119">Application</span></span> | <span data-ttu-id="d0598-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0598-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0598-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0598-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="d0598-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0598-122">Request headers</span></span>

| <span data-ttu-id="d0598-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0598-123">Header</span></span> |<span data-ttu-id="d0598-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d0598-124">Value</span></span>
|:----|:------|
|<span data-ttu-id="d0598-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0598-125">Authorization</span></span>| <span data-ttu-id="d0598-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0598-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d0598-128">Accept</span><span class="sxs-lookup"><span data-stu-id="d0598-128">Accept</span></span> | <span data-ttu-id="d0598-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d0598-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0598-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0598-130">Request body</span></span>
<span data-ttu-id="d0598-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0598-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0598-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0598-132">Response</span></span>

<span data-ttu-id="d0598-133">В случае успешной работы этот метод возвращает код ответа в 200 и свойства устройства пользователя в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d0598-133">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="d0598-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d0598-134">Example</span></span>
<span data-ttu-id="d0598-135">В этом примере будет возвращен список устройств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0598-135">This example will return the list of devices for a user.</span></span> <span data-ttu-id="d0598-136">Чтобы командовать устройством с помощью, необходимо получить `me/devices/{id}/command` ID возвращенного устройства.</span><span class="sxs-lookup"><span data-stu-id="d0598-136">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="d0598-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0598-137">Request</span></span>

<span data-ttu-id="d0598-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0598-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="d0598-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0598-139">Response</span></span>

<span data-ttu-id="d0598-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d0598-140">The following is an example of the response.</span></span> <span data-ttu-id="d0598-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0598-141">Note: The response object shown here might be shortened for readability.</span></span>

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


