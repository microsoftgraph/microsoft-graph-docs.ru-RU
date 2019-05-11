---
title: Обновление deviceManagementScript
description: Обновление свойств объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dc0554456be285f8f6306bfa52033e851164874
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909906"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="d38df-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="d38df-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="d38df-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d38df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d38df-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d38df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d38df-106">Обновление свойств объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="d38df-106">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d38df-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d38df-107">Prerequisites</span></span>
<span data-ttu-id="d38df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d38df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d38df-110">Permission type</span></span>|<span data-ttu-id="d38df-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d38df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d38df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d38df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d38df-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d38df-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d38df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d38df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d38df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d38df-115">Not supported.</span></span>|
|<span data-ttu-id="d38df-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d38df-116">Application</span></span>|<span data-ttu-id="d38df-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d38df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d38df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d38df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="d38df-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d38df-119">Request headers</span></span>
|<span data-ttu-id="d38df-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d38df-120">Header</span></span>|<span data-ttu-id="d38df-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d38df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d38df-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d38df-122">Authorization</span></span>|<span data-ttu-id="d38df-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d38df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d38df-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d38df-124">Accept</span></span>|<span data-ttu-id="d38df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d38df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d38df-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d38df-126">Request body</span></span>
<span data-ttu-id="d38df-127">В тексте запроса добавьте представление объекта [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d38df-127">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="d38df-128">В следующей таблице приведены свойства, необходимые при создании [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="d38df-128">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="d38df-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d38df-129">Property</span></span>|<span data-ttu-id="d38df-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d38df-130">Type</span></span>|<span data-ttu-id="d38df-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d38df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d38df-132">id</span><span class="sxs-lookup"><span data-stu-id="d38df-132">id</span></span>|<span data-ttu-id="d38df-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d38df-133">String</span></span>|<span data-ttu-id="d38df-134">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d38df-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="d38df-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d38df-135">displayName</span></span>|<span data-ttu-id="d38df-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d38df-136">String</span></span>|<span data-ttu-id="d38df-137">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d38df-137">Name of the device management script.</span></span>|
|<span data-ttu-id="d38df-138">description</span><span class="sxs-lookup"><span data-stu-id="d38df-138">description</span></span>|<span data-ttu-id="d38df-139">String</span><span class="sxs-lookup"><span data-stu-id="d38df-139">String</span></span>|<span data-ttu-id="d38df-140">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d38df-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="d38df-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d38df-141">runSchedule</span></span>|[<span data-ttu-id="d38df-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d38df-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="d38df-143">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="d38df-143">The interval for script to run.</span></span> <span data-ttu-id="d38df-144">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="d38df-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="d38df-145">Скриптконтент</span><span class="sxs-lookup"><span data-stu-id="d38df-145">scriptContent</span></span>|<span data-ttu-id="d38df-146">Binary</span><span class="sxs-lookup"><span data-stu-id="d38df-146">Binary</span></span>|<span data-ttu-id="d38df-147">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="d38df-147">The script content.</span></span>|
|<span data-ttu-id="d38df-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d38df-148">createdDateTime</span></span>|<span data-ttu-id="d38df-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d38df-149">DateTimeOffset</span></span>|<span data-ttu-id="d38df-150">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d38df-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="d38df-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d38df-151">lastModifiedDateTime</span></span>|<span data-ttu-id="d38df-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d38df-152">DateTimeOffset</span></span>|<span data-ttu-id="d38df-153">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d38df-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="d38df-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d38df-154">runAsAccount</span></span>|[<span data-ttu-id="d38df-155">Рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="d38df-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d38df-156">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="d38df-156">Indicates the type of execution context.</span></span> <span data-ttu-id="d38df-157">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="d38df-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="d38df-158">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="d38df-158">enforceSignatureCheck</span></span>|<span data-ttu-id="d38df-159">Логический</span><span class="sxs-lookup"><span data-stu-id="d38df-159">Boolean</span></span>|<span data-ttu-id="d38df-160">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="d38df-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="d38df-161">fileName</span><span class="sxs-lookup"><span data-stu-id="d38df-161">fileName</span></span>|<span data-ttu-id="d38df-162">String</span><span class="sxs-lookup"><span data-stu-id="d38df-162">String</span></span>|<span data-ttu-id="d38df-163">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="d38df-163">Script file name.</span></span>|
|<span data-ttu-id="d38df-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d38df-164">roleScopeTagIds</span></span>|<span data-ttu-id="d38df-165">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d38df-165">String collection</span></span>|<span data-ttu-id="d38df-166">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="d38df-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="d38df-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="d38df-167">runAs32Bit</span></span>|<span data-ttu-id="d38df-168">Логический</span><span class="sxs-lookup"><span data-stu-id="d38df-168">Boolean</span></span>|<span data-ttu-id="d38df-169">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="d38df-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="d38df-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38df-170">Response</span></span>
<span data-ttu-id="d38df-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d38df-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38df-172">Пример</span><span class="sxs-lookup"><span data-stu-id="d38df-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d38df-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="d38df-173">Request</span></span>
<span data-ttu-id="d38df-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d38df-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d38df-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38df-175">Response</span></span>
<span data-ttu-id="d38df-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d38df-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




