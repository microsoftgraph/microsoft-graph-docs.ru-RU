---
title: Отправка команды устройства
description: 'Этот интерфейс API обеспечивает возможности рим проекта для передачи команд устройство, связанное с учетной записью Майкрософт. После выполнения на вызов GET `me/devices`, передайте идентификатор устройства, чтобы выполнить команду на устройство. Поддерживаются два типа из команд: LaunchURI и AppServices. Если вы используете LaunchURI, указания параметров *типа* и *полезных данных* . Для вызова AppService, укажите '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526244"
---
# <a name="send-device-command"></a><span data-ttu-id="604c7-107">Отправка команды устройства</span><span class="sxs-lookup"><span data-stu-id="604c7-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="604c7-108">Этот интерфейс API обеспечивает возможности рим проекта для передачи команд устройство, связанное с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="604c7-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="604c7-109">После выполнения на вызов GET `me/devices`, передайте идентификатор устройства, чтобы выполнить команду на устройство.</span><span class="sxs-lookup"><span data-stu-id="604c7-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="604c7-110">Поддерживаются два типа из команд: LaunchURI и AppServices.</span><span class="sxs-lookup"><span data-stu-id="604c7-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="604c7-111">Если вы используете LaunchURI, указания параметров *типа* и *полезных данных* .</span><span class="sxs-lookup"><span data-stu-id="604c7-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="604c7-112">Для вызова AppService укажите *Тип*, *полезных данных*, *packageFamilyName*и *appServiceName* параметры.</span><span class="sxs-lookup"><span data-stu-id="604c7-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="604c7-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="604c7-113">Permissions</span></span>

<span data-ttu-id="604c7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="604c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="604c7-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="604c7-116">Permission type</span></span>      | <span data-ttu-id="604c7-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="604c7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="604c7-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="604c7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="604c7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="604c7-119">Not supported.</span></span>    |
|<span data-ttu-id="604c7-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="604c7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="604c7-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="604c7-121">Device.Command</span></span>    |
|<span data-ttu-id="604c7-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="604c7-122">Application</span></span> | <span data-ttu-id="604c7-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="604c7-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="604c7-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="604c7-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="604c7-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="604c7-125">Request headers</span></span>


| <span data-ttu-id="604c7-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="604c7-126">Header</span></span> |<span data-ttu-id="604c7-127">Значение</span><span class="sxs-lookup"><span data-stu-id="604c7-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="604c7-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="604c7-128">Authorization</span></span>| <span data-ttu-id="604c7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="604c7-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="604c7-131">Accept</span><span class="sxs-lookup"><span data-stu-id="604c7-131">Accept</span></span> | <span data-ttu-id="604c7-132">application/json</span><span class="sxs-lookup"><span data-stu-id="604c7-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="604c7-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="604c7-133">Request body</span></span>

<span data-ttu-id="604c7-134">В тексте запроса укажите представление JSON свойства команды.</span><span class="sxs-lookup"><span data-stu-id="604c7-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="604c7-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="604c7-135">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="604c7-136">Свойства команды</span><span class="sxs-lookup"><span data-stu-id="604c7-136">Command properties</span></span> 

|<span data-ttu-id="604c7-137">**Name**</span><span class="sxs-lookup"><span data-stu-id="604c7-137">**Name**</span></span>|<span data-ttu-id="604c7-138">**Тип**</span><span class="sxs-lookup"><span data-stu-id="604c7-138">**Type**</span></span>|<span data-ttu-id="604c7-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="604c7-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="604c7-140">payload</span><span class="sxs-lookup"><span data-stu-id="604c7-140">payload</span></span> | <span data-ttu-id="604c7-141">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="604c7-141">microsoft.graph.json</span></span>| <span data-ttu-id="604c7-142">Полезные данные для отправки приложения-службы или для запуска URI на устройстве.</span><span class="sxs-lookup"><span data-stu-id="604c7-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="604c7-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="604c7-143">responsePayload</span></span> | <span data-ttu-id="604c7-144">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="604c7-144">microsoft.graph.json</span></span>| <span data-ttu-id="604c7-145">Полезные данные, возвращаемые целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="604c7-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="604c7-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="604c7-146">postBackURI</span></span> | <span data-ttu-id="604c7-147">String</span><span class="sxs-lookup"><span data-stu-id="604c7-147">String</span></span> | <span data-ttu-id="604c7-148">Публикация резервного URI для отправки последующих уведомлений об обновлениях.</span><span class="sxs-lookup"><span data-stu-id="604c7-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="604c7-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="604c7-149">packageFamilyName</span></span> | <span data-ttu-id="604c7-150">String</span><span class="sxs-lookup"><span data-stu-id="604c7-150">String</span></span> | <span data-ttu-id="604c7-151">Имя семейства Windows пакет приложения.</span><span class="sxs-lookup"><span data-stu-id="604c7-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="604c7-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="604c7-152">appServiceName</span></span> | <span data-ttu-id="604c7-153">String</span><span class="sxs-lookup"><span data-stu-id="604c7-153">String</span></span> | <span data-ttu-id="604c7-154">Имя приложения-службы, определенные в конечное приложение.</span><span class="sxs-lookup"><span data-stu-id="604c7-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="604c7-155">Требуется при запуске приложения-службы.</span><span class="sxs-lookup"><span data-stu-id="604c7-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="604c7-156">type</span><span class="sxs-lookup"><span data-stu-id="604c7-156">type</span></span>| <span data-ttu-id="604c7-157">String</span><span class="sxs-lookup"><span data-stu-id="604c7-157">String</span></span> | <span data-ttu-id="604c7-158">LaunchURI или AppService.</span><span class="sxs-lookup"><span data-stu-id="604c7-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="604c7-159">id</span><span class="sxs-lookup"><span data-stu-id="604c7-159">id</span></span>| <span data-ttu-id="604c7-160">String</span><span class="sxs-lookup"><span data-stu-id="604c7-160">String</span></span> | <span data-ttu-id="604c7-161">Идентификатор команды, полученного на устройство.</span><span class="sxs-lookup"><span data-stu-id="604c7-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="604c7-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="604c7-162">actionStatus</span></span> | <span data-ttu-id="604c7-163">String</span><span class="sxs-lookup"><span data-stu-id="604c7-163">String</span></span> | <span data-ttu-id="604c7-164">[Состояние](get-device-command-status.md) команды.</span><span class="sxs-lookup"><span data-stu-id="604c7-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="604c7-165">error</span><span class="sxs-lookup"><span data-stu-id="604c7-165">error</span></span>| <span data-ttu-id="604c7-166">String</span><span class="sxs-lookup"><span data-stu-id="604c7-166">String</span></span>| <span data-ttu-id="604c7-167">Все ошибки, связанные с запросом от целевого приложения.</span><span class="sxs-lookup"><span data-stu-id="604c7-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="604c7-168">Запуск примера URI</span><span class="sxs-lookup"><span data-stu-id="604c7-168">Launch URI example</span></span>

<span data-ttu-id="604c7-169">Ниже приведен пример запроса LaunchURI; он запустится URI или на устройстве конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="604c7-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="604c7-170">Для запуска приложения или URI, заключать POST, используя идентификатор устройства (полученных при выполнении вызова GET для `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="604c7-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="604c7-171">Параметры *типа* для *LaunchURI* , поэтому указывать значение URI, таких как https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="604c7-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="604c7-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="604c7-172">Request</span></span>

<span data-ttu-id="604c7-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="604c7-173">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="604c7-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="604c7-174">Response</span></span> 

<span data-ttu-id="604c7-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="604c7-175">The following is an example of the response.</span></span>

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


## <a name="app-service-example"></a><span data-ttu-id="604c7-176">Пример приложения-службы</span><span class="sxs-lookup"><span data-stu-id="604c7-176">App service example</span></span>

<span data-ttu-id="604c7-177">Ниже приведен пример запросов службу приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="604c7-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="604c7-178">Использование приложения-службы необходимо выполнить вызов POST, с помощью идентификатор устройства (полученных при выполнении вызова GET для `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="604c7-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="604c7-179">Для использования в следующем примере, необходимо установить [приложение рим](https://aka.ms/romanapp) целевое устройство.</span><span class="sxs-lookup"><span data-stu-id="604c7-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="604c7-180">Несколько дополнительных свойств необходимо установить в вызове.</span><span class="sxs-lookup"><span data-stu-id="604c7-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="604c7-181">*Тип* должен иметь значение *AppService*, *AppServiceName* должно быть присвоено имя службы приложения, определенные в приложении, *PackageFamilyName* должно быть присвоено имя пакета семейства, определенные в манифесте приложения и *полезных данных* содержит ключи и значения для службы вызова в конечном приложении.</span><span class="sxs-lookup"><span data-stu-id="604c7-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="604c7-182">Запросить</span><span class="sxs-lookup"><span data-stu-id="604c7-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="604c7-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="604c7-183">Response</span></span>

<span data-ttu-id="604c7-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="604c7-184">The following is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
