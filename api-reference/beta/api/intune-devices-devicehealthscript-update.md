---
title: Обновление Девицехеалсскрипт
description: Обновление свойств объекта Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 517a3f13c1520d3967c799cffc2cd6fc8347703e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469722"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="732fc-103">Обновление Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="732fc-103">Update deviceHealthScript</span></span>

<span data-ttu-id="732fc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="732fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="732fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="732fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="732fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="732fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="732fc-107">Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="732fc-107">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="732fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="732fc-108">Prerequisites</span></span>
<span data-ttu-id="732fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="732fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="732fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="732fc-111">Permission type</span></span>|<span data-ttu-id="732fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="732fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="732fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="732fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="732fc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="732fc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="732fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="732fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="732fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="732fc-116">Not supported.</span></span>|
|<span data-ttu-id="732fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="732fc-117">Application</span></span>|<span data-ttu-id="732fc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="732fc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="732fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="732fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="732fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="732fc-120">Request headers</span></span>
|<span data-ttu-id="732fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="732fc-121">Header</span></span>|<span data-ttu-id="732fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="732fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="732fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="732fc-123">Authorization</span></span>|<span data-ttu-id="732fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="732fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="732fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="732fc-125">Accept</span></span>|<span data-ttu-id="732fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="732fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="732fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="732fc-127">Request body</span></span>
<span data-ttu-id="732fc-128">В тексте запроса добавьте представление объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="732fc-128">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="732fc-129">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="732fc-129">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="732fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="732fc-130">Property</span></span>|<span data-ttu-id="732fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="732fc-131">Type</span></span>|<span data-ttu-id="732fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="732fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="732fc-133">id</span><span class="sxs-lookup"><span data-stu-id="732fc-133">id</span></span>|<span data-ttu-id="732fc-134">String</span><span class="sxs-lookup"><span data-stu-id="732fc-134">String</span></span>|<span data-ttu-id="732fc-135">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="732fc-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="732fc-136">publisher</span><span class="sxs-lookup"><span data-stu-id="732fc-136">publisher</span></span>|<span data-ttu-id="732fc-137">String</span><span class="sxs-lookup"><span data-stu-id="732fc-137">String</span></span>|<span data-ttu-id="732fc-138">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="732fc-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="732fc-139">version</span><span class="sxs-lookup"><span data-stu-id="732fc-139">version</span></span>|<span data-ttu-id="732fc-140">String</span><span class="sxs-lookup"><span data-stu-id="732fc-140">String</span></span>|<span data-ttu-id="732fc-141">Версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="732fc-141">Version of the device health script</span></span>|
|<span data-ttu-id="732fc-142">displayName</span><span class="sxs-lookup"><span data-stu-id="732fc-142">displayName</span></span>|<span data-ttu-id="732fc-143">Строка</span><span class="sxs-lookup"><span data-stu-id="732fc-143">String</span></span>|<span data-ttu-id="732fc-144">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="732fc-144">Name of the device health script</span></span>|
|<span data-ttu-id="732fc-145">description</span><span class="sxs-lookup"><span data-stu-id="732fc-145">description</span></span>|<span data-ttu-id="732fc-146">String</span><span class="sxs-lookup"><span data-stu-id="732fc-146">String</span></span>|<span data-ttu-id="732fc-147">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="732fc-147">Description of the device health script</span></span>|
|<span data-ttu-id="732fc-148">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="732fc-148">detectionScriptContent</span></span>|<span data-ttu-id="732fc-149">Binary</span><span class="sxs-lookup"><span data-stu-id="732fc-149">Binary</span></span>|<span data-ttu-id="732fc-150">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="732fc-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="732fc-151">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="732fc-151">remediationScriptContent</span></span>|<span data-ttu-id="732fc-152">Binary</span><span class="sxs-lookup"><span data-stu-id="732fc-152">Binary</span></span>|<span data-ttu-id="732fc-153">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="732fc-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="732fc-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="732fc-154">createdDateTime</span></span>|<span data-ttu-id="732fc-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732fc-155">DateTimeOffset</span></span>|<span data-ttu-id="732fc-156">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="732fc-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="732fc-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="732fc-157">This property is read-only.</span></span>|
|<span data-ttu-id="732fc-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="732fc-158">lastModifiedDateTime</span></span>|<span data-ttu-id="732fc-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732fc-159">DateTimeOffset</span></span>|<span data-ttu-id="732fc-160">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="732fc-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="732fc-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="732fc-161">This property is read-only.</span></span>|
|<span data-ttu-id="732fc-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="732fc-162">runAsAccount</span></span>|[<span data-ttu-id="732fc-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="732fc-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="732fc-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="732fc-164">Indicates the type of execution context.</span></span> <span data-ttu-id="732fc-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="732fc-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="732fc-166">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="732fc-166">enforceSignatureCheck</span></span>|<span data-ttu-id="732fc-167">Логический</span><span class="sxs-lookup"><span data-stu-id="732fc-167">Boolean</span></span>|<span data-ttu-id="732fc-168">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="732fc-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="732fc-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="732fc-169">runAs32Bit</span></span>|<span data-ttu-id="732fc-170">Логический</span><span class="sxs-lookup"><span data-stu-id="732fc-170">Boolean</span></span>|<span data-ttu-id="732fc-171">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="732fc-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="732fc-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="732fc-172">roleScopeTagIds</span></span>|<span data-ttu-id="732fc-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="732fc-173">String collection</span></span>|<span data-ttu-id="732fc-174">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="732fc-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="732fc-175">исглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="732fc-175">isGlobalScript</span></span>|<span data-ttu-id="732fc-176">Логический</span><span class="sxs-lookup"><span data-stu-id="732fc-176">Boolean</span></span>|<span data-ttu-id="732fc-177">Определяет, является ли этот сценарий фирменным (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="732fc-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="732fc-178">Специальные сценарии доступны только для чтения</span><span class="sxs-lookup"><span data-stu-id="732fc-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="732fc-179">хигхеставаилаблеверсион</span><span class="sxs-lookup"><span data-stu-id="732fc-179">highestAvailableVersion</span></span>|<span data-ttu-id="732fc-180">String</span><span class="sxs-lookup"><span data-stu-id="732fc-180">String</span></span>|<span data-ttu-id="732fc-181">Самая высокая доступная версия для собственного сценария Майкрософт</span><span class="sxs-lookup"><span data-stu-id="732fc-181">Highest available version for a Microsoft Proprietary script</span></span>|



## <a name="response"></a><span data-ttu-id="732fc-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="732fc-182">Response</span></span>
<span data-ttu-id="732fc-183">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="732fc-183">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="732fc-184">Пример</span><span class="sxs-lookup"><span data-stu-id="732fc-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="732fc-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="732fc-185">Request</span></span>
<span data-ttu-id="732fc-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="732fc-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-type: application/json
Content-length: 575

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
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

### <a name="response"></a><span data-ttu-id="732fc-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="732fc-187">Response</span></span>
<span data-ttu-id="732fc-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="732fc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





