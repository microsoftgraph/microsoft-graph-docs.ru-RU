---
title: Создание Девицехеалсскрипт
description: Создание нового объекта Девицехеалсскрипт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5638b7ac4452531e4da173dd3bab53a42ce7e339
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763538"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="385fc-103">Создание Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="385fc-103">Create deviceHealthScript</span></span>

> <span data-ttu-id="385fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="385fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="385fc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="385fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="385fc-106">Создание нового объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="385fc-106">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="385fc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="385fc-107">Prerequisites</span></span>
<span data-ttu-id="385fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="385fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="385fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="385fc-110">Permission type</span></span>|<span data-ttu-id="385fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="385fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="385fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="385fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="385fc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="385fc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="385fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="385fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="385fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="385fc-115">Not supported.</span></span>|
|<span data-ttu-id="385fc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="385fc-116">Application</span></span>|<span data-ttu-id="385fc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="385fc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="385fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="385fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="385fc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="385fc-119">Request headers</span></span>
|<span data-ttu-id="385fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="385fc-120">Header</span></span>|<span data-ttu-id="385fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="385fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="385fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="385fc-122">Authorization</span></span>|<span data-ttu-id="385fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="385fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="385fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="385fc-124">Accept</span></span>|<span data-ttu-id="385fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="385fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="385fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="385fc-126">Request body</span></span>
<span data-ttu-id="385fc-127">В тексте запроса добавьте представление объекта Девицехеалсскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="385fc-127">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="385fc-128">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскрипт.</span><span class="sxs-lookup"><span data-stu-id="385fc-128">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="385fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="385fc-129">Property</span></span>|<span data-ttu-id="385fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="385fc-130">Type</span></span>|<span data-ttu-id="385fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="385fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="385fc-132">id</span><span class="sxs-lookup"><span data-stu-id="385fc-132">id</span></span>|<span data-ttu-id="385fc-133">String</span><span class="sxs-lookup"><span data-stu-id="385fc-133">String</span></span>|<span data-ttu-id="385fc-134">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="385fc-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="385fc-135">publisher</span><span class="sxs-lookup"><span data-stu-id="385fc-135">publisher</span></span>|<span data-ttu-id="385fc-136">String</span><span class="sxs-lookup"><span data-stu-id="385fc-136">String</span></span>|<span data-ttu-id="385fc-137">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="385fc-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="385fc-138">version</span><span class="sxs-lookup"><span data-stu-id="385fc-138">version</span></span>|<span data-ttu-id="385fc-139">String</span><span class="sxs-lookup"><span data-stu-id="385fc-139">String</span></span>|<span data-ttu-id="385fc-140">Версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="385fc-140">Version of the device health script</span></span>|
|<span data-ttu-id="385fc-141">displayName</span><span class="sxs-lookup"><span data-stu-id="385fc-141">displayName</span></span>|<span data-ttu-id="385fc-142">Строка</span><span class="sxs-lookup"><span data-stu-id="385fc-142">String</span></span>|<span data-ttu-id="385fc-143">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="385fc-143">Name of the device health script</span></span>|
|<span data-ttu-id="385fc-144">description</span><span class="sxs-lookup"><span data-stu-id="385fc-144">description</span></span>|<span data-ttu-id="385fc-145">String</span><span class="sxs-lookup"><span data-stu-id="385fc-145">String</span></span>|<span data-ttu-id="385fc-146">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="385fc-146">Description of the device health script</span></span>|
|<span data-ttu-id="385fc-147">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="385fc-147">detectionScriptContent</span></span>|<span data-ttu-id="385fc-148">Binary</span><span class="sxs-lookup"><span data-stu-id="385fc-148">Binary</span></span>|<span data-ttu-id="385fc-149">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="385fc-149">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="385fc-150">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="385fc-150">remediationScriptContent</span></span>|<span data-ttu-id="385fc-151">Binary</span><span class="sxs-lookup"><span data-stu-id="385fc-151">Binary</span></span>|<span data-ttu-id="385fc-152">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="385fc-152">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="385fc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="385fc-153">createdDateTime</span></span>|<span data-ttu-id="385fc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="385fc-154">DateTimeOffset</span></span>|<span data-ttu-id="385fc-155">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="385fc-155">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="385fc-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="385fc-156">This property is read-only.</span></span>|
|<span data-ttu-id="385fc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="385fc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="385fc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="385fc-158">DateTimeOffset</span></span>|<span data-ttu-id="385fc-159">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="385fc-159">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="385fc-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="385fc-160">This property is read-only.</span></span>|
|<span data-ttu-id="385fc-161">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="385fc-161">runAsAccount</span></span>|[<span data-ttu-id="385fc-162">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="385fc-162">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="385fc-163">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="385fc-163">Indicates the type of execution context.</span></span> <span data-ttu-id="385fc-164">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="385fc-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="385fc-165">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="385fc-165">enforceSignatureCheck</span></span>|<span data-ttu-id="385fc-166">Логический</span><span class="sxs-lookup"><span data-stu-id="385fc-166">Boolean</span></span>|<span data-ttu-id="385fc-167">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="385fc-167">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="385fc-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="385fc-168">runAs32Bit</span></span>|<span data-ttu-id="385fc-169">Логический</span><span class="sxs-lookup"><span data-stu-id="385fc-169">Boolean</span></span>|<span data-ttu-id="385fc-170">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="385fc-170">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="385fc-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="385fc-171">roleScopeTagIds</span></span>|<span data-ttu-id="385fc-172">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="385fc-172">String collection</span></span>|<span data-ttu-id="385fc-173">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="385fc-173">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="385fc-174">исглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="385fc-174">isGlobalScript</span></span>|<span data-ttu-id="385fc-175">Логический</span><span class="sxs-lookup"><span data-stu-id="385fc-175">Boolean</span></span>|<span data-ttu-id="385fc-176">Определяет, является ли этот сценарий фирменным (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="385fc-176">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="385fc-177">Специальные сценарии доступны только для чтения</span><span class="sxs-lookup"><span data-stu-id="385fc-177">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="385fc-178">хигхеставаилаблеверсион</span><span class="sxs-lookup"><span data-stu-id="385fc-178">highestAvailableVersion</span></span>|<span data-ttu-id="385fc-179">String</span><span class="sxs-lookup"><span data-stu-id="385fc-179">String</span></span>|<span data-ttu-id="385fc-180">Самая высокая доступная версия для собственного сценария Майкрософт</span><span class="sxs-lookup"><span data-stu-id="385fc-180">Highest available version for a Microsoft Proprietary script</span></span>|



## <a name="response"></a><span data-ttu-id="385fc-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="385fc-181">Response</span></span>
<span data-ttu-id="385fc-182">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="385fc-182">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="385fc-183">Пример</span><span class="sxs-lookup"><span data-stu-id="385fc-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="385fc-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="385fc-184">Request</span></span>
<span data-ttu-id="385fc-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="385fc-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
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

### <a name="response"></a><span data-ttu-id="385fc-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="385fc-186">Response</span></span>
<span data-ttu-id="385fc-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="385fc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




