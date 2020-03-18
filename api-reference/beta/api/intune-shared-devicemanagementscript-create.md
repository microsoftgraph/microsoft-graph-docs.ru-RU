---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d45177375eca0bfdf6575fc4737d53ce0468645b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800986"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="e7ff5-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="e7ff5-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="e7ff5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7ff5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7ff5-106">Создание нового объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="e7ff5-106">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7ff5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e7ff5-107">Prerequisites</span></span>
<span data-ttu-id="e7ff5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7ff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7ff5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7ff5-110">Permission type</span></span>|<span data-ttu-id="e7ff5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7ff5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7ff5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7ff5-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e7ff5-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e7ff5-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e7ff5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ff5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="e7ff5-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="e7ff5-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e7ff5-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ff5-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e7ff5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7ff5-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7ff5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-118">Not supported.</span></span>|
|<span data-ttu-id="e7ff5-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="e7ff5-119">Application</span></span>||
| <span data-ttu-id="e7ff5-120">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="e7ff5-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e7ff5-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ff5-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="e7ff5-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="e7ff5-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e7ff5-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7ff5-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7ff5-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7ff5-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="e7ff5-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e7ff5-125">Request headers</span></span>
|<span data-ttu-id="e7ff5-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7ff5-126">Header</span></span>|<span data-ttu-id="e7ff5-127">Значение</span><span class="sxs-lookup"><span data-stu-id="e7ff5-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7ff5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7ff5-128">Authorization</span></span>|<span data-ttu-id="e7ff5-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7ff5-130">Accept</span><span class="sxs-lookup"><span data-stu-id="e7ff5-130">Accept</span></span>|<span data-ttu-id="e7ff5-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e7ff5-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7ff5-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7ff5-132">Request body</span></span>
<span data-ttu-id="e7ff5-133">В тексте запроса добавьте представление объекта deviceManagementScript в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-133">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="e7ff5-134">В следующей таблице приведены свойства, необходимые при создании deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-134">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="e7ff5-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7ff5-135">Property</span></span>|<span data-ttu-id="e7ff5-136">Тип</span><span class="sxs-lookup"><span data-stu-id="e7ff5-136">Type</span></span>|<span data-ttu-id="e7ff5-137">Описание</span><span class="sxs-lookup"><span data-stu-id="e7ff5-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7ff5-138">id</span><span class="sxs-lookup"><span data-stu-id="e7ff5-138">id</span></span>|<span data-ttu-id="e7ff5-139">Строка</span><span class="sxs-lookup"><span data-stu-id="e7ff5-139">String</span></span>|<span data-ttu-id="e7ff5-140">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-140">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="e7ff5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="e7ff5-141">displayName</span></span>|<span data-ttu-id="e7ff5-142">Строка</span><span class="sxs-lookup"><span data-stu-id="e7ff5-142">String</span></span>|<span data-ttu-id="e7ff5-143">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-143">Name of the device management script.</span></span>|
|<span data-ttu-id="e7ff5-144">description</span><span class="sxs-lookup"><span data-stu-id="e7ff5-144">description</span></span>|<span data-ttu-id="e7ff5-145">String</span><span class="sxs-lookup"><span data-stu-id="e7ff5-145">String</span></span>|<span data-ttu-id="e7ff5-146">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-146">Optional description for the device management script.</span></span>|
|<span data-ttu-id="e7ff5-147">runSchedule</span><span class="sxs-lookup"><span data-stu-id="e7ff5-147">runSchedule</span></span>|[<span data-ttu-id="e7ff5-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="e7ff5-148">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="e7ff5-149">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-149">The interval for script to run.</span></span> <span data-ttu-id="e7ff5-150">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="e7ff5-150">If not defined the script will run once</span></span>|
|<span data-ttu-id="e7ff5-151">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="e7ff5-151">scriptContent</span></span>|<span data-ttu-id="e7ff5-152">Binary</span><span class="sxs-lookup"><span data-stu-id="e7ff5-152">Binary</span></span>|<span data-ttu-id="e7ff5-153">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-153">The script content.</span></span>|
|<span data-ttu-id="e7ff5-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ff5-154">createdDateTime</span></span>|<span data-ttu-id="e7ff5-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ff5-155">DateTimeOffset</span></span>|<span data-ttu-id="e7ff5-156">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-156">The date and time the device management script was created.</span></span> <span data-ttu-id="e7ff5-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-157">This property is read-only.</span></span>|
|<span data-ttu-id="e7ff5-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7ff5-158">lastModifiedDateTime</span></span>|<span data-ttu-id="e7ff5-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7ff5-159">DateTimeOffset</span></span>|<span data-ttu-id="e7ff5-160">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="e7ff5-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-161">This property is read-only.</span></span>|
|<span data-ttu-id="e7ff5-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="e7ff5-162">runAsAccount</span></span>|[<span data-ttu-id="e7ff5-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="e7ff5-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="e7ff5-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-164">Indicates the type of execution context.</span></span> <span data-ttu-id="e7ff5-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="e7ff5-166">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="e7ff5-166">enforceSignatureCheck</span></span>|<span data-ttu-id="e7ff5-167">Логический</span><span class="sxs-lookup"><span data-stu-id="e7ff5-167">Boolean</span></span>|<span data-ttu-id="e7ff5-168">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-168">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="e7ff5-169">fileName</span><span class="sxs-lookup"><span data-stu-id="e7ff5-169">fileName</span></span>|<span data-ttu-id="e7ff5-170">String</span><span class="sxs-lookup"><span data-stu-id="e7ff5-170">String</span></span>|<span data-ttu-id="e7ff5-171">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-171">Script file name.</span></span>|
|<span data-ttu-id="e7ff5-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7ff5-172">roleScopeTagIds</span></span>|<span data-ttu-id="e7ff5-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e7ff5-173">String collection</span></span>|<span data-ttu-id="e7ff5-174">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-174">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="e7ff5-175">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="e7ff5-175">runAs32Bit</span></span>|<span data-ttu-id="e7ff5-176">Логический</span><span class="sxs-lookup"><span data-stu-id="e7ff5-176">Boolean</span></span>|<span data-ttu-id="e7ff5-177">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="e7ff5-177">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="e7ff5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7ff5-178">Response</span></span>
<span data-ttu-id="e7ff5-179">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-179">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7ff5-180">Пример</span><span class="sxs-lookup"><span data-stu-id="e7ff5-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7ff5-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7ff5-181">Request</span></span>
<span data-ttu-id="e7ff5-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
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

### <a name="response"></a><span data-ttu-id="e7ff5-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7ff5-183">Response</span></span>
<span data-ttu-id="e7ff5-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7ff5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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







