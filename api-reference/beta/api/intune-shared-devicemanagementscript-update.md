---
title: Обновление deviceManagementScript
description: Обновление свойств объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f16d40792835086b8c87bf3a3636138deba794d7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458464"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="f1716-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="f1716-103">Update deviceManagementScript</span></span>

<span data-ttu-id="f1716-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f1716-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1716-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1716-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1716-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1716-107">Обновление свойств объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="f1716-107">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1716-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1716-108">Prerequisites</span></span>
<span data-ttu-id="f1716-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1716-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1716-111">Permission type</span></span>|<span data-ttu-id="f1716-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1716-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1716-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1716-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f1716-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f1716-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f1716-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1716-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f1716-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="f1716-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f1716-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1716-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1716-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1716-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1716-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1716-119">Not supported.</span></span>|
|<span data-ttu-id="f1716-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1716-120">Application</span></span>||
| <span data-ttu-id="f1716-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f1716-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f1716-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1716-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f1716-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="f1716-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f1716-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1716-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1716-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1716-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="f1716-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1716-126">Request headers</span></span>
|<span data-ttu-id="f1716-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1716-127">Header</span></span>|<span data-ttu-id="f1716-128">Значение</span><span class="sxs-lookup"><span data-stu-id="f1716-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1716-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1716-129">Authorization</span></span>|<span data-ttu-id="f1716-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1716-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1716-131">Accept</span><span class="sxs-lookup"><span data-stu-id="f1716-131">Accept</span></span>|<span data-ttu-id="f1716-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f1716-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1716-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1716-133">Request body</span></span>
<span data-ttu-id="f1716-134">В тексте запроса добавьте представление объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1716-134">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="f1716-135">В следующей таблице приведены свойства, необходимые при создании [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="f1716-135">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="f1716-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1716-136">Property</span></span>|<span data-ttu-id="f1716-137">Тип</span><span class="sxs-lookup"><span data-stu-id="f1716-137">Type</span></span>|<span data-ttu-id="f1716-138">Описание</span><span class="sxs-lookup"><span data-stu-id="f1716-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1716-139">id</span><span class="sxs-lookup"><span data-stu-id="f1716-139">id</span></span>|<span data-ttu-id="f1716-140">Строка</span><span class="sxs-lookup"><span data-stu-id="f1716-140">String</span></span>|<span data-ttu-id="f1716-141">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f1716-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="f1716-142">displayName</span><span class="sxs-lookup"><span data-stu-id="f1716-142">displayName</span></span>|<span data-ttu-id="f1716-143">Строка</span><span class="sxs-lookup"><span data-stu-id="f1716-143">String</span></span>|<span data-ttu-id="f1716-144">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f1716-144">Name of the device management script.</span></span>|
|<span data-ttu-id="f1716-145">description</span><span class="sxs-lookup"><span data-stu-id="f1716-145">description</span></span>|<span data-ttu-id="f1716-146">String</span><span class="sxs-lookup"><span data-stu-id="f1716-146">String</span></span>|<span data-ttu-id="f1716-147">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f1716-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="f1716-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="f1716-148">runSchedule</span></span>|[<span data-ttu-id="f1716-149">runSchedule</span><span class="sxs-lookup"><span data-stu-id="f1716-149">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="f1716-150">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="f1716-150">The interval for script to run.</span></span> <span data-ttu-id="f1716-151">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="f1716-151">If not defined the script will run once</span></span>|
|<span data-ttu-id="f1716-152">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="f1716-152">scriptContent</span></span>|<span data-ttu-id="f1716-153">Binary</span><span class="sxs-lookup"><span data-stu-id="f1716-153">Binary</span></span>|<span data-ttu-id="f1716-154">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="f1716-154">The script content.</span></span>|
|<span data-ttu-id="f1716-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1716-155">createdDateTime</span></span>|<span data-ttu-id="f1716-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1716-156">DateTimeOffset</span></span>|<span data-ttu-id="f1716-157">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f1716-157">The date and time the device management script was created.</span></span> <span data-ttu-id="f1716-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1716-158">This property is read-only.</span></span>|
|<span data-ttu-id="f1716-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1716-159">lastModifiedDateTime</span></span>|<span data-ttu-id="f1716-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1716-160">DateTimeOffset</span></span>|<span data-ttu-id="f1716-161">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f1716-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="f1716-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1716-162">This property is read-only.</span></span>|
|<span data-ttu-id="f1716-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f1716-163">runAsAccount</span></span>|[<span data-ttu-id="f1716-164">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="f1716-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f1716-165">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="f1716-165">Indicates the type of execution context.</span></span> <span data-ttu-id="f1716-166">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="f1716-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="f1716-167">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="f1716-167">enforceSignatureCheck</span></span>|<span data-ttu-id="f1716-168">Логический</span><span class="sxs-lookup"><span data-stu-id="f1716-168">Boolean</span></span>|<span data-ttu-id="f1716-169">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="f1716-169">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="f1716-170">fileName</span><span class="sxs-lookup"><span data-stu-id="f1716-170">fileName</span></span>|<span data-ttu-id="f1716-171">String</span><span class="sxs-lookup"><span data-stu-id="f1716-171">String</span></span>|<span data-ttu-id="f1716-172">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="f1716-172">Script file name.</span></span>|
|<span data-ttu-id="f1716-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1716-173">roleScopeTagIds</span></span>|<span data-ttu-id="f1716-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1716-174">String collection</span></span>|<span data-ttu-id="f1716-175">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="f1716-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="f1716-176">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="f1716-176">runAs32Bit</span></span>|<span data-ttu-id="f1716-177">Логический</span><span class="sxs-lookup"><span data-stu-id="f1716-177">Boolean</span></span>|<span data-ttu-id="f1716-178">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="f1716-178">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="f1716-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1716-179">Response</span></span>
<span data-ttu-id="f1716-180">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1716-180">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1716-181">Пример</span><span class="sxs-lookup"><span data-stu-id="f1716-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1716-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1716-182">Request</span></span>
<span data-ttu-id="f1716-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1716-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1716-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1716-184">Response</span></span>
<span data-ttu-id="f1716-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1716-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








