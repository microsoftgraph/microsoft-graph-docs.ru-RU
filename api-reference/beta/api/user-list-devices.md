---
title: Список пользователей устройств
description: Ознакомьтесь со списком пользователей устройств, которые поддерживают возможности рим проекта. Этот компонент включает возможность запуска приложения, или сообщение или отправки данных в приложение. После того как вы выполнять на мне вызов GET- и устройств, передайте идентификатор устройства для отправки команды на устройство.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509527"
---
# <a name="list-user-devices"></a><span data-ttu-id="214b0-105">Список пользователей устройств</span><span class="sxs-lookup"><span data-stu-id="214b0-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="214b0-106">Ознакомьтесь со списком пользователей устройств, которые поддерживают возможности рим проекта.</span><span class="sxs-lookup"><span data-stu-id="214b0-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="214b0-107">Этот компонент включает возможность запуска приложения, или сообщение или отправки данных в приложение.</span><span class="sxs-lookup"><span data-stu-id="214b0-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="214b0-108">После того как вы выполнять на мне вызов GET- и устройств, передайте идентификатор устройства для [отправки команды](send-device-command.md) на устройство.</span><span class="sxs-lookup"><span data-stu-id="214b0-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="214b0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="214b0-109">Permissions</span></span>

<span data-ttu-id="214b0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="214b0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="214b0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="214b0-112">Permission type</span></span>      | <span data-ttu-id="214b0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="214b0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="214b0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="214b0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="214b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214b0-115">Not supported.</span></span>    |
|<span data-ttu-id="214b0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="214b0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214b0-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="214b0-117">Device.Read</span></span>    |
|<span data-ttu-id="214b0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="214b0-118">Application</span></span> | <span data-ttu-id="214b0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214b0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="214b0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="214b0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="214b0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="214b0-121">Request headers</span></span>

| <span data-ttu-id="214b0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="214b0-122">Header</span></span> |<span data-ttu-id="214b0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="214b0-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="214b0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="214b0-124">Authorization</span></span>| <span data-ttu-id="214b0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="214b0-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="214b0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="214b0-127">Accept</span></span> | <span data-ttu-id="214b0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="214b0-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="214b0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="214b0-129">Request body</span></span>
<span data-ttu-id="214b0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="214b0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214b0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="214b0-131">Response</span></span>

<span data-ttu-id="214b0-132">В случае успеха этот метод возвращает код ответа 200 и свойств пользователя устройства в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="214b0-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="214b0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="214b0-133">Example</span></span>
<span data-ttu-id="214b0-134">В этом примере возвращается список устройств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="214b0-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="214b0-135">Для передачи команд устройство, с помощью `me/devices/{id}/command`, вам потребуется получить идентификатор устройства, который возвращается.</span><span class="sxs-lookup"><span data-stu-id="214b0-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="214b0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="214b0-136">Request</span></span>

<span data-ttu-id="214b0-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="214b0-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="214b0-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="214b0-138">Response</span></span>

<span data-ttu-id="214b0-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="214b0-139">The following is an example of the response.</span></span> <span data-ttu-id="214b0-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="214b0-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="214b0-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="214b0-141">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
