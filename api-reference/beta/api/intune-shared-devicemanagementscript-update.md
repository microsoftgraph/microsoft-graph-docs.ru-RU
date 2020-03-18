---
title: Обновление deviceManagementScript
description: Обновление свойств объекта deviceManagementScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3d27fdbaf7de530783c4751c7898dd972f45db2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800951"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="08f0a-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="08f0a-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="08f0a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08f0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08f0a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08f0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08f0a-106">Обновление свойств объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="08f0a-106">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08f0a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08f0a-107">Prerequisites</span></span>
<span data-ttu-id="08f0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08f0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08f0a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08f0a-110">Permission type</span></span>|<span data-ttu-id="08f0a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08f0a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08f0a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08f0a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="08f0a-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="08f0a-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="08f0a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f0a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="08f0a-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="08f0a-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="08f0a-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f0a-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="08f0a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08f0a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08f0a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08f0a-118">Not supported.</span></span>|
|<span data-ttu-id="08f0a-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="08f0a-119">Application</span></span>||
| <span data-ttu-id="08f0a-120">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="08f0a-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="08f0a-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f0a-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="08f0a-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="08f0a-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="08f0a-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f0a-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08f0a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08f0a-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="08f0a-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08f0a-125">Request headers</span></span>
|<span data-ttu-id="08f0a-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08f0a-126">Header</span></span>|<span data-ttu-id="08f0a-127">Значение</span><span class="sxs-lookup"><span data-stu-id="08f0a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08f0a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="08f0a-128">Authorization</span></span>|<span data-ttu-id="08f0a-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08f0a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08f0a-130">Accept</span><span class="sxs-lookup"><span data-stu-id="08f0a-130">Accept</span></span>|<span data-ttu-id="08f0a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="08f0a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08f0a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08f0a-132">Request body</span></span>
<span data-ttu-id="08f0a-133">В тексте запроса добавьте представление объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08f0a-133">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="08f0a-134">В следующей таблице приведены свойства, необходимые при создании [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="08f0a-134">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="08f0a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="08f0a-135">Property</span></span>|<span data-ttu-id="08f0a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="08f0a-136">Type</span></span>|<span data-ttu-id="08f0a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="08f0a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08f0a-138">id</span><span class="sxs-lookup"><span data-stu-id="08f0a-138">id</span></span>|<span data-ttu-id="08f0a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="08f0a-139">String</span></span>|<span data-ttu-id="08f0a-140">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="08f0a-140">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="08f0a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="08f0a-141">displayName</span></span>|<span data-ttu-id="08f0a-142">Строка</span><span class="sxs-lookup"><span data-stu-id="08f0a-142">String</span></span>|<span data-ttu-id="08f0a-143">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="08f0a-143">Name of the device management script.</span></span>|
|<span data-ttu-id="08f0a-144">description</span><span class="sxs-lookup"><span data-stu-id="08f0a-144">description</span></span>|<span data-ttu-id="08f0a-145">String</span><span class="sxs-lookup"><span data-stu-id="08f0a-145">String</span></span>|<span data-ttu-id="08f0a-146">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="08f0a-146">Optional description for the device management script.</span></span>|
|<span data-ttu-id="08f0a-147">runSchedule</span><span class="sxs-lookup"><span data-stu-id="08f0a-147">runSchedule</span></span>|[<span data-ttu-id="08f0a-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="08f0a-148">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="08f0a-149">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="08f0a-149">The interval for script to run.</span></span> <span data-ttu-id="08f0a-150">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="08f0a-150">If not defined the script will run once</span></span>|
|<span data-ttu-id="08f0a-151">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="08f0a-151">scriptContent</span></span>|<span data-ttu-id="08f0a-152">Binary</span><span class="sxs-lookup"><span data-stu-id="08f0a-152">Binary</span></span>|<span data-ttu-id="08f0a-153">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="08f0a-153">The script content.</span></span>|
|<span data-ttu-id="08f0a-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08f0a-154">createdDateTime</span></span>|<span data-ttu-id="08f0a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f0a-155">DateTimeOffset</span></span>|<span data-ttu-id="08f0a-156">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="08f0a-156">The date and time the device management script was created.</span></span> <span data-ttu-id="08f0a-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08f0a-157">This property is read-only.</span></span>|
|<span data-ttu-id="08f0a-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08f0a-158">lastModifiedDateTime</span></span>|<span data-ttu-id="08f0a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f0a-159">DateTimeOffset</span></span>|<span data-ttu-id="08f0a-160">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="08f0a-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="08f0a-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08f0a-161">This property is read-only.</span></span>|
|<span data-ttu-id="08f0a-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="08f0a-162">runAsAccount</span></span>|[<span data-ttu-id="08f0a-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="08f0a-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="08f0a-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="08f0a-164">Indicates the type of execution context.</span></span> <span data-ttu-id="08f0a-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="08f0a-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="08f0a-166">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="08f0a-166">enforceSignatureCheck</span></span>|<span data-ttu-id="08f0a-167">Логический</span><span class="sxs-lookup"><span data-stu-id="08f0a-167">Boolean</span></span>|<span data-ttu-id="08f0a-168">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="08f0a-168">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="08f0a-169">fileName</span><span class="sxs-lookup"><span data-stu-id="08f0a-169">fileName</span></span>|<span data-ttu-id="08f0a-170">String</span><span class="sxs-lookup"><span data-stu-id="08f0a-170">String</span></span>|<span data-ttu-id="08f0a-171">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="08f0a-171">Script file name.</span></span>|
|<span data-ttu-id="08f0a-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08f0a-172">roleScopeTagIds</span></span>|<span data-ttu-id="08f0a-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="08f0a-173">String collection</span></span>|<span data-ttu-id="08f0a-174">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="08f0a-174">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="08f0a-175">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="08f0a-175">runAs32Bit</span></span>|<span data-ttu-id="08f0a-176">Логический</span><span class="sxs-lookup"><span data-stu-id="08f0a-176">Boolean</span></span>|<span data-ttu-id="08f0a-177">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="08f0a-177">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="08f0a-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="08f0a-178">Response</span></span>
<span data-ttu-id="08f0a-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08f0a-179">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08f0a-180">Пример</span><span class="sxs-lookup"><span data-stu-id="08f0a-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="08f0a-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="08f0a-181">Request</span></span>
<span data-ttu-id="08f0a-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08f0a-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="08f0a-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="08f0a-183">Response</span></span>
<span data-ttu-id="08f0a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08f0a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```







