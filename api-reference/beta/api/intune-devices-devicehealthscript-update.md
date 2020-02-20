---
title: Обновление Девицехеалсскрипт
description: Обновление свойств объекта Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1aab6b8bacba8175138beffeb6b5afc9108fd64b
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162192"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="8fefd-103">Обновление Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="8fefd-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="8fefd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fefd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fefd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fefd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fefd-106">Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="8fefd-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fefd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8fefd-107">Prerequisites</span></span>
<span data-ttu-id="8fefd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fefd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fefd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fefd-110">Permission type</span></span>|<span data-ttu-id="8fefd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fefd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fefd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fefd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8fefd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fefd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8fefd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fefd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fefd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fefd-115">Not supported.</span></span>|
|<span data-ttu-id="8fefd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fefd-116">Application</span></span>|<span data-ttu-id="8fefd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fefd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fefd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fefd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="8fefd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8fefd-119">Request headers</span></span>
|<span data-ttu-id="8fefd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fefd-120">Header</span></span>|<span data-ttu-id="8fefd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8fefd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fefd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fefd-122">Authorization</span></span>|<span data-ttu-id="8fefd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fefd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fefd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8fefd-124">Accept</span></span>|<span data-ttu-id="8fefd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8fefd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fefd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fefd-126">Request body</span></span>
<span data-ttu-id="8fefd-127">В тексте запроса добавьте представление объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fefd-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="8fefd-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="8fefd-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="8fefd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fefd-129">Property</span></span>|<span data-ttu-id="8fefd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8fefd-130">Type</span></span>|<span data-ttu-id="8fefd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8fefd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fefd-132">id</span><span class="sxs-lookup"><span data-stu-id="8fefd-132">id</span></span>|<span data-ttu-id="8fefd-133">String</span><span class="sxs-lookup"><span data-stu-id="8fefd-133">String</span></span>|<span data-ttu-id="8fefd-134">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="8fefd-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="8fefd-135">publisher</span><span class="sxs-lookup"><span data-stu-id="8fefd-135">publisher</span></span>|<span data-ttu-id="8fefd-136">String</span><span class="sxs-lookup"><span data-stu-id="8fefd-136">String</span></span>|<span data-ttu-id="8fefd-137">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="8fefd-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="8fefd-138">version</span><span class="sxs-lookup"><span data-stu-id="8fefd-138">version</span></span>|<span data-ttu-id="8fefd-139">String</span><span class="sxs-lookup"><span data-stu-id="8fefd-139">String</span></span>|<span data-ttu-id="8fefd-140">Версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="8fefd-140">Version of the device health script</span></span>|
|<span data-ttu-id="8fefd-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8fefd-141">displayName</span></span>|<span data-ttu-id="8fefd-142">Строка</span><span class="sxs-lookup"><span data-stu-id="8fefd-142">String</span></span>|<span data-ttu-id="8fefd-143">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="8fefd-143">Name of the device health script</span></span>|
|<span data-ttu-id="8fefd-144">description</span><span class="sxs-lookup"><span data-stu-id="8fefd-144">description</span></span>|<span data-ttu-id="8fefd-145">String</span><span class="sxs-lookup"><span data-stu-id="8fefd-145">String</span></span>|<span data-ttu-id="8fefd-146">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="8fefd-146">Description of the device health script</span></span>|
|<span data-ttu-id="8fefd-147">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="8fefd-147">detectionScriptContent</span></span>|<span data-ttu-id="8fefd-148">Binary</span><span class="sxs-lookup"><span data-stu-id="8fefd-148">Binary</span></span>|<span data-ttu-id="8fefd-149">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="8fefd-149">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="8fefd-150">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="8fefd-150">remediationScriptContent</span></span>|<span data-ttu-id="8fefd-151">Binary</span><span class="sxs-lookup"><span data-stu-id="8fefd-151">Binary</span></span>|<span data-ttu-id="8fefd-152">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="8fefd-152">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="8fefd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fefd-153">createdDateTime</span></span>|<span data-ttu-id="8fefd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fefd-154">DateTimeOffset</span></span>|<span data-ttu-id="8fefd-155">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="8fefd-155">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="8fefd-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fefd-156">This property is read-only.</span></span>|
|<span data-ttu-id="8fefd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fefd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8fefd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fefd-158">DateTimeOffset</span></span>|<span data-ttu-id="8fefd-159">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="8fefd-159">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="8fefd-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fefd-160">This property is read-only.</span></span>|
|<span data-ttu-id="8fefd-161">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="8fefd-161">runAsAccount</span></span>|[<span data-ttu-id="8fefd-162">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="8fefd-162">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="8fefd-163">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="8fefd-163">Indicates the type of execution context.</span></span> <span data-ttu-id="8fefd-164">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8fefd-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="8fefd-165">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="8fefd-165">enforceSignatureCheck</span></span>|<span data-ttu-id="8fefd-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fefd-166">Boolean</span></span>|<span data-ttu-id="8fefd-167">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="8fefd-167">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="8fefd-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="8fefd-168">runAs32Bit</span></span>|<span data-ttu-id="8fefd-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fefd-169">Boolean</span></span>|<span data-ttu-id="8fefd-170">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="8fefd-170">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="8fefd-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8fefd-171">roleScopeTagIds</span></span>|<span data-ttu-id="8fefd-172">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8fefd-172">String collection</span></span>|<span data-ttu-id="8fefd-173">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="8fefd-173">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="8fefd-174">исглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="8fefd-174">isGlobalScript</span></span>|<span data-ttu-id="8fefd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fefd-175">Boolean</span></span>|<span data-ttu-id="8fefd-176">Определяет, является ли этот сценарий фирменным (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="8fefd-176">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="8fefd-177">Специальные сценарии доступны только для чтения</span><span class="sxs-lookup"><span data-stu-id="8fefd-177">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="8fefd-178">хигхеставаилаблеверсион</span><span class="sxs-lookup"><span data-stu-id="8fefd-178">highestAvailableVersion</span></span>|<span data-ttu-id="8fefd-179">String</span><span class="sxs-lookup"><span data-stu-id="8fefd-179">String</span></span>|<span data-ttu-id="8fefd-180">Самая высокая доступная версия для собственного сценария Майкрософт</span><span class="sxs-lookup"><span data-stu-id="8fefd-180">Highest available version for a Microsoft Proprietary script</span></span>|



## <a name="response"></a><span data-ttu-id="8fefd-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fefd-181">Response</span></span>
<span data-ttu-id="8fefd-182">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fefd-182">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fefd-183">Пример</span><span class="sxs-lookup"><span data-stu-id="8fefd-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fefd-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fefd-184">Request</span></span>
<span data-ttu-id="8fefd-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fefd-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8fefd-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fefd-186">Response</span></span>
<span data-ttu-id="8fefd-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fefd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





