---
title: Отправка команд для устройства
description: 'Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт. После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство. Поддерживаются два типа команд: Лаунчури и Аппсервицес. Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* . Для вызова включающее укажите '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f112c7d3253a0a0801b7542f492c6f3f1f675c81
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053944"
---
# <a name="send-device-command"></a><span data-ttu-id="cf61c-107">Отправка команд для устройства</span><span class="sxs-lookup"><span data-stu-id="cf61c-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf61c-108">Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="cf61c-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="cf61c-109">После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство.</span><span class="sxs-lookup"><span data-stu-id="cf61c-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="cf61c-110">Поддерживаются два типа команд: Лаунчури и Аппсервицес.</span><span class="sxs-lookup"><span data-stu-id="cf61c-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="cf61c-111">Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* .</span><span class="sxs-lookup"><span data-stu-id="cf61c-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="cf61c-112">Для вызова включающее укажите параметры *Type*, *полезная нагрузка*, *паккажефамилинаме*и *аппсервиценаме* .</span><span class="sxs-lookup"><span data-stu-id="cf61c-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf61c-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf61c-113">Permissions</span></span>

<span data-ttu-id="cf61c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf61c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cf61c-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf61c-116">Permission type</span></span>      | <span data-ttu-id="cf61c-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf61c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf61c-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf61c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="cf61c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf61c-119">Not supported.</span></span>    |
|<span data-ttu-id="cf61c-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf61c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf61c-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="cf61c-121">Device.Command</span></span>    |
|<span data-ttu-id="cf61c-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf61c-122">Application</span></span> | <span data-ttu-id="cf61c-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf61c-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf61c-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf61c-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="cf61c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf61c-125">Request headers</span></span>


| <span data-ttu-id="cf61c-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf61c-126">Header</span></span> |<span data-ttu-id="cf61c-127">Значение</span><span class="sxs-lookup"><span data-stu-id="cf61c-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="cf61c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf61c-128">Authorization</span></span>| <span data-ttu-id="cf61c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf61c-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="cf61c-131">Accept</span><span class="sxs-lookup"><span data-stu-id="cf61c-131">Accept</span></span> | <span data-ttu-id="cf61c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="cf61c-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf61c-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf61c-133">Request body</span></span>

<span data-ttu-id="cf61c-134">В тексте запроса добавьте представление свойств команды в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf61c-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="cf61c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf61c-135">Response</span></span>

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
### <a name="command-properties"></a><span data-ttu-id="cf61c-136">Свойства команды</span><span class="sxs-lookup"><span data-stu-id="cf61c-136">Command properties</span></span> 

|<span data-ttu-id="cf61c-137">**Имя**</span><span class="sxs-lookup"><span data-stu-id="cf61c-137">**Name**</span></span>|<span data-ttu-id="cf61c-138">**Тип**</span><span class="sxs-lookup"><span data-stu-id="cf61c-138">**Type**</span></span>|<span data-ttu-id="cf61c-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf61c-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="cf61c-140">payload</span><span class="sxs-lookup"><span data-stu-id="cf61c-140">payload</span></span> | <span data-ttu-id="cf61c-141">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="cf61c-141">microsoft.graph.json</span></span>| <span data-ttu-id="cf61c-142">Полезные данные для отправки в службу приложения или для запуска URI на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cf61c-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="cf61c-143">респонсепайлоад</span><span class="sxs-lookup"><span data-stu-id="cf61c-143">responsePayload</span></span> | <span data-ttu-id="cf61c-144">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="cf61c-144">microsoft.graph.json</span></span>| <span data-ttu-id="cf61c-145">Полезные данные, возвращенные с целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="cf61c-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="cf61c-146">постбаккури</span><span class="sxs-lookup"><span data-stu-id="cf61c-146">postBackURI</span></span> | <span data-ttu-id="cf61c-147">String.</span><span class="sxs-lookup"><span data-stu-id="cf61c-147">String</span></span> | <span data-ttu-id="cf61c-148">Обратный адрес URI для отправки последующих уведомлений об обновлениях.</span><span class="sxs-lookup"><span data-stu-id="cf61c-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="cf61c-149">паккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="cf61c-149">packageFamilyName</span></span> | <span data-ttu-id="cf61c-150">String.</span><span class="sxs-lookup"><span data-stu-id="cf61c-150">String</span></span> | <span data-ttu-id="cf61c-151">Имя семейства пакетов Windows Application.</span><span class="sxs-lookup"><span data-stu-id="cf61c-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="cf61c-152">аппсервиценаме</span><span class="sxs-lookup"><span data-stu-id="cf61c-152">appServiceName</span></span> | <span data-ttu-id="cf61c-153">String.</span><span class="sxs-lookup"><span data-stu-id="cf61c-153">String</span></span> | <span data-ttu-id="cf61c-154">Имя службы приложений, определенной конечным приложением.</span><span class="sxs-lookup"><span data-stu-id="cf61c-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="cf61c-155">Является обязательным при запуске службы приложений.</span><span class="sxs-lookup"><span data-stu-id="cf61c-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="cf61c-156">type</span><span class="sxs-lookup"><span data-stu-id="cf61c-156">type</span></span>| <span data-ttu-id="cf61c-157">String</span><span class="sxs-lookup"><span data-stu-id="cf61c-157">String</span></span> | <span data-ttu-id="cf61c-158">Лаунчури или включающее.</span><span class="sxs-lookup"><span data-stu-id="cf61c-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="cf61c-159">id</span><span class="sxs-lookup"><span data-stu-id="cf61c-159">id</span></span>| <span data-ttu-id="cf61c-160">Строка</span><span class="sxs-lookup"><span data-stu-id="cf61c-160">String</span></span> | <span data-ttu-id="cf61c-161">Идентификатор команды, отправленной на устройство.</span><span class="sxs-lookup"><span data-stu-id="cf61c-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="cf61c-162">актионстатус</span><span class="sxs-lookup"><span data-stu-id="cf61c-162">actionStatus</span></span> | <span data-ttu-id="cf61c-163">String.</span><span class="sxs-lookup"><span data-stu-id="cf61c-163">String</span></span> | <span data-ttu-id="cf61c-164">[Состояние](get-device-command-status.md) команды.</span><span class="sxs-lookup"><span data-stu-id="cf61c-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="cf61c-165">error</span><span class="sxs-lookup"><span data-stu-id="cf61c-165">error</span></span>| <span data-ttu-id="cf61c-166">String.</span><span class="sxs-lookup"><span data-stu-id="cf61c-166">String</span></span>| <span data-ttu-id="cf61c-167">Все ошибки, связанные с запросом от конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="cf61c-167">Any errors associated with the request from the target application.</span></span> |

## <a name="examples"></a><span data-ttu-id="cf61c-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="cf61c-168">Examples</span></span>

### <a name="example-1-launch-uri"></a><span data-ttu-id="cf61c-169">Пример 1: URI запуска</span><span class="sxs-lookup"><span data-stu-id="cf61c-169">Example 1: Launch URI</span></span> 

<span data-ttu-id="cf61c-170">Ниже приведен пример запроса Лаунчури. он запустит URI или приложение на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="cf61c-170">The following is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="cf61c-171">Чтобы запустить URI или приложение, отправьте сообщение POST с использованием идентификатора устройства (получено при вызове GET `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="cf61c-171">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="cf61c-172">Задайте для параметров *Type* значение *лаунчури* и введите значение URI, например https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="cf61c-172">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="cf61c-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf61c-173">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="cf61c-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf61c-174">Response</span></span> 

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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


### <a name="example-2-app-service"></a><span data-ttu-id="cf61c-175">Пример 2: служба приложений</span><span class="sxs-lookup"><span data-stu-id="cf61c-175">Example 2: App service</span></span>

<span data-ttu-id="cf61c-176">В приведенном ниже примере показано, как запросить службу приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cf61c-176">The following example shows how to query an app service on a device.</span></span> <span data-ttu-id="cf61c-177">Чтобы использовать службу приложения, необходимо выполнить запрос POST, используя идентификатор устройства (полученный при выполнении вызова GET `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="cf61c-177">To use an app service, you must do a POST call using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="cf61c-178">Чтобы использовать приведенный ниже пример, необходимо установить [приложение Рим](https://aka.ms/romanapp) на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="cf61c-178">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="cf61c-179">В вызове необходимо задать несколько дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="cf61c-179">Several additional properties must be set in the call.</span></span> <span data-ttu-id="cf61c-180">Для *типа* должно быть задано значение *включающее*, для *аппсервиценаме* должно быть задано имя службы приложений, определенной в приложении, *паккажефамилинаме* должно быть задано имя семейства пакетов, заданное в манифесте приложения, а *полезные данные* . содержит ключи и значения для службы, вызываемой в целевом приложении.</span><span class="sxs-lookup"><span data-stu-id="cf61c-180">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="cf61c-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf61c-181">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cf61c-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf61c-182">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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
