---
title: Получение состояния команд для устройства
description: Получение состояния команды на устройстве. Полный список кодов состояния представлен в разделе List of Актионстатус.
localization_priority: Normal
ms.openlocfilehash: 9b914cdfde78ce50df812acb09dc034c978c7e08
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324999"
---
# <a name="get-device-command-status"></a><span data-ttu-id="e49f6-104">Получение состояния команд для устройства</span><span class="sxs-lookup"><span data-stu-id="e49f6-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49f6-105">Получение состояния команды на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e49f6-105">Get the status of a command on a device.</span></span> <span data-ttu-id="e49f6-106">Полный список кодов состояния представлен в разделе [List of актионстатус](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="e49f6-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="e49f6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e49f6-107">Permissions</span></span>

<span data-ttu-id="e49f6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e49f6-110">Permission type</span></span>      | <span data-ttu-id="e49f6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e49f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e49f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e49f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e49f6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f6-113">Not supported.</span></span>    |
|<span data-ttu-id="e49f6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e49f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e49f6-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="e49f6-115">Device.Command</span></span>    |
|<span data-ttu-id="e49f6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e49f6-116">Application</span></span> | <span data-ttu-id="e49f6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e49f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e49f6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e49f6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e49f6-119">Request headers</span></span>

| <span data-ttu-id="e49f6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e49f6-120">Header</span></span> |<span data-ttu-id="e49f6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e49f6-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="e49f6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e49f6-122">Authorization</span></span>| <span data-ttu-id="e49f6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e49f6-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e49f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e49f6-125">Accept</span></span> | <span data-ttu-id="e49f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e49f6-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="e49f6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f6-127">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="e49f6-128">Список Актионстатус</span><span class="sxs-lookup"><span data-stu-id="e49f6-128">List of actionStatus</span></span>

- <span data-ttu-id="e49f6-129">была создана команда запроса//, ожидающая обработки</span><span class="sxs-lookup"><span data-stu-id="e49f6-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="e49f6-130">Сенттотаржет,///команда отправлена на целевое устройство</span><span class="sxs-lookup"><span data-stu-id="e49f6-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="e49f6-131">выполнение,//целевое устройство подтвердилое получение команды и выполняет ее.</span><span class="sxs-lookup"><span data-stu-id="e49f6-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="e49f6-132">завершено,//выполнение команды завершено</span><span class="sxs-lookup"><span data-stu-id="e49f6-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="e49f6-133">Фаиледтосенд,//служба не смогла отправить команду целевому устройству</span><span class="sxs-lookup"><span data-stu-id="e49f6-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="e49f6-134">Сбой при выполнении команды Ексекутионфаилед или//.</span><span class="sxs-lookup"><span data-stu-id="e49f6-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="e49f6-135">Команда Комманддроппед и//отброшена клиентом, если устройство находится в состоянии Коннектедстандби</span><span class="sxs-lookup"><span data-stu-id="e49f6-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="e49f6-136">Отмена,//отмена команды</span><span class="sxs-lookup"><span data-stu-id="e49f6-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="e49f6-137">Отмена и Отмена команды</span><span class="sxs-lookup"><span data-stu-id="e49f6-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="e49f6-138">отменено,//команда отменена</span><span class="sxs-lookup"><span data-stu-id="e49f6-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="e49f6-139">Retry,//служба повторяет попытку отправить целевую команду</span><span class="sxs-lookup"><span data-stu-id="e49f6-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="e49f6-140">просрочено,//превышена Дата истечения срока действия обработки команд</span><span class="sxs-lookup"><span data-stu-id="e49f6-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="e49f6-141">ошибка,//внутренняя ошибка при обработке команды</span><span class="sxs-lookup"><span data-stu-id="e49f6-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="e49f6-142">настраиваемый//настраиваемый статус</span><span class="sxs-lookup"><span data-stu-id="e49f6-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="e49f6-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e49f6-143">Example</span></span>

<span data-ttu-id="e49f6-144">В этом примере вам потребуется идентификатор устройства и идентификатор команды, выданной устройству.</span><span class="sxs-lookup"><span data-stu-id="e49f6-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="e49f6-145">ИДЕНТИФИКАТОР устройства возвращается при выдаче вызова GET `/me/devices`, а идентификатор команды возвращается при выполнении вызова POST. `/me/devices/{id}/command`</span><span class="sxs-lookup"><span data-stu-id="e49f6-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="e49f6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e49f6-146">Request</span></span>

<span data-ttu-id="e49f6-147">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e49f6-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="e49f6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f6-148">Response</span></span>

<span data-ttu-id="e49f6-149">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e49f6-149">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="e49f6-150">Получение полезных данных команды</span><span class="sxs-lookup"><span data-stu-id="e49f6-150">Get command payload</span></span>

<span data-ttu-id="e49f6-151">Получение полезных данных ответа для определенного действия на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e49f6-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="e49f6-152">Полезные данные ответа используются при запросе службы приложений для обратного переноса данных.</span><span class="sxs-lookup"><span data-stu-id="e49f6-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="e49f6-153">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e49f6-153">Permissions</span></span>

<span data-ttu-id="e49f6-p107">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49f6-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49f6-156">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e49f6-156">Permission type</span></span>      | <span data-ttu-id="e49f6-157">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e49f6-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e49f6-158">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e49f6-158">Delegated (work or school account)</span></span> | <span data-ttu-id="e49f6-159">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f6-159">Not supported.</span></span>    |
|<span data-ttu-id="e49f6-160">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e49f6-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e49f6-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="e49f6-161">Device.Command</span></span>    |
|<span data-ttu-id="e49f6-162">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e49f6-162">Application</span></span> | <span data-ttu-id="e49f6-163">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e49f6-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="e49f6-164">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e49f6-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="e49f6-165">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e49f6-165">Request headers</span></span>

| <span data-ttu-id="e49f6-166">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e49f6-166">Header</span></span> |<span data-ttu-id="e49f6-167">Значение</span><span class="sxs-lookup"><span data-stu-id="e49f6-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="e49f6-168">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e49f6-168">Authorization</span></span>| <span data-ttu-id="e49f6-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e49f6-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="e49f6-171">Accept</span><span class="sxs-lookup"><span data-stu-id="e49f6-171">Accept</span></span> | <span data-ttu-id="e49f6-172">application/json</span><span class="sxs-lookup"><span data-stu-id="e49f6-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="e49f6-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f6-173">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="e49f6-174">Пример</span><span class="sxs-lookup"><span data-stu-id="e49f6-174">Example</span></span>

<span data-ttu-id="e49f6-175">В этом примере вам потребуется идентификатор устройства и идентификатор команды, выданной устройству.</span><span class="sxs-lookup"><span data-stu-id="e49f6-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="e49f6-176">ИДЕНТИФИКАТОР устройства возвращается при выдаче вызова GET `/me/devices`, а идентификатор команды возвращается при выполнении вызова POST. `/me/devices/{id}/command`</span><span class="sxs-lookup"><span data-stu-id="e49f6-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="e49f6-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="e49f6-177">Request</span></span>

<span data-ttu-id="e49f6-178">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e49f6-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="e49f6-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="e49f6-179">Response</span></span>

<span data-ttu-id="e49f6-180">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e49f6-180">The following example shows the response.</span></span>

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
