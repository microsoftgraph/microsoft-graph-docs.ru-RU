---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9564b0946158b8313c01e6bd2df7fc02b04c9a3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178859"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="5dfee-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="5dfee-103">Create deviceManagementScript</span></span>

<span data-ttu-id="5dfee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dfee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5dfee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dfee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dfee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5dfee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dfee-107">Создание нового объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="5dfee-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dfee-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5dfee-108">Prerequisites</span></span>
<span data-ttu-id="5dfee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dfee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dfee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5dfee-111">Permission type</span></span>|<span data-ttu-id="5dfee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5dfee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dfee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5dfee-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5dfee-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5dfee-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5dfee-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dfee-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5dfee-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5dfee-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5dfee-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dfee-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5dfee-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5dfee-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dfee-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dfee-119">Not supported.</span></span>|
|<span data-ttu-id="5dfee-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5dfee-120">Application</span></span>||
| <span data-ttu-id="5dfee-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5dfee-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5dfee-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dfee-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="5dfee-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="5dfee-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5dfee-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dfee-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dfee-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5dfee-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="5dfee-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5dfee-126">Request headers</span></span>
|<span data-ttu-id="5dfee-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5dfee-127">Header</span></span>|<span data-ttu-id="5dfee-128">Значение</span><span class="sxs-lookup"><span data-stu-id="5dfee-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dfee-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5dfee-129">Authorization</span></span>|<span data-ttu-id="5dfee-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5dfee-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dfee-131">Accept</span><span class="sxs-lookup"><span data-stu-id="5dfee-131">Accept</span></span>|<span data-ttu-id="5dfee-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5dfee-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dfee-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5dfee-133">Request body</span></span>
<span data-ttu-id="5dfee-134">В тексте запроса добавьте представление объекта deviceManagementScript в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dfee-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="5dfee-135">В следующей таблице приведены свойства, необходимые при создании deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="5dfee-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="5dfee-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dfee-136">Property</span></span>|<span data-ttu-id="5dfee-137">Тип</span><span class="sxs-lookup"><span data-stu-id="5dfee-137">Type</span></span>|<span data-ttu-id="5dfee-138">Описание</span><span class="sxs-lookup"><span data-stu-id="5dfee-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dfee-139">id</span><span class="sxs-lookup"><span data-stu-id="5dfee-139">id</span></span>|<span data-ttu-id="5dfee-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5dfee-140">String</span></span>|<span data-ttu-id="5dfee-141">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5dfee-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="5dfee-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5dfee-142">displayName</span></span>|<span data-ttu-id="5dfee-143">Строка</span><span class="sxs-lookup"><span data-stu-id="5dfee-143">String</span></span>|<span data-ttu-id="5dfee-144">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5dfee-144">Name of the device management script.</span></span>|
|<span data-ttu-id="5dfee-145">description</span><span class="sxs-lookup"><span data-stu-id="5dfee-145">description</span></span>|<span data-ttu-id="5dfee-146">String</span><span class="sxs-lookup"><span data-stu-id="5dfee-146">String</span></span>|<span data-ttu-id="5dfee-147">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5dfee-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="5dfee-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfee-148">createdDateTime</span></span>|<span data-ttu-id="5dfee-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfee-149">DateTimeOffset</span></span>|<span data-ttu-id="5dfee-150">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5dfee-150">The date and time the device management script was created.</span></span> <span data-ttu-id="5dfee-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dfee-151">This property is read-only.</span></span>|
|<span data-ttu-id="5dfee-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfee-152">lastModifiedDateTime</span></span>|<span data-ttu-id="5dfee-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfee-153">DateTimeOffset</span></span>|<span data-ttu-id="5dfee-154">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="5dfee-154">The date and time the device management script was last modified.</span></span> <span data-ttu-id="5dfee-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dfee-155">This property is read-only.</span></span>|
|<span data-ttu-id="5dfee-156">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="5dfee-156">runAsAccount</span></span>|[<span data-ttu-id="5dfee-157">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="5dfee-157">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="5dfee-158">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="5dfee-158">Indicates the type of execution context.</span></span> <span data-ttu-id="5dfee-159">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="5dfee-159">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="5dfee-160">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="5dfee-160">enforceSignatureCheck</span></span>|<span data-ttu-id="5dfee-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfee-161">Boolean</span></span>|<span data-ttu-id="5dfee-162">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="5dfee-162">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="5dfee-163">fileName</span><span class="sxs-lookup"><span data-stu-id="5dfee-163">fileName</span></span>|<span data-ttu-id="5dfee-164">String</span><span class="sxs-lookup"><span data-stu-id="5dfee-164">String</span></span>|<span data-ttu-id="5dfee-165">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="5dfee-165">Script file name.</span></span>|
|<span data-ttu-id="5dfee-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5dfee-166">roleScopeTagIds</span></span>|<span data-ttu-id="5dfee-167">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5dfee-167">String collection</span></span>|<span data-ttu-id="5dfee-168">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="5dfee-168">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="5dfee-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="5dfee-169">runAs32Bit</span></span>|<span data-ttu-id="5dfee-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfee-170">Boolean</span></span>|<span data-ttu-id="5dfee-171">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="5dfee-171">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="5dfee-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="5dfee-172">Response</span></span>
<span data-ttu-id="5dfee-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5dfee-173">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dfee-174">Пример</span><span class="sxs-lookup"><span data-stu-id="5dfee-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dfee-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="5dfee-175">Request</span></span>
<span data-ttu-id="5dfee-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5dfee-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5dfee-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dfee-177">Response</span></span>
<span data-ttu-id="5dfee-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5dfee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






