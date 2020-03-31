---
title: Обновление Девицехеалсскрипт
description: Обновление свойств объекта Девицехеалсскрипт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ec2609c17259dcfb04e06aa115be0fe99e33c20
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062065"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="83a58-103">Обновление Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="83a58-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="83a58-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83a58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83a58-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83a58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83a58-106">Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="83a58-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83a58-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="83a58-107">Prerequisites</span></span>
<span data-ttu-id="83a58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83a58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83a58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83a58-110">Permission type</span></span>|<span data-ttu-id="83a58-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83a58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83a58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83a58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83a58-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="83a58-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="83a58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83a58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83a58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83a58-115">Not supported.</span></span>|
|<span data-ttu-id="83a58-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="83a58-116">Application</span></span>|<span data-ttu-id="83a58-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="83a58-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83a58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83a58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="83a58-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="83a58-119">Request headers</span></span>
|<span data-ttu-id="83a58-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83a58-120">Header</span></span>|<span data-ttu-id="83a58-121">Значение</span><span class="sxs-lookup"><span data-stu-id="83a58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83a58-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83a58-122">Authorization</span></span>|<span data-ttu-id="83a58-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83a58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83a58-124">Accept</span><span class="sxs-lookup"><span data-stu-id="83a58-124">Accept</span></span>|<span data-ttu-id="83a58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83a58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83a58-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83a58-126">Request body</span></span>
<span data-ttu-id="83a58-127">В тексте запроса добавьте представление объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83a58-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="83a58-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="83a58-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="83a58-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="83a58-129">Property</span></span>|<span data-ttu-id="83a58-130">Тип</span><span class="sxs-lookup"><span data-stu-id="83a58-130">Type</span></span>|<span data-ttu-id="83a58-131">Описание</span><span class="sxs-lookup"><span data-stu-id="83a58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83a58-132">id</span><span class="sxs-lookup"><span data-stu-id="83a58-132">id</span></span>|<span data-ttu-id="83a58-133">Строка</span><span class="sxs-lookup"><span data-stu-id="83a58-133">String</span></span>|<span data-ttu-id="83a58-134">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="83a58-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="83a58-135">publisher</span><span class="sxs-lookup"><span data-stu-id="83a58-135">publisher</span></span>|<span data-ttu-id="83a58-136">String</span><span class="sxs-lookup"><span data-stu-id="83a58-136">String</span></span>|<span data-ttu-id="83a58-137">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="83a58-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="83a58-138">displayName</span><span class="sxs-lookup"><span data-stu-id="83a58-138">displayName</span></span>|<span data-ttu-id="83a58-139">Строка</span><span class="sxs-lookup"><span data-stu-id="83a58-139">String</span></span>|<span data-ttu-id="83a58-140">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="83a58-140">Name of the device health script</span></span>|
|<span data-ttu-id="83a58-141">description</span><span class="sxs-lookup"><span data-stu-id="83a58-141">description</span></span>|<span data-ttu-id="83a58-142">String</span><span class="sxs-lookup"><span data-stu-id="83a58-142">String</span></span>|<span data-ttu-id="83a58-143">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="83a58-143">Description of the device health script</span></span>|
|<span data-ttu-id="83a58-144">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="83a58-144">detectionScriptContent</span></span>|<span data-ttu-id="83a58-145">Binary</span><span class="sxs-lookup"><span data-stu-id="83a58-145">Binary</span></span>|<span data-ttu-id="83a58-146">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="83a58-146">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="83a58-147">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="83a58-147">remediationScriptContent</span></span>|<span data-ttu-id="83a58-148">Binary</span><span class="sxs-lookup"><span data-stu-id="83a58-148">Binary</span></span>|<span data-ttu-id="83a58-149">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="83a58-149">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="83a58-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83a58-150">createdDateTime</span></span>|<span data-ttu-id="83a58-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83a58-151">DateTimeOffset</span></span>|<span data-ttu-id="83a58-152">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="83a58-152">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="83a58-153">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83a58-153">This property is read-only.</span></span>|
|<span data-ttu-id="83a58-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83a58-154">lastModifiedDateTime</span></span>|<span data-ttu-id="83a58-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83a58-155">DateTimeOffset</span></span>|<span data-ttu-id="83a58-156">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="83a58-156">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="83a58-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83a58-157">This property is read-only.</span></span>|
|<span data-ttu-id="83a58-158">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="83a58-158">runAsAccount</span></span>|[<span data-ttu-id="83a58-159">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="83a58-159">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="83a58-160">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="83a58-160">Indicates the type of execution context.</span></span> <span data-ttu-id="83a58-161">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="83a58-161">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="83a58-162">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="83a58-162">enforceSignatureCheck</span></span>|<span data-ttu-id="83a58-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="83a58-163">Boolean</span></span>|<span data-ttu-id="83a58-164">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="83a58-164">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="83a58-165">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="83a58-165">runAs32Bit</span></span>|<span data-ttu-id="83a58-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="83a58-166">Boolean</span></span>|<span data-ttu-id="83a58-167">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="83a58-167">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="83a58-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83a58-168">roleScopeTagIds</span></span>|<span data-ttu-id="83a58-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="83a58-169">String collection</span></span>|<span data-ttu-id="83a58-170">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="83a58-170">List of Scope Tag IDs for the device health script</span></span>|



## <a name="response"></a><span data-ttu-id="83a58-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="83a58-171">Response</span></span>
<span data-ttu-id="83a58-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83a58-172">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83a58-173">Пример</span><span class="sxs-lookup"><span data-stu-id="83a58-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="83a58-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="83a58-174">Request</span></span>
<span data-ttu-id="83a58-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83a58-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-type: application/json
Content-length: 575

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
 }
```

### <a name="response"></a><span data-ttu-id="83a58-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="83a58-176">Response</span></span>
<span data-ttu-id="83a58-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83a58-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 747

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
}
```




