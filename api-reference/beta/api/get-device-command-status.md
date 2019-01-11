---
title: Получение состояния команды устройства
description: Получение состояния команды на устройстве. Полный список кодов состояния списка actionStatus см.
localization_priority: Normal
ms.openlocfilehash: 9dca743a50f248abee76fb4d54352df3d400ada1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883134"
---
# <a name="get-device-command-status"></a><span data-ttu-id="a90a4-104">Получение состояния команды устройства</span><span class="sxs-lookup"><span data-stu-id="a90a4-104">Get device command status</span></span>

> <span data-ttu-id="a90a4-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a90a4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a90a4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90a4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a90a4-107">Получение состояния команды на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a90a4-107">Get the status of a command on a device.</span></span> <span data-ttu-id="a90a4-108">Полный список кодов состояния [списка actionStatus](#list-of-actionstatus)см.</span><span class="sxs-lookup"><span data-stu-id="a90a4-108">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="a90a4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a90a4-109">Permissions</span></span>

<span data-ttu-id="a90a4-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a90a4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a90a4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a90a4-112">Permission type</span></span>      | <span data-ttu-id="a90a4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a90a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a90a4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a90a4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a90a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90a4-115">Not supported.</span></span>    |
|<span data-ttu-id="a90a4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a90a4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a90a4-117">Device.Command</span><span class="sxs-lookup"><span data-stu-id="a90a4-117">Device.Command</span></span>    |
|<span data-ttu-id="a90a4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a90a4-118">Application</span></span> | <span data-ttu-id="a90a4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90a4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a90a4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a90a4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a90a4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a90a4-121">Request headers</span></span>

| <span data-ttu-id="a90a4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a90a4-122">Header</span></span> |<span data-ttu-id="a90a4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a90a4-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="a90a4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a90a4-124">Authorization</span></span>| <span data-ttu-id="a90a4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a90a4-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a90a4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a90a4-127">Accept</span></span> | <span data-ttu-id="a90a4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a90a4-128">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="a90a4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a90a4-129">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="a90a4-130">Список actionStatus</span><span class="sxs-lookup"><span data-stu-id="a90a4-130">List of actionStatus</span></span>

- <span data-ttu-id="a90a4-131">разрешения на запрос, / / команда будет создан и ожидает обработки</span><span class="sxs-lookup"><span data-stu-id="a90a4-131">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="a90a4-132">sentToTarget, / / отправить команду целевого устройства</span><span class="sxs-lookup"><span data-stu-id="a90a4-132">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="a90a4-133">выполнение, / / устройство подтверждено поступления команды и он выполняется</span><span class="sxs-lookup"><span data-stu-id="a90a4-133">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="a90a4-134">завершена, и аудио- и завершения выполнения команд</span><span class="sxs-lookup"><span data-stu-id="a90a4-134">completed, // Command execution completed</span></span>
- <span data-ttu-id="a90a4-135">failedToSend, / / службе не удалось передать команду устройство</span><span class="sxs-lookup"><span data-stu-id="a90a4-135">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="a90a4-136">executionFailed, / / команда не выполнена.</span><span class="sxs-lookup"><span data-stu-id="a90a4-136">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="a90a4-137">commandDropped, / / команда Удалить клиентом, если устройство находится в состоянии ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="a90a4-137">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="a90a4-138">отменить, / / отмена команды</span><span class="sxs-lookup"><span data-stu-id="a90a4-138">cancel, // Cancel the command</span></span>
- <span data-ttu-id="a90a4-139">Отмена, / / отмены команды</span><span class="sxs-lookup"><span data-stu-id="a90a4-139">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="a90a4-140">отменено, / / команда была отменена</span><span class="sxs-lookup"><span data-stu-id="a90a4-140">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="a90a4-141">повторить попытку, / / службы восстанавливается для отправки команд к целевому</span><span class="sxs-lookup"><span data-stu-id="a90a4-141">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="a90a4-142">истек срок действия, / / команды обработки превышено время истечения срока действия</span><span class="sxs-lookup"><span data-stu-id="a90a4-142">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="a90a4-143">Ошибка, / аудио- и внутренняя ошибка при обработке команды</span><span class="sxs-lookup"><span data-stu-id="a90a4-143">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="a90a4-144">настраиваемые / аудио- и настраиваемые состояния</span><span class="sxs-lookup"><span data-stu-id="a90a4-144">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="a90a4-145">Пример</span><span class="sxs-lookup"><span data-stu-id="a90a4-145">Example</span></span>

<span data-ttu-id="a90a4-146">В этом примере необходимо будет идентификатор устройства и идентификатор команды, которая выполнялась для устройства.</span><span class="sxs-lookup"><span data-stu-id="a90a4-146">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="a90a4-147">При выдаче GET возвращается идентификатор устройства звонок, чтобы `/me/devices`, и команды, при выполнении отправки возвращается идентификатор звонок на `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="a90a4-147">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="a90a4-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a90a4-148">Request</span></span>

<span data-ttu-id="a90a4-149">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a90a4-149">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="a90a4-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="a90a4-150">Response</span></span>

<span data-ttu-id="a90a4-151">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a90a4-151">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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


## <a name="get-command-payload"></a><span data-ttu-id="a90a4-152">Получение полезных данных команды</span><span class="sxs-lookup"><span data-stu-id="a90a4-152">Get command payload</span></span>

<span data-ttu-id="a90a4-153">Получение ответа полезных для определенных действий на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a90a4-153">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="a90a4-154">Полезные данные ответа используется при запросе приложения-службы для выполнения данных обратно.</span><span class="sxs-lookup"><span data-stu-id="a90a4-154">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="a90a4-155">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a90a4-155">Permissions</span></span>

<span data-ttu-id="a90a4-p108">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a90a4-p108">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a90a4-158">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a90a4-158">Permission type</span></span>      | <span data-ttu-id="a90a4-159">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a90a4-159">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a90a4-160">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a90a4-160">Delegated (work or school account)</span></span> | <span data-ttu-id="a90a4-161">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90a4-161">Not supported.</span></span>    |
|<span data-ttu-id="a90a4-162">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a90a4-162">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a90a4-163">Device.Command</span><span class="sxs-lookup"><span data-stu-id="a90a4-163">Device.Command</span></span>    |
|<span data-ttu-id="a90a4-164">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a90a4-164">Application</span></span> | <span data-ttu-id="a90a4-165">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90a4-165">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="a90a4-166">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a90a4-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="a90a4-167">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a90a4-167">Request headers</span></span>

| <span data-ttu-id="a90a4-168">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a90a4-168">Header</span></span> |<span data-ttu-id="a90a4-169">Значение</span><span class="sxs-lookup"><span data-stu-id="a90a4-169">Value</span></span>
|:----|:------|
|<span data-ttu-id="a90a4-170">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a90a4-170">Authorization</span></span>| <span data-ttu-id="a90a4-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a90a4-p109">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="a90a4-173">Accept</span><span class="sxs-lookup"><span data-stu-id="a90a4-173">Accept</span></span> | <span data-ttu-id="a90a4-174">application/json</span><span class="sxs-lookup"><span data-stu-id="a90a4-174">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="a90a4-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="a90a4-175">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="a90a4-176">Пример</span><span class="sxs-lookup"><span data-stu-id="a90a4-176">Example</span></span>

<span data-ttu-id="a90a4-177">В этом примере необходимо будет идентификатор устройства и идентификатор команды, которая выполнялась для устройства.</span><span class="sxs-lookup"><span data-stu-id="a90a4-177">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="a90a4-178">Устройство, возвращается идентификатор при выдаче получить вызов на `/me/devices`, и команды, при выполнении отправки возвращается идентификатор звонок на `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="a90a4-178">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="a90a4-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="a90a4-179">Request</span></span>

<span data-ttu-id="a90a4-180">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a90a4-180">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="a90a4-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="a90a4-181">Response</span></span>

<span data-ttu-id="a90a4-182">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a90a4-182">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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
