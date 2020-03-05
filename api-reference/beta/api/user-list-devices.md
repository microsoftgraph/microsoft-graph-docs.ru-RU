---
title: Перечисление пользовательских устройств
description: Получение списка устройств пользователей, поддерживающих возможности Project Рим. Это включает в себя возможность запуска приложения или сообщения или отправки данных в приложение. Когда вы выполняете вызов GET на моих устройствах, передайте ему идентификатор устройства, чтобы отправить команду на устройство.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f98c50cd82bb3c79eca9d6172a0e5d3fc4074a0a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451849"
---
# <a name="list-user-devices"></a><span data-ttu-id="49cce-105">Перечисление пользовательских устройств</span><span class="sxs-lookup"><span data-stu-id="49cce-105">List user devices</span></span>

<span data-ttu-id="49cce-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="49cce-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49cce-107">Получение списка устройств пользователей, поддерживающих возможности Project Рим.</span><span class="sxs-lookup"><span data-stu-id="49cce-107">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="49cce-108">Это включает в себя возможность запуска приложения или сообщения или отправки данных в приложение.</span><span class="sxs-lookup"><span data-stu-id="49cce-108">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="49cce-109">Когда вы выполняете вызов GET на моих устройствах, передайте ему идентификатор устройства, чтобы [отправить команду](send-device-command.md) на устройство.</span><span class="sxs-lookup"><span data-stu-id="49cce-109">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="49cce-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49cce-110">Permissions</span></span>

<span data-ttu-id="49cce-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49cce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="49cce-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49cce-113">Permission type</span></span>      | <span data-ttu-id="49cce-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49cce-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49cce-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49cce-115">Delegated (work or school account)</span></span> | <span data-ttu-id="49cce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49cce-116">Not supported.</span></span>    |
|<span data-ttu-id="49cce-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49cce-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49cce-118">Device.Read</span><span class="sxs-lookup"><span data-stu-id="49cce-118">Device.Read</span></span>    |
|<span data-ttu-id="49cce-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49cce-119">Application</span></span> | <span data-ttu-id="49cce-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49cce-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49cce-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49cce-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="49cce-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49cce-122">Request headers</span></span>

| <span data-ttu-id="49cce-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49cce-123">Header</span></span> |<span data-ttu-id="49cce-124">Значение</span><span class="sxs-lookup"><span data-stu-id="49cce-124">Value</span></span>
|:----|:------|
|<span data-ttu-id="49cce-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49cce-125">Authorization</span></span>| <span data-ttu-id="49cce-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49cce-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="49cce-128">Accept</span><span class="sxs-lookup"><span data-stu-id="49cce-128">Accept</span></span> | <span data-ttu-id="49cce-129">application/json</span><span class="sxs-lookup"><span data-stu-id="49cce-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="49cce-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49cce-130">Request body</span></span>
<span data-ttu-id="49cce-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49cce-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49cce-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="49cce-132">Response</span></span>

<span data-ttu-id="49cce-133">В случае успешного выполнения этот метод возвращает код ответа 200 и свойства устройства пользователя в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49cce-133">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="49cce-134">Пример</span><span class="sxs-lookup"><span data-stu-id="49cce-134">Example</span></span>
<span data-ttu-id="49cce-135">В этом примере возвращается список устройств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="49cce-135">This example will return the list of devices for a user.</span></span> <span data-ttu-id="49cce-136">Чтобы выполнить командное устройство `me/devices/{id}/command`с помощью, необходимо получить идентификатор возвращенного устройства.</span><span class="sxs-lookup"><span data-stu-id="49cce-136">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="49cce-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="49cce-137">Request</span></span>

<span data-ttu-id="49cce-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49cce-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="49cce-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="49cce-139">Response</span></span>

<span data-ttu-id="49cce-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49cce-140">The following is an example of the response.</span></span> <span data-ttu-id="49cce-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="49cce-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="49cce-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49cce-142">All of the properties will be returned from an actual call.</span></span>

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
