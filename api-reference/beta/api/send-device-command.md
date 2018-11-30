---
title: Отправка команды устройства
description: 'Этот интерфейс API обеспечивает возможности рим проекта для передачи команд устройство, связанное с учетной записью Майкрософт. После выполнения на вызов GET `me/devices`, передайте идентификатор устройства, чтобы выполнить команду на устройство. Поддерживаются два типа из команд: LaunchURI и AppServices. Если вы используете LaunchURI, указания параметров *типа* и *полезных данных* . Для вызова AppService, укажите '
ms.openlocfilehash: bf330ab1234ef6ce22c6a43711621827b628a7ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078753"
---
# <a name="send-device-command"></a><span data-ttu-id="3db59-107">Отправка команды устройства</span><span class="sxs-lookup"><span data-stu-id="3db59-107">Send device command</span></span>

> <span data-ttu-id="3db59-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3db59-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3db59-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3db59-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3db59-110">Этот интерфейс API обеспечивает возможности рим проекта для передачи команд устройство, связанное с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3db59-110">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="3db59-111">После выполнения на вызов GET `me/devices`, передайте идентификатор устройства, чтобы выполнить команду на устройство.</span><span class="sxs-lookup"><span data-stu-id="3db59-111">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="3db59-112">Поддерживаются два типа из команд: LaunchURI и AppServices.</span><span class="sxs-lookup"><span data-stu-id="3db59-112">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="3db59-113">Если вы используете LaunchURI, указания параметров *типа* и *полезных данных* .</span><span class="sxs-lookup"><span data-stu-id="3db59-113">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="3db59-114">Для вызова AppService укажите *Тип*, *полезных данных*, *packageFamilyName*и *appServiceName* параметры.</span><span class="sxs-lookup"><span data-stu-id="3db59-114">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="3db59-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3db59-115">Permissions</span></span>

<span data-ttu-id="3db59-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3db59-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3db59-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3db59-118">Permission type</span></span>      | <span data-ttu-id="3db59-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3db59-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3db59-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3db59-120">Delegated (work or school account)</span></span> | <span data-ttu-id="3db59-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3db59-121">Not supported.</span></span>    |
|<span data-ttu-id="3db59-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3db59-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db59-123">Device.Command</span><span class="sxs-lookup"><span data-stu-id="3db59-123">Device.Command</span></span>    |
|<span data-ttu-id="3db59-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3db59-124">Application</span></span> | <span data-ttu-id="3db59-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3db59-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3db59-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3db59-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="3db59-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3db59-127">Request headers</span></span>


| <span data-ttu-id="3db59-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3db59-128">Header</span></span> |<span data-ttu-id="3db59-129">Значение</span><span class="sxs-lookup"><span data-stu-id="3db59-129">Value</span></span>
|:----|:------|
|<span data-ttu-id="3db59-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3db59-130">Authorization</span></span>| <span data-ttu-id="3db59-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3db59-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="3db59-133">Accept</span><span class="sxs-lookup"><span data-stu-id="3db59-133">Accept</span></span> | <span data-ttu-id="3db59-134">application/json</span><span class="sxs-lookup"><span data-stu-id="3db59-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3db59-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3db59-135">Request body</span></span>

<span data-ttu-id="3db59-136">В тексте запроса укажите представление JSON свойства команды.</span><span class="sxs-lookup"><span data-stu-id="3db59-136">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="3db59-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="3db59-137">Response</span></span>

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
## <a name="command-properties"></a><span data-ttu-id="3db59-138">Свойства команды</span><span class="sxs-lookup"><span data-stu-id="3db59-138">Command properties</span></span> 

|<span data-ttu-id="3db59-139">**Name**</span><span class="sxs-lookup"><span data-stu-id="3db59-139">**Name**</span></span>|<span data-ttu-id="3db59-140">**Тип**</span><span class="sxs-lookup"><span data-stu-id="3db59-140">**Type**</span></span>|<span data-ttu-id="3db59-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3db59-141">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="3db59-142">payload</span><span class="sxs-lookup"><span data-stu-id="3db59-142">payload</span></span> | <span data-ttu-id="3db59-143">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="3db59-143">microsoft.graph.json</span></span>| <span data-ttu-id="3db59-144">Полезные данные для отправки приложения-службы или для запуска URI на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3db59-144">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="3db59-145">responsePayload</span><span class="sxs-lookup"><span data-stu-id="3db59-145">responsePayload</span></span> | <span data-ttu-id="3db59-146">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="3db59-146">microsoft.graph.json</span></span>| <span data-ttu-id="3db59-147">Полезные данные, возвращаемые целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="3db59-147">Payload returned from target device.</span></span> |
|<span data-ttu-id="3db59-148">postBackURI</span><span class="sxs-lookup"><span data-stu-id="3db59-148">postBackURI</span></span> | <span data-ttu-id="3db59-149">String</span><span class="sxs-lookup"><span data-stu-id="3db59-149">String</span></span> | <span data-ttu-id="3db59-150">Публикация резервного URI для отправки последующих уведомлений об обновлениях.</span><span class="sxs-lookup"><span data-stu-id="3db59-150">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="3db59-151">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="3db59-151">packageFamilyName</span></span> | <span data-ttu-id="3db59-152">String</span><span class="sxs-lookup"><span data-stu-id="3db59-152">String</span></span> | <span data-ttu-id="3db59-153">Имя семейства Windows пакет приложения.</span><span class="sxs-lookup"><span data-stu-id="3db59-153">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="3db59-154">appServiceName</span><span class="sxs-lookup"><span data-stu-id="3db59-154">appServiceName</span></span> | <span data-ttu-id="3db59-155">String</span><span class="sxs-lookup"><span data-stu-id="3db59-155">String</span></span> | <span data-ttu-id="3db59-156">Имя приложения-службы, определенные в конечное приложение.</span><span class="sxs-lookup"><span data-stu-id="3db59-156">Name of app service defined by the target application.</span></span> <span data-ttu-id="3db59-157">Требуется при запуске приложения-службы.</span><span class="sxs-lookup"><span data-stu-id="3db59-157">Required if launching an app service.</span></span> |
|<span data-ttu-id="3db59-158">type</span><span class="sxs-lookup"><span data-stu-id="3db59-158">type</span></span>| <span data-ttu-id="3db59-159">String</span><span class="sxs-lookup"><span data-stu-id="3db59-159">String</span></span> | <span data-ttu-id="3db59-160">LaunchURI или AppService.</span><span class="sxs-lookup"><span data-stu-id="3db59-160">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="3db59-161">id</span><span class="sxs-lookup"><span data-stu-id="3db59-161">id</span></span>| <span data-ttu-id="3db59-162">String</span><span class="sxs-lookup"><span data-stu-id="3db59-162">String</span></span> | <span data-ttu-id="3db59-163">Идентификатор команды, полученного на устройство.</span><span class="sxs-lookup"><span data-stu-id="3db59-163">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="3db59-164">actionStatus</span><span class="sxs-lookup"><span data-stu-id="3db59-164">actionStatus</span></span> | <span data-ttu-id="3db59-165">String</span><span class="sxs-lookup"><span data-stu-id="3db59-165">String</span></span> | <span data-ttu-id="3db59-166">[Состояние](get-device-command-status.md) команды.</span><span class="sxs-lookup"><span data-stu-id="3db59-166">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="3db59-167">error</span><span class="sxs-lookup"><span data-stu-id="3db59-167">error</span></span>| <span data-ttu-id="3db59-168">String</span><span class="sxs-lookup"><span data-stu-id="3db59-168">String</span></span>| <span data-ttu-id="3db59-169">Все ошибки, связанные с запросом от целевого приложения.</span><span class="sxs-lookup"><span data-stu-id="3db59-169">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="3db59-170">Запуск примера URI</span><span class="sxs-lookup"><span data-stu-id="3db59-170">Launch URI example</span></span>

<span data-ttu-id="3db59-171">Ниже приведен пример запроса LaunchURI; он запустится URI или на устройстве конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="3db59-171">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="3db59-172">Для запуска приложения или URI, заключать POST, используя идентификатор устройства (полученных при выполнении вызова GET для `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="3db59-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="3db59-173">Параметры *типа* для *LaunchURI* , поэтому указывать значение URI, таких как https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="3db59-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="3db59-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="3db59-174">Request</span></span>

<span data-ttu-id="3db59-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3db59-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```

#### <a name="response"></a><span data-ttu-id="3db59-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="3db59-176">Response</span></span> 

<span data-ttu-id="3db59-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3db59-177">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


## <a name="app-service-example"></a><span data-ttu-id="3db59-178">Пример приложения-службы</span><span class="sxs-lookup"><span data-stu-id="3db59-178">App service example</span></span>

<span data-ttu-id="3db59-179">Ниже приведен пример запросов службу приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3db59-179">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="3db59-180">Использование приложения-службы необходимо выполнить вызов POST, с помощью идентификатор устройства (полученных при выполнении вызова GET для `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="3db59-180">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="3db59-181">Для использования в следующем примере, необходимо установить [приложение рим](https://aka.ms/romanapp) целевое устройство.</span><span class="sxs-lookup"><span data-stu-id="3db59-181">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="3db59-182">Несколько дополнительных свойств необходимо установить в вызове.</span><span class="sxs-lookup"><span data-stu-id="3db59-182">Several additional properties must be set in the call.</span></span> <span data-ttu-id="3db59-183">*Тип* должен иметь значение *AppService*, *AppServiceName* должно быть присвоено имя службы приложения, определенные в приложении, *PackageFamilyName* должно быть присвоено имя пакета семейства, определенные в манифесте приложения и *полезных данных* содержит ключи и значения для службы вызова в конечном приложении.</span><span class="sxs-lookup"><span data-stu-id="3db59-183">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="3db59-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="3db59-184">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a><span data-ttu-id="3db59-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="3db59-185">Response</span></span>

<span data-ttu-id="3db59-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3db59-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
