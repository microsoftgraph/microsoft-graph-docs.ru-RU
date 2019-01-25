---
title: Получение состояния команды устройства
description: Получение состояния команды на устройстве. Полный список кодов состояния списка actionStatus см.
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510115"
---
# <a name="get-device-command-status"></a><span data-ttu-id="14744-104">Получение состояния команды устройства</span><span class="sxs-lookup"><span data-stu-id="14744-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14744-105">Получение состояния команды на устройстве.</span><span class="sxs-lookup"><span data-stu-id="14744-105">Get the status of a command on a device.</span></span> <span data-ttu-id="14744-106">Полный список кодов состояния [списка actionStatus](#list-of-actionstatus)см.</span><span class="sxs-lookup"><span data-stu-id="14744-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="14744-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14744-107">Permissions</span></span>

<span data-ttu-id="14744-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14744-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14744-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14744-110">Permission type</span></span>      | <span data-ttu-id="14744-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14744-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14744-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14744-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14744-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14744-113">Not supported.</span></span>    |
|<span data-ttu-id="14744-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14744-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14744-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="14744-115">Device.Command</span></span>    |
|<span data-ttu-id="14744-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14744-116">Application</span></span> | <span data-ttu-id="14744-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14744-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14744-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14744-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="14744-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14744-119">Request headers</span></span>

| <span data-ttu-id="14744-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14744-120">Header</span></span> |<span data-ttu-id="14744-121">Значение</span><span class="sxs-lookup"><span data-stu-id="14744-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="14744-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14744-122">Authorization</span></span>| <span data-ttu-id="14744-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14744-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="14744-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14744-125">Accept</span></span> | <span data-ttu-id="14744-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14744-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="14744-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="14744-127">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="14744-128">Список actionStatus</span><span class="sxs-lookup"><span data-stu-id="14744-128">List of actionStatus</span></span>

- <span data-ttu-id="14744-129">разрешения на запрос, / / команда будет создан и ожидает обработки</span><span class="sxs-lookup"><span data-stu-id="14744-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="14744-130">sentToTarget, / / отправить команду целевого устройства</span><span class="sxs-lookup"><span data-stu-id="14744-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="14744-131">выполнение, / / устройство подтверждено поступления команды и он выполняется</span><span class="sxs-lookup"><span data-stu-id="14744-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="14744-132">завершена, и аудио- и завершения выполнения команд</span><span class="sxs-lookup"><span data-stu-id="14744-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="14744-133">failedToSend, / / службе не удалось передать команду устройство</span><span class="sxs-lookup"><span data-stu-id="14744-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="14744-134">executionFailed, / / команда не выполнена.</span><span class="sxs-lookup"><span data-stu-id="14744-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="14744-135">commandDropped, / / команда Удалить клиентом, если устройство находится в состоянии ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="14744-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="14744-136">отменить, / / отмена команды</span><span class="sxs-lookup"><span data-stu-id="14744-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="14744-137">Отмена, / / отмены команды</span><span class="sxs-lookup"><span data-stu-id="14744-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="14744-138">отменено, / / команда была отменена</span><span class="sxs-lookup"><span data-stu-id="14744-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="14744-139">повторить попытку, / / службы восстанавливается для отправки команд к целевому</span><span class="sxs-lookup"><span data-stu-id="14744-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="14744-140">истек срок действия, / / команды обработки превышено время истечения срока действия</span><span class="sxs-lookup"><span data-stu-id="14744-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="14744-141">Ошибка, / аудио- и внутренняя ошибка при обработке команды</span><span class="sxs-lookup"><span data-stu-id="14744-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="14744-142">настраиваемые / аудио- и настраиваемые состояния</span><span class="sxs-lookup"><span data-stu-id="14744-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="14744-143">Пример</span><span class="sxs-lookup"><span data-stu-id="14744-143">Example</span></span>

<span data-ttu-id="14744-144">В этом примере необходимо будет идентификатор устройства и идентификатор команды, которая выполнялась для устройства.</span><span class="sxs-lookup"><span data-stu-id="14744-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="14744-145">При выдаче GET возвращается идентификатор устройства звонок, чтобы `/me/devices`, и команды, при выполнении отправки возвращается идентификатор звонок на `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="14744-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="14744-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="14744-146">Request</span></span>

<span data-ttu-id="14744-147">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14744-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="14744-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="14744-148">Response</span></span>

<span data-ttu-id="14744-149">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14744-149">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="14744-150">Получение полезных данных команды</span><span class="sxs-lookup"><span data-stu-id="14744-150">Get command payload</span></span>

<span data-ttu-id="14744-151">Получение ответа полезных для определенных действий на устройстве.</span><span class="sxs-lookup"><span data-stu-id="14744-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="14744-152">Полезные данные ответа используется при запросе приложения-службы для выполнения данных обратно.</span><span class="sxs-lookup"><span data-stu-id="14744-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="14744-153">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14744-153">Permissions</span></span>

<span data-ttu-id="14744-p107">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14744-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14744-156">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14744-156">Permission type</span></span>      | <span data-ttu-id="14744-157">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14744-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14744-158">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14744-158">Delegated (work or school account)</span></span> | <span data-ttu-id="14744-159">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14744-159">Not supported.</span></span>    |
|<span data-ttu-id="14744-160">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14744-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14744-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="14744-161">Device.Command</span></span>    |
|<span data-ttu-id="14744-162">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14744-162">Application</span></span> | <span data-ttu-id="14744-163">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14744-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="14744-164">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14744-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="14744-165">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14744-165">Request headers</span></span>

| <span data-ttu-id="14744-166">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14744-166">Header</span></span> |<span data-ttu-id="14744-167">Значение</span><span class="sxs-lookup"><span data-stu-id="14744-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="14744-168">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14744-168">Authorization</span></span>| <span data-ttu-id="14744-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14744-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="14744-171">Accept</span><span class="sxs-lookup"><span data-stu-id="14744-171">Accept</span></span> | <span data-ttu-id="14744-172">application/json</span><span class="sxs-lookup"><span data-stu-id="14744-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="14744-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="14744-173">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="14744-174">Пример</span><span class="sxs-lookup"><span data-stu-id="14744-174">Example</span></span>

<span data-ttu-id="14744-175">В этом примере необходимо будет идентификатор устройства и идентификатор команды, которая выполнялась для устройства.</span><span class="sxs-lookup"><span data-stu-id="14744-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="14744-176">Устройство, возвращается идентификатор при выдаче получить вызов на `/me/devices`, и команды, при выполнении отправки возвращается идентификатор звонок на `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="14744-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="14744-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="14744-177">Request</span></span>

<span data-ttu-id="14744-178">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14744-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="14744-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="14744-179">Response</span></span>

<span data-ttu-id="14744-180">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14744-180">The following example shows the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
