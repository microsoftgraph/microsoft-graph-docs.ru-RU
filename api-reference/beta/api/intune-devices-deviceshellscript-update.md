---
title: Обновление Девицешеллскрипт
description: Обновление свойств объекта Девицешеллскрипт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9e3c2da2008b5e44f4b13449abd6b63251fe08f
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034750"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="58436-103">Обновление Девицешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="58436-103">Update deviceShellScript</span></span>

> <span data-ttu-id="58436-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58436-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58436-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58436-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58436-106">Обновление свойств объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="58436-106">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58436-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58436-107">Prerequisites</span></span>
<span data-ttu-id="58436-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58436-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58436-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58436-110">Permission type</span></span>|<span data-ttu-id="58436-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58436-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58436-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58436-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58436-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58436-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58436-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58436-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58436-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58436-115">Not supported.</span></span>|
|<span data-ttu-id="58436-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="58436-116">Application</span></span>|<span data-ttu-id="58436-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58436-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58436-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58436-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="58436-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58436-119">Request headers</span></span>
|<span data-ttu-id="58436-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58436-120">Header</span></span>|<span data-ttu-id="58436-121">Значение</span><span class="sxs-lookup"><span data-stu-id="58436-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58436-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58436-122">Authorization</span></span>|<span data-ttu-id="58436-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58436-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58436-124">Accept</span><span class="sxs-lookup"><span data-stu-id="58436-124">Accept</span></span>|<span data-ttu-id="58436-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58436-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58436-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58436-126">Request body</span></span>
<span data-ttu-id="58436-127">В тексте запроса добавьте представление объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58436-127">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="58436-128">В следующей таблице приведены свойства, необходимые при создании [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="58436-128">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="58436-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58436-129">Property</span></span>|<span data-ttu-id="58436-130">Тип</span><span class="sxs-lookup"><span data-stu-id="58436-130">Type</span></span>|<span data-ttu-id="58436-131">Описание</span><span class="sxs-lookup"><span data-stu-id="58436-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58436-132">ексекутионфрекуенци</span><span class="sxs-lookup"><span data-stu-id="58436-132">executionFrequency</span></span>|<span data-ttu-id="58436-133">Длительность</span><span class="sxs-lookup"><span data-stu-id="58436-133">Duration</span></span>|<span data-ttu-id="58436-134">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="58436-134">The interval for script to run.</span></span> <span data-ttu-id="58436-135">Если он не определен, сценарий выполняется один раз.</span><span class="sxs-lookup"><span data-stu-id="58436-135">If not defined, the script runs once.</span></span>|
|<span data-ttu-id="58436-136">ретрикаунт</span><span class="sxs-lookup"><span data-stu-id="58436-136">retryCount</span></span>|<span data-ttu-id="58436-137">Int32</span><span class="sxs-lookup"><span data-stu-id="58436-137">Int32</span></span>|<span data-ttu-id="58436-138">Количество повторных попыток выполнения скрипта в случае сбоя.</span><span class="sxs-lookup"><span data-stu-id="58436-138">The number of times for the script to be retried if it fails.</span></span>|
|<span data-ttu-id="58436-139">блоккексекутионнотификатионс</span><span class="sxs-lookup"><span data-stu-id="58436-139">blockExecutionNotifications</span></span>|<span data-ttu-id="58436-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="58436-140">Boolean</span></span>|<span data-ttu-id="58436-141">Указывает, является ли пользователь уведомленным при запуске скрипта.</span><span class="sxs-lookup"><span data-stu-id="58436-141">Indicates whether the user is notified when a script runs.</span></span>|
|<span data-ttu-id="58436-142">id</span><span class="sxs-lookup"><span data-stu-id="58436-142">id</span></span>|<span data-ttu-id="58436-143">Строка</span><span class="sxs-lookup"><span data-stu-id="58436-143">String</span></span>|<span data-ttu-id="58436-144">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="58436-144">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="58436-145">displayName</span><span class="sxs-lookup"><span data-stu-id="58436-145">displayName</span></span>|<span data-ttu-id="58436-146">Строка</span><span class="sxs-lookup"><span data-stu-id="58436-146">String</span></span>|<span data-ttu-id="58436-147">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="58436-147">The name of the device management script.</span></span>|
|<span data-ttu-id="58436-148">description</span><span class="sxs-lookup"><span data-stu-id="58436-148">description</span></span>|<span data-ttu-id="58436-149">String</span><span class="sxs-lookup"><span data-stu-id="58436-149">String</span></span>|<span data-ttu-id="58436-150">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="58436-150">Optional description for the device management script.</span></span>|
|<span data-ttu-id="58436-151">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="58436-151">scriptContent</span></span>|<span data-ttu-id="58436-152">Binary</span><span class="sxs-lookup"><span data-stu-id="58436-152">Binary</span></span>|<span data-ttu-id="58436-153">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="58436-153">The script content.</span></span>|
|<span data-ttu-id="58436-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58436-154">createdDateTime</span></span>|<span data-ttu-id="58436-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58436-155">DateTimeOffset</span></span>|<span data-ttu-id="58436-156">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="58436-156">The date and time the device management script was created.</span></span> <span data-ttu-id="58436-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="58436-157">This property is read-only.</span></span>|
|<span data-ttu-id="58436-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58436-158">lastModifiedDateTime</span></span>|<span data-ttu-id="58436-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58436-159">DateTimeOffset</span></span>|<span data-ttu-id="58436-160">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="58436-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="58436-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="58436-161">This property is read-only.</span></span>|
|<span data-ttu-id="58436-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="58436-162">runAsAccount</span></span>|[<span data-ttu-id="58436-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="58436-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="58436-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="58436-164">Indicates the type of execution context.</span></span> <span data-ttu-id="58436-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="58436-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="58436-166">fileName</span><span class="sxs-lookup"><span data-stu-id="58436-166">fileName</span></span>|<span data-ttu-id="58436-167">String</span><span class="sxs-lookup"><span data-stu-id="58436-167">String</span></span>|<span data-ttu-id="58436-168">Имя файла скрипта.</span><span class="sxs-lookup"><span data-stu-id="58436-168">The script file name.</span></span>|
|<span data-ttu-id="58436-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58436-169">roleScopeTagIds</span></span>|<span data-ttu-id="58436-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="58436-170">String collection</span></span>|<span data-ttu-id="58436-171">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="58436-171">The list of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="58436-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="58436-172">Response</span></span>
<span data-ttu-id="58436-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58436-173">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58436-174">Пример</span><span class="sxs-lookup"><span data-stu-id="58436-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="58436-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="58436-175">Request</span></span>
<span data-ttu-id="58436-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58436-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="58436-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="58436-177">Response</span></span>
<span data-ttu-id="58436-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58436-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "id": "ca9e0ad8-0ad8-ca9e-d80a-9ecad80a9eca",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



