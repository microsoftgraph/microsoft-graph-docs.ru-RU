---
title: Обновление deviceManagementScript
description: Обновление свойств объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a65a2b761a604a592fda4c3b205ada9a1019fd0c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201038"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="2c6e6-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="2c6e6-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="2c6e6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c6e6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c6e6-106">Обновление свойств объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="2c6e6-106">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c6e6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2c6e6-107">Prerequisites</span></span>
<span data-ttu-id="2c6e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c6e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c6e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c6e6-110">Permission type</span></span>|<span data-ttu-id="2c6e6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c6e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c6e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c6e6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2c6e6-113">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2c6e6-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2c6e6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6e6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2c6e6-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2c6e6-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2c6e6-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6e6-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2c6e6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c6e6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c6e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-118">Not supported.</span></span>|
|<span data-ttu-id="2c6e6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c6e6-119">Application</span></span>||
| <span data-ttu-id="2c6e6-120">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2c6e6-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2c6e6-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6e6-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2c6e6-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2c6e6-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2c6e6-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6e6-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c6e6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c6e6-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="2c6e6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c6e6-125">Request headers</span></span>
|<span data-ttu-id="2c6e6-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c6e6-126">Header</span></span>|<span data-ttu-id="2c6e6-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2c6e6-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c6e6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c6e6-128">Authorization</span></span>|<span data-ttu-id="2c6e6-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c6e6-130">Accept</span><span class="sxs-lookup"><span data-stu-id="2c6e6-130">Accept</span></span>|<span data-ttu-id="2c6e6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2c6e6-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c6e6-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c6e6-132">Request body</span></span>
<span data-ttu-id="2c6e6-133">В тексте запроса добавьте представление объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-133">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="2c6e6-134">В следующей таблице приведены свойства, необходимые при создании [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="2c6e6-134">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="2c6e6-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c6e6-135">Property</span></span>|<span data-ttu-id="2c6e6-136">Тип</span><span class="sxs-lookup"><span data-stu-id="2c6e6-136">Type</span></span>|<span data-ttu-id="2c6e6-137">Описание</span><span class="sxs-lookup"><span data-stu-id="2c6e6-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c6e6-138">id</span><span class="sxs-lookup"><span data-stu-id="2c6e6-138">id</span></span>|<span data-ttu-id="2c6e6-139">Строка</span><span class="sxs-lookup"><span data-stu-id="2c6e6-139">String</span></span>|<span data-ttu-id="2c6e6-140">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-140">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="2c6e6-141">displayName</span><span class="sxs-lookup"><span data-stu-id="2c6e6-141">displayName</span></span>|<span data-ttu-id="2c6e6-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2c6e6-142">String</span></span>|<span data-ttu-id="2c6e6-143">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-143">Name of the device management script.</span></span>|
|<span data-ttu-id="2c6e6-144">description</span><span class="sxs-lookup"><span data-stu-id="2c6e6-144">description</span></span>|<span data-ttu-id="2c6e6-145">String</span><span class="sxs-lookup"><span data-stu-id="2c6e6-145">String</span></span>|<span data-ttu-id="2c6e6-146">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-146">Optional description for the device management script.</span></span>|
|<span data-ttu-id="2c6e6-147">runSchedule</span><span class="sxs-lookup"><span data-stu-id="2c6e6-147">runSchedule</span></span>|[<span data-ttu-id="2c6e6-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="2c6e6-148">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="2c6e6-149">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-149">The interval for script to run.</span></span> <span data-ttu-id="2c6e6-150">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="2c6e6-150">If not defined the script will run once</span></span>|
|<span data-ttu-id="2c6e6-151">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="2c6e6-151">scriptContent</span></span>|<span data-ttu-id="2c6e6-152">Binary</span><span class="sxs-lookup"><span data-stu-id="2c6e6-152">Binary</span></span>|<span data-ttu-id="2c6e6-153">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-153">The script content.</span></span>|
|<span data-ttu-id="2c6e6-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c6e6-154">createdDateTime</span></span>|<span data-ttu-id="2c6e6-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c6e6-155">DateTimeOffset</span></span>|<span data-ttu-id="2c6e6-156">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-156">The date and time the device management script was created.</span></span> <span data-ttu-id="2c6e6-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-157">This property is read-only.</span></span>|
|<span data-ttu-id="2c6e6-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c6e6-158">lastModifiedDateTime</span></span>|<span data-ttu-id="2c6e6-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c6e6-159">DateTimeOffset</span></span>|<span data-ttu-id="2c6e6-160">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="2c6e6-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-161">This property is read-only.</span></span>|
|<span data-ttu-id="2c6e6-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="2c6e6-162">runAsAccount</span></span>|[<span data-ttu-id="2c6e6-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="2c6e6-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="2c6e6-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-164">Indicates the type of execution context.</span></span> <span data-ttu-id="2c6e6-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="2c6e6-166">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="2c6e6-166">enforceSignatureCheck</span></span>|<span data-ttu-id="2c6e6-167">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-167">Boolean</span></span>|<span data-ttu-id="2c6e6-168">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-168">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="2c6e6-169">fileName</span><span class="sxs-lookup"><span data-stu-id="2c6e6-169">fileName</span></span>|<span data-ttu-id="2c6e6-170">String</span><span class="sxs-lookup"><span data-stu-id="2c6e6-170">String</span></span>|<span data-ttu-id="2c6e6-171">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-171">Script file name.</span></span>|
|<span data-ttu-id="2c6e6-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c6e6-172">roleScopeTagIds</span></span>|<span data-ttu-id="2c6e6-173">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2c6e6-173">String collection</span></span>|<span data-ttu-id="2c6e6-174">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-174">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="2c6e6-175">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="2c6e6-175">runAs32Bit</span></span>|<span data-ttu-id="2c6e6-176">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-176">Boolean</span></span>|<span data-ttu-id="2c6e6-177">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="2c6e6-177">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="2c6e6-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c6e6-178">Response</span></span>
<span data-ttu-id="2c6e6-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-179">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c6e6-180">Пример</span><span class="sxs-lookup"><span data-stu-id="2c6e6-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c6e6-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c6e6-181">Request</span></span>
<span data-ttu-id="2c6e6-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c6e6-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c6e6-183">Response</span></span>
<span data-ttu-id="2c6e6-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




