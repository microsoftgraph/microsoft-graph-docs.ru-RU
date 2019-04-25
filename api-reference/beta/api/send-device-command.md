---
title: Отправка команд для устройства
description: 'Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт. После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство. Поддерживаются два типа команд: Лаунчури и Аппсервицес. Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* . Для вызова включающее укажите '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537536"
---
# <a name="send-device-command"></a><span data-ttu-id="0a252-107">Отправка команд для устройства</span><span class="sxs-lookup"><span data-stu-id="0a252-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a252-108">Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0a252-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="0a252-109">После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство.</span><span class="sxs-lookup"><span data-stu-id="0a252-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="0a252-110">Поддерживаются два типа команд: Лаунчури и Аппсервицес.</span><span class="sxs-lookup"><span data-stu-id="0a252-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="0a252-111">Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* .</span><span class="sxs-lookup"><span data-stu-id="0a252-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="0a252-112">Для вызова включающее укажите параметры *Type*, *полезная нагрузка*, *паккажефамилинаме*и *аппсервиценаме* .</span><span class="sxs-lookup"><span data-stu-id="0a252-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a252-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a252-113">Permissions</span></span>

<span data-ttu-id="0a252-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a252-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0a252-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a252-116">Permission type</span></span>      | <span data-ttu-id="0a252-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a252-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a252-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a252-118">Delegated (work or school account)</span></span> | <span data-ttu-id="0a252-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a252-119">Not supported.</span></span>    |
|<span data-ttu-id="0a252-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a252-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a252-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="0a252-121">Device.Command</span></span>    |
|<span data-ttu-id="0a252-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a252-122">Application</span></span> | <span data-ttu-id="0a252-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a252-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a252-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a252-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="0a252-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a252-125">Request headers</span></span>


| <span data-ttu-id="0a252-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a252-126">Header</span></span> |<span data-ttu-id="0a252-127">Значение</span><span class="sxs-lookup"><span data-stu-id="0a252-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="0a252-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a252-128">Authorization</span></span>| <span data-ttu-id="0a252-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a252-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="0a252-131">Accept</span><span class="sxs-lookup"><span data-stu-id="0a252-131">Accept</span></span> | <span data-ttu-id="0a252-132">application/json</span><span class="sxs-lookup"><span data-stu-id="0a252-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a252-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a252-133">Request body</span></span>

<span data-ttu-id="0a252-134">В тексте запроса добавьте представление свойств команды в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a252-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="0a252-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a252-135">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="0a252-136">Свойства команды</span><span class="sxs-lookup"><span data-stu-id="0a252-136">Command properties</span></span> 

|<span data-ttu-id="0a252-137">**Name**</span><span class="sxs-lookup"><span data-stu-id="0a252-137">**Name**</span></span>|<span data-ttu-id="0a252-138">**Type**</span><span class="sxs-lookup"><span data-stu-id="0a252-138">**Type**</span></span>|<span data-ttu-id="0a252-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0a252-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="0a252-140">payload</span><span class="sxs-lookup"><span data-stu-id="0a252-140">payload</span></span> | <span data-ttu-id="0a252-141">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="0a252-141">microsoft.graph.json</span></span>| <span data-ttu-id="0a252-142">Полезные данные для отправки в службу приложения или для запуска URI на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a252-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="0a252-143">Респонсепайлоад</span><span class="sxs-lookup"><span data-stu-id="0a252-143">responsePayload</span></span> | <span data-ttu-id="0a252-144">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="0a252-144">microsoft.graph.json</span></span>| <span data-ttu-id="0a252-145">Полезные данные, возвращенные с целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="0a252-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="0a252-146">Постбаккури</span><span class="sxs-lookup"><span data-stu-id="0a252-146">postBackURI</span></span> | <span data-ttu-id="0a252-147">String</span><span class="sxs-lookup"><span data-stu-id="0a252-147">String</span></span> | <span data-ttu-id="0a252-148">Обратный адрес URI для отправки последующих уведомлений об обновлениях.</span><span class="sxs-lookup"><span data-stu-id="0a252-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="0a252-149">Паккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="0a252-149">packageFamilyName</span></span> | <span data-ttu-id="0a252-150">String</span><span class="sxs-lookup"><span data-stu-id="0a252-150">String</span></span> | <span data-ttu-id="0a252-151">Имя семейства пакетов Windows Application.</span><span class="sxs-lookup"><span data-stu-id="0a252-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="0a252-152">Аппсервиценаме</span><span class="sxs-lookup"><span data-stu-id="0a252-152">appServiceName</span></span> | <span data-ttu-id="0a252-153">String</span><span class="sxs-lookup"><span data-stu-id="0a252-153">String</span></span> | <span data-ttu-id="0a252-154">Имя службы приложений, определенной конечным приложением.</span><span class="sxs-lookup"><span data-stu-id="0a252-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="0a252-155">Является обязательным при запуске службы приложений.</span><span class="sxs-lookup"><span data-stu-id="0a252-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="0a252-156">type</span><span class="sxs-lookup"><span data-stu-id="0a252-156">type</span></span>| <span data-ttu-id="0a252-157">String</span><span class="sxs-lookup"><span data-stu-id="0a252-157">String</span></span> | <span data-ttu-id="0a252-158">Лаунчури или включающее.</span><span class="sxs-lookup"><span data-stu-id="0a252-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="0a252-159">id</span><span class="sxs-lookup"><span data-stu-id="0a252-159">id</span></span>| <span data-ttu-id="0a252-160">String</span><span class="sxs-lookup"><span data-stu-id="0a252-160">String</span></span> | <span data-ttu-id="0a252-161">Идентификатор команды, отправленной на устройство.</span><span class="sxs-lookup"><span data-stu-id="0a252-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="0a252-162">Актионстатус</span><span class="sxs-lookup"><span data-stu-id="0a252-162">actionStatus</span></span> | <span data-ttu-id="0a252-163">String</span><span class="sxs-lookup"><span data-stu-id="0a252-163">String</span></span> | <span data-ttu-id="0a252-164">[Состояние](get-device-command-status.md) команды.</span><span class="sxs-lookup"><span data-stu-id="0a252-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="0a252-165">error</span><span class="sxs-lookup"><span data-stu-id="0a252-165">error</span></span>| <span data-ttu-id="0a252-166">String</span><span class="sxs-lookup"><span data-stu-id="0a252-166">String</span></span>| <span data-ttu-id="0a252-167">Все ошибки, связанные с запросом от конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="0a252-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="0a252-168">Пример кода URI запуска</span><span class="sxs-lookup"><span data-stu-id="0a252-168">Launch URI example</span></span>

<span data-ttu-id="0a252-169">Ниже приведен пример запроса Лаунчури. он запустит URI или приложение на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a252-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="0a252-170">Чтобы запустить URI или приложение, отправьте сообщение POST с использованием идентификатора устройства (получено при вызове GET `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="0a252-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="0a252-171">Задайте для параметров *Type* значение *лаунчури* и введите значение URI, например https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="0a252-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="0a252-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a252-172">Request</span></span>

<span data-ttu-id="0a252-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a252-173">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="0a252-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a252-174">Response</span></span> 

<span data-ttu-id="0a252-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a252-175">The following is an example of the response.</span></span>

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


## <a name="app-service-example"></a><span data-ttu-id="0a252-176">Пример службы приложений</span><span class="sxs-lookup"><span data-stu-id="0a252-176">App service example</span></span>

<span data-ttu-id="0a252-177">Ниже приведен пример запроса службы приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a252-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="0a252-178">Чтобы использовать службу приложений, необходимо выполнить запрос POST, используя идентификатор устройства (полученный при выполнении вызова GET `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="0a252-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="0a252-179">Чтобы использовать приведенный ниже пример, необходимо установить [приложение Рим](https://aka.ms/romanapp) на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a252-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="0a252-180">В вызове необходимо задать несколько дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="0a252-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="0a252-181">Для *типа* должно быть задано значение *включающее*, для *аппсервиценаме* должно быть задано имя службы приложений, определенной в приложении, *паккажефамилинаме* должно быть задано имя семейства пакетов, заданное в манифесте приложения, а *полезные данные* . содержит ключи и значения для службы, вызываемой в целевом приложении.</span><span class="sxs-lookup"><span data-stu-id="0a252-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="0a252-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a252-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="0a252-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a252-183">Response</span></span>

<span data-ttu-id="0a252-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a252-184">The following is an example of the response.</span></span>

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
