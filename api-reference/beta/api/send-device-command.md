---
title: Отправка команд для устройства
description: 'Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт. После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство. Поддерживаются два типа команд: Лаунчури и Аппсервицес. Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* . Для вызова включающее укажите '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a7516798c18ec00f770d5632f3ed3faee1830e64
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453515"
---
# <a name="send-device-command"></a><span data-ttu-id="40d98-107">Отправка команд для устройства</span><span class="sxs-lookup"><span data-stu-id="40d98-107">Send device command</span></span>

<span data-ttu-id="40d98-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40d98-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40d98-109">Этот API позволяет функциям Project Рим выполнять командное устройство, связанное с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="40d98-109">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="40d98-110">После выполнения вызова GET `me/devices`, передайте идентификатор устройства, чтобы выдать команду на устройство.</span><span class="sxs-lookup"><span data-stu-id="40d98-110">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="40d98-111">Поддерживаются два типа команд: Лаунчури и Аппсервицес.</span><span class="sxs-lookup"><span data-stu-id="40d98-111">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="40d98-112">Если вы используете Лаунчури, укажите *тип* и параметры *полезных данных* .</span><span class="sxs-lookup"><span data-stu-id="40d98-112">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="40d98-113">Для вызова включающее укажите параметры *Type*, *полезная нагрузка*, *паккажефамилинаме*и *аппсервиценаме* .</span><span class="sxs-lookup"><span data-stu-id="40d98-113">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="40d98-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40d98-114">Permissions</span></span>

<span data-ttu-id="40d98-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40d98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="40d98-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40d98-117">Permission type</span></span>      | <span data-ttu-id="40d98-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40d98-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40d98-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40d98-119">Delegated (work or school account)</span></span> | <span data-ttu-id="40d98-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40d98-120">Not supported.</span></span>    |
|<span data-ttu-id="40d98-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40d98-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40d98-122">Device.Command</span><span class="sxs-lookup"><span data-stu-id="40d98-122">Device.Command</span></span>    |
|<span data-ttu-id="40d98-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40d98-123">Application</span></span> | <span data-ttu-id="40d98-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40d98-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40d98-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40d98-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="40d98-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40d98-126">Request headers</span></span>


| <span data-ttu-id="40d98-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40d98-127">Header</span></span> |<span data-ttu-id="40d98-128">Значение</span><span class="sxs-lookup"><span data-stu-id="40d98-128">Value</span></span>
|:----|:------|
|<span data-ttu-id="40d98-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40d98-129">Authorization</span></span>| <span data-ttu-id="40d98-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40d98-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="40d98-132">Accept</span><span class="sxs-lookup"><span data-stu-id="40d98-132">Accept</span></span> | <span data-ttu-id="40d98-133">application/json</span><span class="sxs-lookup"><span data-stu-id="40d98-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="40d98-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40d98-134">Request body</span></span>

<span data-ttu-id="40d98-135">В тексте запроса добавьте представление свойств команды в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40d98-135">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="40d98-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="40d98-136">Response</span></span>

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
### <a name="command-properties"></a><span data-ttu-id="40d98-137">Свойства команды</span><span class="sxs-lookup"><span data-stu-id="40d98-137">Command properties</span></span> 

|<span data-ttu-id="40d98-138">**Имя**</span><span class="sxs-lookup"><span data-stu-id="40d98-138">**Name**</span></span>|<span data-ttu-id="40d98-139">**Тип**</span><span class="sxs-lookup"><span data-stu-id="40d98-139">**Type**</span></span>|<span data-ttu-id="40d98-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="40d98-140">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="40d98-141">payload</span><span class="sxs-lookup"><span data-stu-id="40d98-141">payload</span></span> | <span data-ttu-id="40d98-142">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="40d98-142">microsoft.graph.json</span></span>| <span data-ttu-id="40d98-143">Полезные данные для отправки в службу приложения или для запуска URI на устройстве.</span><span class="sxs-lookup"><span data-stu-id="40d98-143">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="40d98-144">респонсепайлоад</span><span class="sxs-lookup"><span data-stu-id="40d98-144">responsePayload</span></span> | <span data-ttu-id="40d98-145">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="40d98-145">microsoft.graph.json</span></span>| <span data-ttu-id="40d98-146">Полезные данные, возвращенные с целевого устройства.</span><span class="sxs-lookup"><span data-stu-id="40d98-146">Payload returned from target device.</span></span> |
|<span data-ttu-id="40d98-147">постбаккури</span><span class="sxs-lookup"><span data-stu-id="40d98-147">postBackURI</span></span> | <span data-ttu-id="40d98-148">String</span><span class="sxs-lookup"><span data-stu-id="40d98-148">String</span></span> | <span data-ttu-id="40d98-149">Обратный адрес URI для отправки последующих уведомлений об обновлениях.</span><span class="sxs-lookup"><span data-stu-id="40d98-149">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="40d98-150">паккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="40d98-150">packageFamilyName</span></span> | <span data-ttu-id="40d98-151">String</span><span class="sxs-lookup"><span data-stu-id="40d98-151">String</span></span> | <span data-ttu-id="40d98-152">Имя семейства пакетов Windows Application.</span><span class="sxs-lookup"><span data-stu-id="40d98-152">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="40d98-153">аппсервиценаме</span><span class="sxs-lookup"><span data-stu-id="40d98-153">appServiceName</span></span> | <span data-ttu-id="40d98-154">String</span><span class="sxs-lookup"><span data-stu-id="40d98-154">String</span></span> | <span data-ttu-id="40d98-155">Имя службы приложений, определенной конечным приложением.</span><span class="sxs-lookup"><span data-stu-id="40d98-155">Name of app service defined by the target application.</span></span> <span data-ttu-id="40d98-156">Является обязательным при запуске службы приложений.</span><span class="sxs-lookup"><span data-stu-id="40d98-156">Required if launching an app service.</span></span> |
|<span data-ttu-id="40d98-157">type</span><span class="sxs-lookup"><span data-stu-id="40d98-157">type</span></span>| <span data-ttu-id="40d98-158">String</span><span class="sxs-lookup"><span data-stu-id="40d98-158">String</span></span> | <span data-ttu-id="40d98-159">Лаунчури или включающее.</span><span class="sxs-lookup"><span data-stu-id="40d98-159">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="40d98-160">id</span><span class="sxs-lookup"><span data-stu-id="40d98-160">id</span></span>| <span data-ttu-id="40d98-161">Строка</span><span class="sxs-lookup"><span data-stu-id="40d98-161">String</span></span> | <span data-ttu-id="40d98-162">Идентификатор команды, отправленной на устройство.</span><span class="sxs-lookup"><span data-stu-id="40d98-162">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="40d98-163">актионстатус</span><span class="sxs-lookup"><span data-stu-id="40d98-163">actionStatus</span></span> | <span data-ttu-id="40d98-164">String</span><span class="sxs-lookup"><span data-stu-id="40d98-164">String</span></span> | <span data-ttu-id="40d98-165">[Состояние](get-device-command-status.md) команды.</span><span class="sxs-lookup"><span data-stu-id="40d98-165">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="40d98-166">error</span><span class="sxs-lookup"><span data-stu-id="40d98-166">error</span></span>| <span data-ttu-id="40d98-167">String</span><span class="sxs-lookup"><span data-stu-id="40d98-167">String</span></span>| <span data-ttu-id="40d98-168">Все ошибки, связанные с запросом от конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="40d98-168">Any errors associated with the request from the target application.</span></span> |

## <a name="examples"></a><span data-ttu-id="40d98-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="40d98-169">Examples</span></span>

### <a name="example-1-launch-uri"></a><span data-ttu-id="40d98-170">Пример 1: URI запуска</span><span class="sxs-lookup"><span data-stu-id="40d98-170">Example 1: Launch URI</span></span> 

<span data-ttu-id="40d98-171">Ниже приведен пример запроса Лаунчури. он запустит URI или приложение на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="40d98-171">The following is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="40d98-172">Чтобы запустить URI или приложение, отправьте сообщение POST с использованием идентификатора устройства (получено при вызове GET `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="40d98-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="40d98-173">Задайте для параметров *Type* значение *лаунчури* и введите значение URI, например https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="40d98-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="40d98-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="40d98-174">Request</span></span>

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
#### <a name="response"></a><span data-ttu-id="40d98-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="40d98-175">Response</span></span> 

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


### <a name="example-2-app-service"></a><span data-ttu-id="40d98-176">Пример 2: служба приложений</span><span class="sxs-lookup"><span data-stu-id="40d98-176">Example 2: App service</span></span>

<span data-ttu-id="40d98-177">В приведенном ниже примере показано, как запросить службу приложения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="40d98-177">The following example shows how to query an app service on a device.</span></span> <span data-ttu-id="40d98-178">Чтобы использовать службу приложения, необходимо выполнить запрос POST, используя идентификатор устройства (полученный при выполнении вызова GET `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="40d98-178">To use an app service, you must do a POST call using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="40d98-179">Чтобы использовать приведенный ниже пример, необходимо установить [приложение Рим](https://aka.ms/romanapp) на целевом устройстве.</span><span class="sxs-lookup"><span data-stu-id="40d98-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="40d98-180">В вызове необходимо задать несколько дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="40d98-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="40d98-181">Для *типа* должно быть задано значение *включающее*, в *аппсервиценаме* должно быть задано имя службы приложений, определенной в приложении, *паккажефамилинаме* должно быть задано имя семейства пакетов, определенное в манифесте приложения, а *полезные данные* содержат ключи и значения для службы, вызываемой в целевом приложении.</span><span class="sxs-lookup"><span data-stu-id="40d98-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="40d98-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="40d98-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="40d98-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="40d98-183">Response</span></span>

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
