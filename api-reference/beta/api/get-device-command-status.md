---
title: Получение состояния команд для устройства
description: Получение состояния команды на устройстве. Полный список кодов состояния представлен в разделе List of Актионстатус.
localization_priority: Normal
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: 33470cb5aceb402d6a37749fa8c2ebcfcd0bce75
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807334"
---
# <a name="get-device-command-status"></a><span data-ttu-id="fa278-104">Получение состояния команд для устройства</span><span class="sxs-lookup"><span data-stu-id="fa278-104">Get device command status</span></span>

<span data-ttu-id="fa278-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa278-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa278-106">Получение состояния команды на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fa278-106">Get the status of a command on a device.</span></span> <span data-ttu-id="fa278-107">Полный список кодов состояния представлен в разделе [List of актионстатус](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="fa278-107">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa278-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa278-108">Permissions</span></span>

<span data-ttu-id="fa278-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa278-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa278-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa278-111">Permission type</span></span>      | <span data-ttu-id="fa278-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa278-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa278-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa278-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fa278-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa278-114">Not supported.</span></span>    |
|<span data-ttu-id="fa278-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa278-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa278-116">Device.Command</span><span class="sxs-lookup"><span data-stu-id="fa278-116">Device.Command</span></span>    |
|<span data-ttu-id="fa278-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa278-117">Application</span></span> | <span data-ttu-id="fa278-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa278-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa278-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa278-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa278-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa278-120">Request headers</span></span>

| <span data-ttu-id="fa278-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa278-121">Header</span></span> |<span data-ttu-id="fa278-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa278-122">Value</span></span>
|:----|:------|
|<span data-ttu-id="fa278-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa278-123">Authorization</span></span>| <span data-ttu-id="fa278-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa278-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="fa278-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fa278-126">Accept</span></span> | <span data-ttu-id="fa278-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fa278-127">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="fa278-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa278-128">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="fa278-129">Список Актионстатус</span><span class="sxs-lookup"><span data-stu-id="fa278-129">List of actionStatus</span></span>

- <span data-ttu-id="fa278-130">была создана команда запроса//, ожидающая обработки</span><span class="sxs-lookup"><span data-stu-id="fa278-130">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="fa278-131">Сенттотаржет,///команда отправлена на целевое устройство</span><span class="sxs-lookup"><span data-stu-id="fa278-131">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="fa278-132">выполнение,//целевое устройство подтвердилое получение команды и выполняет ее.</span><span class="sxs-lookup"><span data-stu-id="fa278-132">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="fa278-133">завершено,//выполнение команды завершено</span><span class="sxs-lookup"><span data-stu-id="fa278-133">completed, // Command execution completed</span></span>
- <span data-ttu-id="fa278-134">Фаиледтосенд,//служба не смогла отправить команду целевому устройству</span><span class="sxs-lookup"><span data-stu-id="fa278-134">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="fa278-135">Сбой при выполнении команды Ексекутионфаилед или//.</span><span class="sxs-lookup"><span data-stu-id="fa278-135">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="fa278-136">Команда Комманддроппед и//отброшена клиентом, если устройство находится в состоянии Коннектедстандби</span><span class="sxs-lookup"><span data-stu-id="fa278-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="fa278-137">Отмена,//отмена команды</span><span class="sxs-lookup"><span data-stu-id="fa278-137">cancel, // Cancel the command</span></span>
- <span data-ttu-id="fa278-138">Отмена и Отмена команды</span><span class="sxs-lookup"><span data-stu-id="fa278-138">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="fa278-139">отменено,//команда отменена</span><span class="sxs-lookup"><span data-stu-id="fa278-139">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="fa278-140">Retry,//служба повторяет попытку отправить целевую команду</span><span class="sxs-lookup"><span data-stu-id="fa278-140">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="fa278-141">просрочено,//превышена Дата истечения срока действия обработки команд</span><span class="sxs-lookup"><span data-stu-id="fa278-141">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="fa278-142">ошибка,//внутренняя ошибка при обработке команды</span><span class="sxs-lookup"><span data-stu-id="fa278-142">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="fa278-143">настраиваемый//настраиваемый статус</span><span class="sxs-lookup"><span data-stu-id="fa278-143">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="fa278-144">Пример</span><span class="sxs-lookup"><span data-stu-id="fa278-144">Example</span></span>

<span data-ttu-id="fa278-145">В этом примере вам потребуется идентификатор устройства и идентификатор команды, выданной устройству.</span><span class="sxs-lookup"><span data-stu-id="fa278-145">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="fa278-146">ИДЕНТИФИКАТОР устройства возвращается при выдаче вызова GET `/me/devices` , а идентификатор команды возвращается при выполнении вызова Post `/me/devices/{id}/command` .</span><span class="sxs-lookup"><span data-stu-id="fa278-146">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="fa278-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa278-147">Request</span></span>

<span data-ttu-id="fa278-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa278-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="fa278-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa278-149">Response</span></span>

<span data-ttu-id="fa278-150">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa278-150">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="fa278-151">Получение полезных данных команды</span><span class="sxs-lookup"><span data-stu-id="fa278-151">Get command payload</span></span>

<span data-ttu-id="fa278-152">Получение полезных данных ответа для определенного действия на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fa278-152">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="fa278-153">Полезные данные ответа используются при запросе службы приложений для обратного переноса данных.</span><span class="sxs-lookup"><span data-stu-id="fa278-153">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="fa278-154">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa278-154">Permissions</span></span>

<span data-ttu-id="fa278-p107">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa278-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa278-157">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa278-157">Permission type</span></span>      | <span data-ttu-id="fa278-158">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa278-158">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa278-159">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa278-159">Delegated (work or school account)</span></span> | <span data-ttu-id="fa278-160">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa278-160">Not supported.</span></span>    |
|<span data-ttu-id="fa278-161">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa278-161">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa278-162">Device.Command</span><span class="sxs-lookup"><span data-stu-id="fa278-162">Device.Command</span></span>    |
|<span data-ttu-id="fa278-163">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa278-163">Application</span></span> | <span data-ttu-id="fa278-164">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa278-164">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="fa278-165">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa278-165">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="fa278-166">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa278-166">Request headers</span></span>

| <span data-ttu-id="fa278-167">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa278-167">Header</span></span> |<span data-ttu-id="fa278-168">Значение</span><span class="sxs-lookup"><span data-stu-id="fa278-168">Value</span></span>
|:----|:------|
|<span data-ttu-id="fa278-169">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa278-169">Authorization</span></span>| <span data-ttu-id="fa278-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa278-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="fa278-172">Accept</span><span class="sxs-lookup"><span data-stu-id="fa278-172">Accept</span></span> | <span data-ttu-id="fa278-173">application/json</span><span class="sxs-lookup"><span data-stu-id="fa278-173">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="fa278-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa278-174">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="fa278-175">Пример</span><span class="sxs-lookup"><span data-stu-id="fa278-175">Example</span></span>

<span data-ttu-id="fa278-176">В этом примере вам потребуется идентификатор устройства и идентификатор команды, выданной устройству.</span><span class="sxs-lookup"><span data-stu-id="fa278-176">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="fa278-177">ИДЕНТИФИКАТОР устройства возвращается при выдаче вызова GET `/me/devices` , а идентификатор команды возвращается при выполнении вызова Post `/me/devices/{id}/command` .</span><span class="sxs-lookup"><span data-stu-id="fa278-177">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="fa278-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa278-178">Request</span></span>

<span data-ttu-id="fa278-179">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa278-179">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="fa278-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa278-180">Response</span></span>

<span data-ttu-id="fa278-181">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa278-181">The following example shows the response.</span></span>

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
