---
title: Обновление deviceManagementScript
description: Обновление свойств объекта deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2df66d7a5e5bb22d74c898c012e7d177784f9ffd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153671"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="5f203-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="5f203-103">Update deviceManagementScript</span></span>

<span data-ttu-id="5f203-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f203-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f203-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f203-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f203-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f203-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f203-107">Обновление свойств объекта [deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5f203-107">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f203-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f203-108">Prerequisites</span></span>
<span data-ttu-id="5f203-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f203-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f203-111">Permission type</span></span>|<span data-ttu-id="5f203-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f203-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f203-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f203-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5f203-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5f203-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5f203-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f203-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5f203-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5f203-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5f203-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f203-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5f203-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f203-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f203-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f203-119">Not supported.</span></span>|
|<span data-ttu-id="5f203-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f203-120">Application</span></span>||
| <span data-ttu-id="5f203-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5f203-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5f203-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f203-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5f203-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5f203-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5f203-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f203-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f203-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f203-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="5f203-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5f203-126">Request headers</span></span>
|<span data-ttu-id="5f203-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f203-127">Header</span></span>|<span data-ttu-id="5f203-128">Значение</span><span class="sxs-lookup"><span data-stu-id="5f203-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f203-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f203-129">Authorization</span></span>|<span data-ttu-id="5f203-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f203-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f203-131">Accept</span><span class="sxs-lookup"><span data-stu-id="5f203-131">Accept</span></span>|<span data-ttu-id="5f203-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5f203-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f203-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f203-133">Request body</span></span>
<span data-ttu-id="5f203-134">В теле запроса укажу представление объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="5f203-134">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="5f203-135">В следующей таблице показаны свойства, необходимые при создании [deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="5f203-135">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="5f203-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f203-136">Property</span></span>|<span data-ttu-id="5f203-137">Тип</span><span class="sxs-lookup"><span data-stu-id="5f203-137">Type</span></span>|<span data-ttu-id="5f203-138">Описание</span><span class="sxs-lookup"><span data-stu-id="5f203-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f203-139">id</span><span class="sxs-lookup"><span data-stu-id="5f203-139">id</span></span>|<span data-ttu-id="5f203-140">String</span><span class="sxs-lookup"><span data-stu-id="5f203-140">String</span></span>|<span data-ttu-id="5f203-141">Уникальный идентификатор сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5f203-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="5f203-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5f203-142">displayName</span></span>|<span data-ttu-id="5f203-143">String</span><span class="sxs-lookup"><span data-stu-id="5f203-143">String</span></span>|<span data-ttu-id="5f203-144">Имя сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5f203-144">Name of the device management script.</span></span>|
|<span data-ttu-id="5f203-145">description</span><span class="sxs-lookup"><span data-stu-id="5f203-145">description</span></span>|<span data-ttu-id="5f203-146">String</span><span class="sxs-lookup"><span data-stu-id="5f203-146">String</span></span>|<span data-ttu-id="5f203-147">Необязательное описание сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5f203-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="5f203-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="5f203-148">scriptContent</span></span>|<span data-ttu-id="5f203-149">Binary</span><span class="sxs-lookup"><span data-stu-id="5f203-149">Binary</span></span>|<span data-ttu-id="5f203-150">Содержимое сценария.</span><span class="sxs-lookup"><span data-stu-id="5f203-150">The script content.</span></span>|
|<span data-ttu-id="5f203-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f203-151">createdDateTime</span></span>|<span data-ttu-id="5f203-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f203-152">DateTimeOffset</span></span>|<span data-ttu-id="5f203-153">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5f203-153">The date and time the device management script was created.</span></span> <span data-ttu-id="5f203-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f203-154">This property is read-only.</span></span>|
|<span data-ttu-id="5f203-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f203-155">lastModifiedDateTime</span></span>|<span data-ttu-id="5f203-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f203-156">DateTimeOffset</span></span>|<span data-ttu-id="5f203-157">Дата и время последнего изменения сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5f203-157">The date and time the device management script was last modified.</span></span> <span data-ttu-id="5f203-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f203-158">This property is read-only.</span></span>|
|<span data-ttu-id="5f203-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="5f203-159">runAsAccount</span></span>|[<span data-ttu-id="5f203-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="5f203-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="5f203-161">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="5f203-161">Indicates the type of execution context.</span></span> <span data-ttu-id="5f203-162">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="5f203-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="5f203-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="5f203-163">enforceSignatureCheck</span></span>|<span data-ttu-id="5f203-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f203-164">Boolean</span></span>|<span data-ttu-id="5f203-165">Указать, требуется ли проверять подпись сценария.</span><span class="sxs-lookup"><span data-stu-id="5f203-165">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="5f203-166">fileName</span><span class="sxs-lookup"><span data-stu-id="5f203-166">fileName</span></span>|<span data-ttu-id="5f203-167">String</span><span class="sxs-lookup"><span data-stu-id="5f203-167">String</span></span>|<span data-ttu-id="5f203-168">Имя файла скрипта.</span><span class="sxs-lookup"><span data-stu-id="5f203-168">Script file name.</span></span>|
|<span data-ttu-id="5f203-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5f203-169">roleScopeTagIds</span></span>|<span data-ttu-id="5f203-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5f203-170">String collection</span></span>|<span data-ttu-id="5f203-171">Список ИД тегов области для этого экземпляра PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="5f203-171">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="5f203-172">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="5f203-172">runAs32Bit</span></span>|<span data-ttu-id="5f203-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f203-173">Boolean</span></span>|<span data-ttu-id="5f203-174">Значение, указывающее, должен ли сценарий PowerShell работать как 32-битный</span><span class="sxs-lookup"><span data-stu-id="5f203-174">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="5f203-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f203-175">Response</span></span>
<span data-ttu-id="5f203-176">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f203-176">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f203-177">Пример</span><span class="sxs-lookup"><span data-stu-id="5f203-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f203-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f203-178">Request</span></span>
<span data-ttu-id="5f203-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f203-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f203-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f203-180">Response</span></span>
<span data-ttu-id="5f203-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f203-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
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







