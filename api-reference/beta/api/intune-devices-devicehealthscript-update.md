---
title: Обновление Девицехеалсскрипт
description: Обновление свойств объекта Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd5d44e45639ed59518cc4af413b8db76a6c6430
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311735"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="b9feb-103">Обновление Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="b9feb-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="b9feb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9feb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9feb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9feb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9feb-106">Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="b9feb-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9feb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9feb-107">Prerequisites</span></span>
<span data-ttu-id="b9feb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9feb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9feb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9feb-110">Permission type</span></span>|<span data-ttu-id="b9feb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9feb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9feb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9feb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9feb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9feb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b9feb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9feb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9feb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9feb-115">Not supported.</span></span>|
|<span data-ttu-id="b9feb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9feb-116">Application</span></span>|<span data-ttu-id="b9feb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9feb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9feb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9feb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="b9feb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9feb-119">Request headers</span></span>
|<span data-ttu-id="b9feb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9feb-120">Header</span></span>|<span data-ttu-id="b9feb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b9feb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9feb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9feb-122">Authorization</span></span>|<span data-ttu-id="b9feb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9feb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9feb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b9feb-124">Accept</span></span>|<span data-ttu-id="b9feb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9feb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9feb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9feb-126">Request body</span></span>
<span data-ttu-id="b9feb-127">В тексте запроса добавьте представление объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9feb-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="b9feb-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="b9feb-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="b9feb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9feb-129">Property</span></span>|<span data-ttu-id="b9feb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b9feb-130">Type</span></span>|<span data-ttu-id="b9feb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b9feb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9feb-132">id</span><span class="sxs-lookup"><span data-stu-id="b9feb-132">id</span></span>|<span data-ttu-id="b9feb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b9feb-133">String</span></span>|<span data-ttu-id="b9feb-134">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="b9feb-134">Unique Identifier for the device management script.</span></span> <span data-ttu-id="b9feb-135">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-135">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b9feb-136">displayName</span></span>|<span data-ttu-id="b9feb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b9feb-137">String</span></span>|<span data-ttu-id="b9feb-138">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="b9feb-138">Name of the device management script.</span></span> <span data-ttu-id="b9feb-139">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-139">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-140">description</span><span class="sxs-lookup"><span data-stu-id="b9feb-140">description</span></span>|<span data-ttu-id="b9feb-141">String</span><span class="sxs-lookup"><span data-stu-id="b9feb-141">String</span></span>|<span data-ttu-id="b9feb-142">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="b9feb-142">Optional description for the device management script.</span></span> <span data-ttu-id="b9feb-143">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-143">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="b9feb-144">runSchedule</span></span>|[<span data-ttu-id="b9feb-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="b9feb-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="b9feb-146">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="b9feb-146">The interval for script to run.</span></span> <span data-ttu-id="b9feb-147">Если не определен, сценарий будет выполняться один раз наследуемый от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-147">If not defined the script will run once Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-148">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="b9feb-148">scriptContent</span></span>|<span data-ttu-id="b9feb-149">Binary</span><span class="sxs-lookup"><span data-stu-id="b9feb-149">Binary</span></span>|<span data-ttu-id="b9feb-150">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="b9feb-150">The script content.</span></span> <span data-ttu-id="b9feb-151">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-151">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9feb-152">createdDateTime</span></span>|<span data-ttu-id="b9feb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9feb-153">DateTimeOffset</span></span>|<span data-ttu-id="b9feb-154">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="b9feb-154">The date and time the device management script was created.</span></span> <span data-ttu-id="b9feb-155">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-155">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9feb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b9feb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9feb-157">DateTimeOffset</span></span>|<span data-ttu-id="b9feb-158">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="b9feb-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="b9feb-159">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-159">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="b9feb-160">runAsAccount</span></span>|[<span data-ttu-id="b9feb-161">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="b9feb-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="b9feb-162">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="b9feb-162">Indicates the type of execution context.</span></span> <span data-ttu-id="b9feb-163">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="b9feb-163">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span> <span data-ttu-id="b9feb-164">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="b9feb-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="b9feb-165">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="b9feb-165">enforceSignatureCheck</span></span>|<span data-ttu-id="b9feb-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9feb-166">Boolean</span></span>|<span data-ttu-id="b9feb-167">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="b9feb-167">Indicate whether the script signature needs be checked.</span></span> <span data-ttu-id="b9feb-168">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-168">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-169">fileName</span><span class="sxs-lookup"><span data-stu-id="b9feb-169">fileName</span></span>|<span data-ttu-id="b9feb-170">String</span><span class="sxs-lookup"><span data-stu-id="b9feb-170">String</span></span>|<span data-ttu-id="b9feb-171">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="b9feb-171">Script file name.</span></span> <span data-ttu-id="b9feb-172">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-172">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9feb-173">roleScopeTagIds</span></span>|<span data-ttu-id="b9feb-174">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b9feb-174">String collection</span></span>|<span data-ttu-id="b9feb-175">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="b9feb-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span> <span data-ttu-id="b9feb-176">Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-176">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-177">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="b9feb-177">runAs32Bit</span></span>|<span data-ttu-id="b9feb-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9feb-178">Boolean</span></span>|<span data-ttu-id="b9feb-179">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 – бит, наследуемый от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="b9feb-179">A value indicating whether the PowerShell script should run as 32-bit Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="b9feb-180">комплианцеруле</span><span class="sxs-lookup"><span data-stu-id="b9feb-180">complianceRule</span></span>|[<span data-ttu-id="b9feb-181">девицехеалсскрипткомплианцеруле</span><span class="sxs-lookup"><span data-stu-id="b9feb-181">deviceHealthScriptComplianceRule</span></span>](../resources/intune-devices-devicehealthscriptcompliancerule.md)|<span data-ttu-id="b9feb-182">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b9feb-182">Not yet documented</span></span>|
|<span data-ttu-id="b9feb-183">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="b9feb-183">remediationScriptContent</span></span>|<span data-ttu-id="b9feb-184">Binary</span><span class="sxs-lookup"><span data-stu-id="b9feb-184">Binary</span></span>|<span data-ttu-id="b9feb-185">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b9feb-185">Not yet documented</span></span>|
|<span data-ttu-id="b9feb-186">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="b9feb-186">runRemediationScript</span></span>|<span data-ttu-id="b9feb-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9feb-187">Boolean</span></span>|<span data-ttu-id="b9feb-188">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b9feb-188">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b9feb-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9feb-189">Response</span></span>
<span data-ttu-id="b9feb-190">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9feb-190">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9feb-191">Пример</span><span class="sxs-lookup"><span data-stu-id="b9feb-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9feb-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9feb-192">Request</span></span>
<span data-ttu-id="b9feb-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9feb-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 745

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
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```

### <a name="response"></a><span data-ttu-id="b9feb-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9feb-194">Response</span></span>
<span data-ttu-id="b9feb-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9feb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

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
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```






