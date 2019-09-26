---
title: Обновление Девицехеалсскрипт
description: Обновление свойств объекта Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 246f7d00920a096e4e1af328e7bcb7d76c3ba448
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188635"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="4539d-103">Обновление Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="4539d-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="4539d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4539d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4539d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4539d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4539d-106">Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="4539d-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4539d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4539d-107">Prerequisites</span></span>
<span data-ttu-id="4539d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4539d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4539d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4539d-110">Permission type</span></span>|<span data-ttu-id="4539d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4539d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4539d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4539d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4539d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4539d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4539d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4539d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4539d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4539d-115">Not supported.</span></span>|
|<span data-ttu-id="4539d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4539d-116">Application</span></span>|<span data-ttu-id="4539d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4539d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4539d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4539d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="4539d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4539d-119">Request headers</span></span>
|<span data-ttu-id="4539d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4539d-120">Header</span></span>|<span data-ttu-id="4539d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4539d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4539d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4539d-122">Authorization</span></span>|<span data-ttu-id="4539d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4539d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4539d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4539d-124">Accept</span></span>|<span data-ttu-id="4539d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4539d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4539d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4539d-126">Request body</span></span>
<span data-ttu-id="4539d-127">В тексте запроса добавьте представление объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4539d-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="4539d-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="4539d-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="4539d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4539d-129">Property</span></span>|<span data-ttu-id="4539d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4539d-130">Type</span></span>|<span data-ttu-id="4539d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4539d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4539d-132">id</span><span class="sxs-lookup"><span data-stu-id="4539d-132">id</span></span>|<span data-ttu-id="4539d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4539d-133">String</span></span>|<span data-ttu-id="4539d-134">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4539d-134">Unique Identifier for the device management script.</span></span> <span data-ttu-id="4539d-135">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-135">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4539d-136">displayName</span></span>|<span data-ttu-id="4539d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4539d-137">String</span></span>|<span data-ttu-id="4539d-138">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4539d-138">Name of the device management script.</span></span> <span data-ttu-id="4539d-139">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-139">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-140">description</span><span class="sxs-lookup"><span data-stu-id="4539d-140">description</span></span>|<span data-ttu-id="4539d-141">String</span><span class="sxs-lookup"><span data-stu-id="4539d-141">String</span></span>|<span data-ttu-id="4539d-142">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4539d-142">Optional description for the device management script.</span></span> <span data-ttu-id="4539d-143">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-143">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="4539d-144">runSchedule</span></span>|[<span data-ttu-id="4539d-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="4539d-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="4539d-146">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="4539d-146">The interval for script to run.</span></span> <span data-ttu-id="4539d-147">Если не определен, сценарий будет выполняться один раз наследуемый от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-147">If not defined the script will run once Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-148">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="4539d-148">scriptContent</span></span>|<span data-ttu-id="4539d-149">Binary</span><span class="sxs-lookup"><span data-stu-id="4539d-149">Binary</span></span>|<span data-ttu-id="4539d-150">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="4539d-150">The script content.</span></span> <span data-ttu-id="4539d-151">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-151">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4539d-152">createdDateTime</span></span>|<span data-ttu-id="4539d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4539d-153">DateTimeOffset</span></span>|<span data-ttu-id="4539d-154">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4539d-154">The date and time the device management script was created.</span></span> <span data-ttu-id="4539d-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4539d-155">This property is read-only.</span></span> <span data-ttu-id="4539d-156">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-156">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4539d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4539d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4539d-158">DateTimeOffset</span></span>|<span data-ttu-id="4539d-159">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4539d-159">The date and time the device management script was last modified.</span></span> <span data-ttu-id="4539d-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4539d-160">This property is read-only.</span></span> <span data-ttu-id="4539d-161">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-161">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="4539d-162">runAsAccount</span></span>|[<span data-ttu-id="4539d-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="4539d-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="4539d-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="4539d-164">Indicates the type of execution context.</span></span> <span data-ttu-id="4539d-165">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="4539d-165">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span> <span data-ttu-id="4539d-166">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="4539d-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="4539d-167">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="4539d-167">enforceSignatureCheck</span></span>|<span data-ttu-id="4539d-168">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4539d-168">Boolean</span></span>|<span data-ttu-id="4539d-169">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="4539d-169">Indicate whether the script signature needs be checked.</span></span> <span data-ttu-id="4539d-170">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-170">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-171">fileName</span><span class="sxs-lookup"><span data-stu-id="4539d-171">fileName</span></span>|<span data-ttu-id="4539d-172">String</span><span class="sxs-lookup"><span data-stu-id="4539d-172">String</span></span>|<span data-ttu-id="4539d-173">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="4539d-173">Script file name.</span></span> <span data-ttu-id="4539d-174">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-174">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4539d-175">roleScopeTagIds</span></span>|<span data-ttu-id="4539d-176">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4539d-176">String collection</span></span>|<span data-ttu-id="4539d-177">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="4539d-177">List of Scope Tag IDs for this PowerShellScript instance.</span></span> <span data-ttu-id="4539d-178">Наследуется от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-178">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-179">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="4539d-179">runAs32Bit</span></span>|<span data-ttu-id="4539d-180">Boolean.</span><span class="sxs-lookup"><span data-stu-id="4539d-180">Boolean</span></span>|<span data-ttu-id="4539d-181">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 – бит, наследуемый от [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="4539d-181">A value indicating whether the PowerShell script should run as 32-bit Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="4539d-182">комплианцеруле</span><span class="sxs-lookup"><span data-stu-id="4539d-182">complianceRule</span></span>|[<span data-ttu-id="4539d-183">девицехеалсскрипткомплианцеруле</span><span class="sxs-lookup"><span data-stu-id="4539d-183">deviceHealthScriptComplianceRule</span></span>](../resources/intune-devices-devicehealthscriptcompliancerule.md)|<span data-ttu-id="4539d-184">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4539d-184">Not yet documented</span></span>|
|<span data-ttu-id="4539d-185">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="4539d-185">remediationScriptContent</span></span>|<span data-ttu-id="4539d-186">Binary</span><span class="sxs-lookup"><span data-stu-id="4539d-186">Binary</span></span>|<span data-ttu-id="4539d-187">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4539d-187">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4539d-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="4539d-188">Response</span></span>
<span data-ttu-id="4539d-189">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4539d-189">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4539d-190">Пример</span><span class="sxs-lookup"><span data-stu-id="4539d-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="4539d-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="4539d-191">Request</span></span>
<span data-ttu-id="4539d-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4539d-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 712

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
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
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50"
}
```

### <a name="response"></a><span data-ttu-id="4539d-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="4539d-193">Response</span></span>
<span data-ttu-id="4539d-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4539d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
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
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50"
}
```




