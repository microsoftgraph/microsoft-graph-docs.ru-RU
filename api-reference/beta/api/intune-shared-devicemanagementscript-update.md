---
title: Обновление deviceManagementScript
description: Обновление свойств объекта deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adec750ebb872a6bd228c6d2be691bf05f314207
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692795"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="8a93e-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="8a93e-103">Update deviceManagementScript</span></span>

<span data-ttu-id="8a93e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a93e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a93e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a93e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a93e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a93e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a93e-107">Обновление свойств объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="8a93e-107">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a93e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a93e-108">Prerequisites</span></span>
<span data-ttu-id="8a93e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a93e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a93e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a93e-111">Permission type</span></span>|<span data-ttu-id="8a93e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a93e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a93e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a93e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8a93e-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="8a93e-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8a93e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a93e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8a93e-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="8a93e-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8a93e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a93e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8a93e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a93e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a93e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a93e-119">Not supported.</span></span>|
|<span data-ttu-id="8a93e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a93e-120">Application</span></span>||
| <span data-ttu-id="8a93e-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="8a93e-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8a93e-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a93e-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8a93e-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="8a93e-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8a93e-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a93e-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a93e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a93e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="8a93e-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a93e-126">Request headers</span></span>
|<span data-ttu-id="8a93e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a93e-127">Header</span></span>|<span data-ttu-id="8a93e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8a93e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a93e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a93e-129">Authorization</span></span>|<span data-ttu-id="8a93e-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a93e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a93e-131">Accept</span><span class="sxs-lookup"><span data-stu-id="8a93e-131">Accept</span></span>|<span data-ttu-id="8a93e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8a93e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a93e-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a93e-133">Request body</span></span>
<span data-ttu-id="8a93e-134">В тексте запроса добавьте представление объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a93e-134">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="8a93e-135">В следующей таблице приведены свойства, необходимые при создании [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="8a93e-135">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="8a93e-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a93e-136">Property</span></span>|<span data-ttu-id="8a93e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="8a93e-137">Type</span></span>|<span data-ttu-id="8a93e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8a93e-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a93e-139">id</span><span class="sxs-lookup"><span data-stu-id="8a93e-139">id</span></span>|<span data-ttu-id="8a93e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="8a93e-140">String</span></span>|<span data-ttu-id="8a93e-141">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8a93e-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="8a93e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8a93e-142">displayName</span></span>|<span data-ttu-id="8a93e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="8a93e-143">String</span></span>|<span data-ttu-id="8a93e-144">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8a93e-144">Name of the device management script.</span></span>|
|<span data-ttu-id="8a93e-145">description</span><span class="sxs-lookup"><span data-stu-id="8a93e-145">description</span></span>|<span data-ttu-id="8a93e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8a93e-146">String</span></span>|<span data-ttu-id="8a93e-147">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8a93e-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="8a93e-148">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="8a93e-148">scriptContent</span></span>|<span data-ttu-id="8a93e-149">Binary</span><span class="sxs-lookup"><span data-stu-id="8a93e-149">Binary</span></span>|<span data-ttu-id="8a93e-150">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="8a93e-150">The script content.</span></span>|
|<span data-ttu-id="8a93e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a93e-151">createdDateTime</span></span>|<span data-ttu-id="8a93e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a93e-152">DateTimeOffset</span></span>|<span data-ttu-id="8a93e-153">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8a93e-153">The date and time the device management script was created.</span></span> <span data-ttu-id="8a93e-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a93e-154">This property is read-only.</span></span>|
|<span data-ttu-id="8a93e-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a93e-155">lastModifiedDateTime</span></span>|<span data-ttu-id="8a93e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a93e-156">DateTimeOffset</span></span>|<span data-ttu-id="8a93e-157">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8a93e-157">The date and time the device management script was last modified.</span></span> <span data-ttu-id="8a93e-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a93e-158">This property is read-only.</span></span>|
|<span data-ttu-id="8a93e-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="8a93e-159">runAsAccount</span></span>|[<span data-ttu-id="8a93e-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="8a93e-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="8a93e-161">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="8a93e-161">Indicates the type of execution context.</span></span> <span data-ttu-id="8a93e-162">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8a93e-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="8a93e-163">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="8a93e-163">enforceSignatureCheck</span></span>|<span data-ttu-id="8a93e-164">Логический</span><span class="sxs-lookup"><span data-stu-id="8a93e-164">Boolean</span></span>|<span data-ttu-id="8a93e-165">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="8a93e-165">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="8a93e-166">fileName</span><span class="sxs-lookup"><span data-stu-id="8a93e-166">fileName</span></span>|<span data-ttu-id="8a93e-167">String</span><span class="sxs-lookup"><span data-stu-id="8a93e-167">String</span></span>|<span data-ttu-id="8a93e-168">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="8a93e-168">Script file name.</span></span>|
|<span data-ttu-id="8a93e-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a93e-169">roleScopeTagIds</span></span>|<span data-ttu-id="8a93e-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8a93e-170">String collection</span></span>|<span data-ttu-id="8a93e-171">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="8a93e-171">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="8a93e-172">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="8a93e-172">runAs32Bit</span></span>|<span data-ttu-id="8a93e-173">Логический</span><span class="sxs-lookup"><span data-stu-id="8a93e-173">Boolean</span></span>|<span data-ttu-id="8a93e-174">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="8a93e-174">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="8a93e-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a93e-175">Response</span></span>
<span data-ttu-id="8a93e-176">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a93e-176">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a93e-177">Пример</span><span class="sxs-lookup"><span data-stu-id="8a93e-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a93e-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a93e-178">Request</span></span>
<span data-ttu-id="8a93e-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a93e-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="8a93e-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a93e-180">Response</span></span>
<span data-ttu-id="8a93e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a93e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








