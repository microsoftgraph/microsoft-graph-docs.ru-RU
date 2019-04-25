---
title: Перечисление пользовательских устройств
description: Получение списка устройств пользователей, поддерживающих возможности Project Рим. Это включает в себя возможность запуска приложения или сообщения или отправки данных в приложение. Когда вы выполняете вызов GET на моих устройствах, передайте ему идентификатор устройства, чтобы отправить команду на устройство.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544297"
---
# <a name="list-user-devices"></a><span data-ttu-id="9e382-105">Перечисление пользовательских устройств</span><span class="sxs-lookup"><span data-stu-id="9e382-105">List user devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e382-106">Получение списка устройств пользователей, поддерживающих возможности Project Рим.</span><span class="sxs-lookup"><span data-stu-id="9e382-106">Get a list of user devices that support Project Rome capabilities.</span></span> <span data-ttu-id="9e382-107">Это включает в себя возможность запуска приложения или сообщения или отправки данных в приложение.</span><span class="sxs-lookup"><span data-stu-id="9e382-107">This includes the ability to launch an app, or message or send data to an application.</span></span> <span data-ttu-id="9e382-108">Когда вы выполняете вызов GET на моих устройствах, передайте ему идентификатор устройства, чтобы [отправить команду](send-device-command.md) на устройство.</span><span class="sxs-lookup"><span data-stu-id="9e382-108">After you do a GET call on me/devices, pass in the ID of the device to [send a command](send-device-command.md) to your device.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e382-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e382-109">Permissions</span></span>

<span data-ttu-id="9e382-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e382-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e382-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e382-112">Permission type</span></span>      | <span data-ttu-id="9e382-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e382-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e382-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e382-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9e382-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e382-115">Not supported.</span></span>    |
|<span data-ttu-id="9e382-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e382-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e382-117">Device.Read</span><span class="sxs-lookup"><span data-stu-id="9e382-117">Device.Read</span></span>    |
|<span data-ttu-id="9e382-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e382-118">Application</span></span> | <span data-ttu-id="9e382-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e382-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e382-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e382-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a><span data-ttu-id="9e382-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e382-121">Request headers</span></span>

| <span data-ttu-id="9e382-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e382-122">Header</span></span> |<span data-ttu-id="9e382-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9e382-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="9e382-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e382-124">Authorization</span></span>| <span data-ttu-id="9e382-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e382-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9e382-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9e382-127">Accept</span></span> | <span data-ttu-id="9e382-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9e382-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e382-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e382-129">Request body</span></span>
<span data-ttu-id="9e382-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e382-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e382-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e382-131">Response</span></span>

<span data-ttu-id="9e382-132">В случае успешного выполнения этот метод возвращает код ответа 200 и свойства устройства пользователя в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e382-132">If successful, this method returns a 200 response code and the user device properties in the response body.</span></span>

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

## <a name="example"></a><span data-ttu-id="9e382-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9e382-133">Example</span></span>
<span data-ttu-id="9e382-134">В этом примере возвращается список устройств для пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e382-134">This example will return the list of devices for a user.</span></span> <span data-ttu-id="9e382-135">Чтобы выполнить командное устройство `me/devices/{id}/command`с помощью, необходимо получить идентификатор возвращенного устройства.</span><span class="sxs-lookup"><span data-stu-id="9e382-135">To command a device using `me/devices/{id}/command`, you will need to get the ID of the device that is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="9e382-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e382-136">Request</span></span>

<span data-ttu-id="9e382-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e382-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="9e382-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e382-138">Response</span></span>

<span data-ttu-id="9e382-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e382-139">The following is an example of the response.</span></span> <span data-ttu-id="9e382-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9e382-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9e382-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e382-141">All of the properties will be returned from an actual call.</span></span>

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
