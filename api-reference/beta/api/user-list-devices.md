---
title: Список пользователей устройств
description: Ознакомьтесь со списком пользователей устройств, которые поддерживают возможности рим проекта. Этот компонент включает возможность запуска приложения, или сообщение или отправки данных в приложение. После того как вы выполнять на мне вызов GET- и устройств, передайте идентификатор устройства для отправки команды на устройство.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 04b67b770eec38d9e70a2263cd54212077335c85
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983543"
---
# <a name="list-user-devices"></a><span data-ttu-id="d6082-105">Список пользователей устройств</span><span class="sxs-lookup"><span data-stu-id="d6082-105">List user devices</span></span>

> <span data-ttu-id="d6082-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6082-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6082-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6082-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6082-108">Ознакомьтесь со списком пользователей устройств, которые поддерживают возможности рим проекта.</span><span class="sxs-lookup"><span data-stu-id="d6082-108">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="d6082-109">Этот компонент включает возможность запуска приложения, или сообщение или отправки данных в приложение.</span><span class="sxs-lookup"><span data-stu-id="d6082-109">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="d6082-110">После того как вы выполнять на мне вызов GET- и устройств, передайте идентификатор устройства для [отправки команды](send-device-command.md) на устройство.</span><span class="sxs-lookup"><span data-stu-id="d6082-110">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6082-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6082-111">Permissions</span></span>

<span data-ttu-id="d6082-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6082-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6082-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6082-114">Permission type</span></span>      | <span data-ttu-id="d6082-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6082-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6082-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6082-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d6082-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6082-117">Not supported.</span></span>    |
|<span data-ttu-id="d6082-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6082-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6082-119">Device.Read</span><span class="sxs-lookup"><span data-stu-id="d6082-119">Device.Read</span></span>    |
|<span data-ttu-id="d6082-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6082-120">Application</span></span> | <span data-ttu-id="d6082-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6082-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6082-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6082-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="d6082-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6082-123">Request headers</span></span>

| <span data-ttu-id="d6082-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6082-124">Header</span></span> |<span data-ttu-id="d6082-125">Значение</span><span class="sxs-lookup"><span data-stu-id="d6082-125">Value</span></span>
|:----|:------|
|<span data-ttu-id="d6082-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6082-126">Authorization</span></span>| <span data-ttu-id="d6082-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6082-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="d6082-129">Accept</span><span class="sxs-lookup"><span data-stu-id="d6082-129">Accept</span></span> | <span data-ttu-id="d6082-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d6082-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6082-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6082-131">Request body</span></span>
<span data-ttu-id="d6082-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6082-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6082-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6082-133">Response</span></span>

<span data-ttu-id="d6082-134">В случае успеха этот метод возвращает код ответа 200 и свойств пользователя устройства в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d6082-134">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="d6082-135">Пример</span><span class="sxs-lookup"><span data-stu-id="d6082-135">Example</span></span>
<span data-ttu-id="d6082-136">В этом примере возвращается список устройств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6082-136">This example will return the list of devices for a user.</span></span> <span data-ttu-id="d6082-137">Для передачи команд устройство, с помощью `me/devices/{id}/command`, вам потребуется получить идентификатор устройства, который возвращается.</span><span class="sxs-lookup"><span data-stu-id="d6082-137">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="d6082-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6082-138">Request</span></span>

<span data-ttu-id="d6082-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6082-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="d6082-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6082-140">Response</span></span>

<span data-ttu-id="d6082-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d6082-141">The following is an example of the response.</span></span> <span data-ttu-id="d6082-142">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d6082-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d6082-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6082-143">All of the properties will be returned from an actual call.</span></span>

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
