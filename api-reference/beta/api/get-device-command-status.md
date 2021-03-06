---
title: Получение состояния команд для устройства
description: Получите состояние команды на устройстве. Полный список кодов состояния см. в списке actionStatus.
localization_priority: Normal
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: c0747438a9921f2ed6f3ccf1ee551f4aced70fcb
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515970"
---
# <a name="get-device-command-status"></a><span data-ttu-id="f5372-104">Получение состояния команд для устройства</span><span class="sxs-lookup"><span data-stu-id="f5372-104">Get device command status</span></span>

<span data-ttu-id="f5372-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5372-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5372-106">Получите состояние команды на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f5372-106">Get the status of a command on a device.</span></span> <span data-ttu-id="f5372-107">Полный список кодов состояния см. [в списке actionStatus.](#list-of-actionstatus)</span><span class="sxs-lookup"><span data-stu-id="f5372-107">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5372-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5372-108">Permissions</span></span>

<span data-ttu-id="f5372-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5372-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5372-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5372-111">Permission type</span></span>      | <span data-ttu-id="f5372-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5372-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5372-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5372-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f5372-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5372-114">Not supported.</span></span>    |
|<span data-ttu-id="f5372-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5372-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5372-116">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f5372-116">Device.Command</span></span>    |
|<span data-ttu-id="f5372-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5372-117">Application</span></span> | <span data-ttu-id="f5372-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5372-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5372-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5372-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5372-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5372-120">Request headers</span></span>

| <span data-ttu-id="f5372-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5372-121">Header</span></span> |<span data-ttu-id="f5372-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f5372-122">Value</span></span>
|:----|:------|
|<span data-ttu-id="f5372-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5372-123">Authorization</span></span>| <span data-ttu-id="f5372-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5372-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f5372-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f5372-126">Accept</span></span> | <span data-ttu-id="f5372-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f5372-127">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="f5372-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5372-128">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a><span data-ttu-id="f5372-129">Список действийStatus</span><span class="sxs-lookup"><span data-stu-id="f5372-129">List of actionStatus</span></span>

- <span data-ttu-id="f5372-130">запрос, // Команда создана и ожидает обработки</span><span class="sxs-lookup"><span data-stu-id="f5372-130">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="f5372-131">sentToTarget, // Команда отправлена на целевое устройство</span><span class="sxs-lookup"><span data-stu-id="f5372-131">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="f5372-132">выполнение, // Целевое устройство признало получение команды и выполняет ее</span><span class="sxs-lookup"><span data-stu-id="f5372-132">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="f5372-133">завершено,// Выполнено выполнение команды</span><span class="sxs-lookup"><span data-stu-id="f5372-133">completed, // Command execution completed</span></span>
- <span data-ttu-id="f5372-134">failedToSend, // Служба не отправила команду на целевое устройство</span><span class="sxs-lookup"><span data-stu-id="f5372-134">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="f5372-135">executionFailed, // Выполнение команды не удалось</span><span class="sxs-lookup"><span data-stu-id="f5372-135">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="f5372-136">commandDropped, // Команда отброшена клиентом, если устройство находится в состоянии ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="f5372-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="f5372-137">отмена, // Отмена команды</span><span class="sxs-lookup"><span data-stu-id="f5372-137">cancel, // Cancel the command</span></span>
- <span data-ttu-id="f5372-138">отмена, // Отмена команды</span><span class="sxs-lookup"><span data-stu-id="f5372-138">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="f5372-139">отменено, // Команда отменена</span><span class="sxs-lookup"><span data-stu-id="f5372-139">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="f5372-140">retry, // Служба повторно отправляет команду в целевой адрес</span><span class="sxs-lookup"><span data-stu-id="f5372-140">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="f5372-141">истек, // Обработка команд превысила срок действия</span><span class="sxs-lookup"><span data-stu-id="f5372-141">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="f5372-142">ошибка, // Внутренняя ошибка при обработке команды</span><span class="sxs-lookup"><span data-stu-id="f5372-142">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="f5372-143">настраиваемый // Настраиваемый статус</span><span class="sxs-lookup"><span data-stu-id="f5372-143">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="f5372-144">Пример</span><span class="sxs-lookup"><span data-stu-id="f5372-144">Example</span></span>

<span data-ttu-id="f5372-145">В этом примере вам потребуется ID устройства и ID команды, которая была выдана устройству.</span><span class="sxs-lookup"><span data-stu-id="f5372-145">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f5372-146">ID устройства возвращается при выдаче вызова GET, а командный ID возвращается при вызове `/me/devices` `/me/devices/{id}/command` POST.</span><span class="sxs-lookup"><span data-stu-id="f5372-146">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f5372-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5372-147">Request</span></span>

<span data-ttu-id="f5372-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5372-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f5372-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5372-149">Response</span></span>

<span data-ttu-id="f5372-150">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5372-150">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a><span data-ttu-id="f5372-151">Получить командную нагрузку</span><span class="sxs-lookup"><span data-stu-id="f5372-151">Get command payload</span></span>

<span data-ttu-id="f5372-152">Получите полезное устройство для определенного действия на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f5372-152">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="f5372-153">Полезной нагрузки ответа используется при запросе службы приложения для переноса данных обратно.</span><span class="sxs-lookup"><span data-stu-id="f5372-153">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="f5372-154">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5372-154">Permissions</span></span>

<span data-ttu-id="f5372-p107">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5372-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5372-157">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5372-157">Permission type</span></span>      | <span data-ttu-id="f5372-158">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5372-158">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5372-159">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5372-159">Delegated (work or school account)</span></span> | <span data-ttu-id="f5372-160">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5372-160">Not supported.</span></span>    |
|<span data-ttu-id="f5372-161">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5372-161">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5372-162">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f5372-162">Device.Command</span></span>    |
|<span data-ttu-id="f5372-163">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5372-163">Application</span></span> | <span data-ttu-id="f5372-164">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5372-164">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="f5372-165">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5372-165">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="f5372-166">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5372-166">Request headers</span></span>

| <span data-ttu-id="f5372-167">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5372-167">Header</span></span> |<span data-ttu-id="f5372-168">Значение</span><span class="sxs-lookup"><span data-stu-id="f5372-168">Value</span></span>
|:----|:------|
|<span data-ttu-id="f5372-169">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5372-169">Authorization</span></span>| <span data-ttu-id="f5372-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5372-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f5372-172">Accept</span><span class="sxs-lookup"><span data-stu-id="f5372-172">Accept</span></span> | <span data-ttu-id="f5372-173">application/json</span><span class="sxs-lookup"><span data-stu-id="f5372-173">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="f5372-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5372-174">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a><span data-ttu-id="f5372-175">Пример</span><span class="sxs-lookup"><span data-stu-id="f5372-175">Example</span></span>

<span data-ttu-id="f5372-176">В этом примере вам потребуется ID устройства и ID команды, которая была выдана устройству.</span><span class="sxs-lookup"><span data-stu-id="f5372-176">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f5372-177">При выдаче вызова GET возвращается ID устройства, а при вызове POST возвращается командный `/me/devices` `/me/devices/{id}/command` ID.</span><span class="sxs-lookup"><span data-stu-id="f5372-177">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f5372-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5372-178">Request</span></span>

<span data-ttu-id="f5372-179">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5372-179">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f5372-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5372-180">Response</span></span>

<span data-ttu-id="f5372-181">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5372-181">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```


