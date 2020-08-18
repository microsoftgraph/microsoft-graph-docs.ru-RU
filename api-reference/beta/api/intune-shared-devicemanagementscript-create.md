---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9fe1cd9b413e3062e6c5ec06770160f0b73c7b08
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792291"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="096cc-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="096cc-103">Create deviceManagementScript</span></span>

<span data-ttu-id="096cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="096cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="096cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="096cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="096cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="096cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="096cc-107">Создание нового объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="096cc-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="096cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="096cc-108">Prerequisites</span></span>
<span data-ttu-id="096cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="096cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="096cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="096cc-111">Permission type</span></span>|<span data-ttu-id="096cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="096cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="096cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="096cc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="096cc-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="096cc-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="096cc-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096cc-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="096cc-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="096cc-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="096cc-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096cc-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="096cc-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="096cc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="096cc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="096cc-119">Not supported.</span></span>|
|<span data-ttu-id="096cc-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="096cc-120">Application</span></span>||
| <span data-ttu-id="096cc-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="096cc-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="096cc-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096cc-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="096cc-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="096cc-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="096cc-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096cc-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="096cc-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="096cc-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="096cc-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="096cc-126">Request headers</span></span>
|<span data-ttu-id="096cc-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="096cc-127">Header</span></span>|<span data-ttu-id="096cc-128">Значение</span><span class="sxs-lookup"><span data-stu-id="096cc-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="096cc-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="096cc-129">Authorization</span></span>|<span data-ttu-id="096cc-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="096cc-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="096cc-131">Accept</span><span class="sxs-lookup"><span data-stu-id="096cc-131">Accept</span></span>|<span data-ttu-id="096cc-132">application/json</span><span class="sxs-lookup"><span data-stu-id="096cc-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="096cc-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="096cc-133">Request body</span></span>
<span data-ttu-id="096cc-134">В тексте запроса добавьте представление объекта deviceManagementScript в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="096cc-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="096cc-135">В следующей таблице приведены свойства, необходимые при создании deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="096cc-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="096cc-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="096cc-136">Property</span></span>|<span data-ttu-id="096cc-137">Тип</span><span class="sxs-lookup"><span data-stu-id="096cc-137">Type</span></span>|<span data-ttu-id="096cc-138">Описание</span><span class="sxs-lookup"><span data-stu-id="096cc-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="096cc-139">id</span><span class="sxs-lookup"><span data-stu-id="096cc-139">id</span></span>|<span data-ttu-id="096cc-140">String</span><span class="sxs-lookup"><span data-stu-id="096cc-140">String</span></span>|<span data-ttu-id="096cc-141">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="096cc-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="096cc-142">displayName</span><span class="sxs-lookup"><span data-stu-id="096cc-142">displayName</span></span>|<span data-ttu-id="096cc-143">String</span><span class="sxs-lookup"><span data-stu-id="096cc-143">String</span></span>|<span data-ttu-id="096cc-144">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="096cc-144">Name of the device management script.</span></span>|
|<span data-ttu-id="096cc-145">description</span><span class="sxs-lookup"><span data-stu-id="096cc-145">description</span></span>|<span data-ttu-id="096cc-146">String</span><span class="sxs-lookup"><span data-stu-id="096cc-146">String</span></span>|<span data-ttu-id="096cc-147">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="096cc-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="096cc-148">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="096cc-148">scriptContent</span></span>|<span data-ttu-id="096cc-149">Binary</span><span class="sxs-lookup"><span data-stu-id="096cc-149">Binary</span></span>|<span data-ttu-id="096cc-150">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="096cc-150">The script content.</span></span>|
|<span data-ttu-id="096cc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="096cc-151">createdDateTime</span></span>|<span data-ttu-id="096cc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="096cc-152">DateTimeOffset</span></span>|<span data-ttu-id="096cc-153">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="096cc-153">The date and time the device management script was created.</span></span> <span data-ttu-id="096cc-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="096cc-154">This property is read-only.</span></span>|
|<span data-ttu-id="096cc-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="096cc-155">lastModifiedDateTime</span></span>|<span data-ttu-id="096cc-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="096cc-156">DateTimeOffset</span></span>|<span data-ttu-id="096cc-157">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="096cc-157">The date and time the device management script was last modified.</span></span> <span data-ttu-id="096cc-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="096cc-158">This property is read-only.</span></span>|
|<span data-ttu-id="096cc-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="096cc-159">runAsAccount</span></span>|[<span data-ttu-id="096cc-160">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="096cc-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="096cc-161">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="096cc-161">Indicates the type of execution context.</span></span> <span data-ttu-id="096cc-162">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="096cc-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="096cc-163">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="096cc-163">enforceSignatureCheck</span></span>|<span data-ttu-id="096cc-164">Логический</span><span class="sxs-lookup"><span data-stu-id="096cc-164">Boolean</span></span>|<span data-ttu-id="096cc-165">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="096cc-165">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="096cc-166">fileName</span><span class="sxs-lookup"><span data-stu-id="096cc-166">fileName</span></span>|<span data-ttu-id="096cc-167">String</span><span class="sxs-lookup"><span data-stu-id="096cc-167">String</span></span>|<span data-ttu-id="096cc-168">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="096cc-168">Script file name.</span></span>|
|<span data-ttu-id="096cc-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="096cc-169">roleScopeTagIds</span></span>|<span data-ttu-id="096cc-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="096cc-170">String collection</span></span>|<span data-ttu-id="096cc-171">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="096cc-171">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="096cc-172">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="096cc-172">runAs32Bit</span></span>|<span data-ttu-id="096cc-173">Логический</span><span class="sxs-lookup"><span data-stu-id="096cc-173">Boolean</span></span>|<span data-ttu-id="096cc-174">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="096cc-174">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="096cc-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="096cc-175">Response</span></span>
<span data-ttu-id="096cc-176">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="096cc-176">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="096cc-177">Пример</span><span class="sxs-lookup"><span data-stu-id="096cc-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="096cc-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="096cc-178">Request</span></span>
<span data-ttu-id="096cc-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="096cc-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
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

### <a name="response"></a><span data-ttu-id="096cc-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="096cc-180">Response</span></span>
<span data-ttu-id="096cc-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="096cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






