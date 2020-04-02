---
title: Перечисление пользовательских устройств
description: Получение списка устройств пользователей, поддерживающих возможности Project Рим. Это включает в себя возможность запуска приложения или сообщения или отправки данных в приложение. Когда вы выполняете вызов GET на моих устройствах, передайте ему идентификатор устройства, чтобы отправить команду на устройство.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: acd31b5d5b115646716199842d862bf6637ea504
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107705"
---
# <a name="list-user-devices"></a><span data-ttu-id="d5a5a-105">Перечисление пользовательских устройств</span><span class="sxs-lookup"><span data-stu-id="d5a5a-105">List user devices</span></span>

<span data-ttu-id="d5a5a-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a5a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5a5a-107">Получение списка устройств пользователей, поддерживающих возможности Project Рим.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-107">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="d5a5a-108">Это включает в себя возможность запуска приложения или сообщения или отправки данных в приложение.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-108">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="d5a5a-109">Когда вы выполняете вызов GET на моих устройствах, передайте ему идентификатор устройства, чтобы [отправить команду](send-device-command.md) на устройство.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-109">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5a5a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a5a-110">Permissions</span></span>

<span data-ttu-id="d5a5a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a5a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5a5a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a5a-113">Permission type</span></span>      | <span data-ttu-id="d5a5a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5a5a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d5a5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-116">Not supported.</span></span>    |
|<span data-ttu-id="d5a5a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5a5a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5a5a-118">Device.Read</span><span class="sxs-lookup"><span data-stu-id="d5a5a-118">Device.Read</span></span>    |
|<span data-ttu-id="d5a5a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5a5a-119">Application</span></span> | <span data-ttu-id="d5a5a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5a5a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5a5a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="d5a5a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5a5a-122">Request headers</span></span>

| <span data-ttu-id="d5a5a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5a5a-123">Header</span></span> |<span data-ttu-id="d5a5a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d5a5a-124">Value</span></span>
|:----|:------|
|<span data-ttu-id="d5a5a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5a5a-125">Authorization</span></span>| <span data-ttu-id="d5a5a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d5a5a-128">Accept</span><span class="sxs-lookup"><span data-stu-id="d5a5a-128">Accept</span></span> | <span data-ttu-id="d5a5a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d5a5a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5a5a-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5a5a-130">Request body</span></span>
<span data-ttu-id="d5a5a-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5a5a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5a5a-132">Response</span></span>

<span data-ttu-id="d5a5a-133">В случае успешного выполнения этот метод возвращает код ответа 200 и свойства устройства пользователя в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-133">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="d5a5a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d5a5a-134">Example</span></span>
<span data-ttu-id="d5a5a-135">В этом примере возвращается список устройств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-135">This example will return the list of devices for a user.</span></span> <span data-ttu-id="d5a5a-136">Чтобы выполнить командное устройство `me/devices/{id}/command`с помощью, необходимо получить идентификатор возвращенного устройства.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-136">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="d5a5a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a5a-137">Request</span></span>

<span data-ttu-id="d5a5a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="d5a5a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a5a-139">Response</span></span>

<span data-ttu-id="d5a5a-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-140">The following is an example of the response.</span></span> <span data-ttu-id="d5a5a-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5a5a-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5a5a-142">All of the properties will be returned from an actual call.</span></span>

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
