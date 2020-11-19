---
title: Обновление Девицехеалсскрипт
description: Обновление свойств объекта Девицехеалсскрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6aac160d0f3184a3ec1ce9d84d1ba94c03a5bb56
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310806"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="cf76e-103">Обновление Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="cf76e-103">Update deviceHealthScript</span></span>

<span data-ttu-id="cf76e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf76e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf76e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf76e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf76e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf76e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf76e-107">Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="cf76e-107">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf76e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf76e-108">Prerequisites</span></span>
<span data-ttu-id="cf76e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf76e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf76e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf76e-111">Permission type</span></span>|<span data-ttu-id="cf76e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf76e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf76e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf76e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf76e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf76e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cf76e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf76e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf76e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf76e-116">Not supported.</span></span>|
|<span data-ttu-id="cf76e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf76e-117">Application</span></span>|<span data-ttu-id="cf76e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf76e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf76e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf76e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="cf76e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf76e-120">Request headers</span></span>
|<span data-ttu-id="cf76e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf76e-121">Header</span></span>|<span data-ttu-id="cf76e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf76e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf76e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf76e-123">Authorization</span></span>|<span data-ttu-id="cf76e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf76e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf76e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf76e-125">Accept</span></span>|<span data-ttu-id="cf76e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf76e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf76e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf76e-127">Request body</span></span>
<span data-ttu-id="cf76e-128">В тексте запроса добавьте представление объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf76e-128">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="cf76e-129">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="cf76e-129">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="cf76e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf76e-130">Property</span></span>|<span data-ttu-id="cf76e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf76e-131">Type</span></span>|<span data-ttu-id="cf76e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf76e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf76e-133">id</span><span class="sxs-lookup"><span data-stu-id="cf76e-133">id</span></span>|<span data-ttu-id="cf76e-134">String</span><span class="sxs-lookup"><span data-stu-id="cf76e-134">String</span></span>|<span data-ttu-id="cf76e-135">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="cf76e-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="cf76e-136">publisher</span><span class="sxs-lookup"><span data-stu-id="cf76e-136">publisher</span></span>|<span data-ttu-id="cf76e-137">String</span><span class="sxs-lookup"><span data-stu-id="cf76e-137">String</span></span>|<span data-ttu-id="cf76e-138">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="cf76e-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="cf76e-139">version</span><span class="sxs-lookup"><span data-stu-id="cf76e-139">version</span></span>|<span data-ttu-id="cf76e-140">String</span><span class="sxs-lookup"><span data-stu-id="cf76e-140">String</span></span>|<span data-ttu-id="cf76e-141">Версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="cf76e-141">Version of the device health script</span></span>|
|<span data-ttu-id="cf76e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="cf76e-142">displayName</span></span>|<span data-ttu-id="cf76e-143">String</span><span class="sxs-lookup"><span data-stu-id="cf76e-143">String</span></span>|<span data-ttu-id="cf76e-144">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="cf76e-144">Name of the device health script</span></span>|
|<span data-ttu-id="cf76e-145">description</span><span class="sxs-lookup"><span data-stu-id="cf76e-145">description</span></span>|<span data-ttu-id="cf76e-146">String</span><span class="sxs-lookup"><span data-stu-id="cf76e-146">String</span></span>|<span data-ttu-id="cf76e-147">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="cf76e-147">Description of the device health script</span></span>|
|<span data-ttu-id="cf76e-148">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="cf76e-148">detectionScriptContent</span></span>|<span data-ttu-id="cf76e-149">Binary</span><span class="sxs-lookup"><span data-stu-id="cf76e-149">Binary</span></span>|<span data-ttu-id="cf76e-150">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="cf76e-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="cf76e-151">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="cf76e-151">remediationScriptContent</span></span>|<span data-ttu-id="cf76e-152">Binary</span><span class="sxs-lookup"><span data-stu-id="cf76e-152">Binary</span></span>|<span data-ttu-id="cf76e-153">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="cf76e-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="cf76e-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf76e-154">createdDateTime</span></span>|<span data-ttu-id="cf76e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf76e-155">DateTimeOffset</span></span>|<span data-ttu-id="cf76e-156">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="cf76e-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="cf76e-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf76e-157">This property is read-only.</span></span>|
|<span data-ttu-id="cf76e-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf76e-158">lastModifiedDateTime</span></span>|<span data-ttu-id="cf76e-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf76e-159">DateTimeOffset</span></span>|<span data-ttu-id="cf76e-160">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="cf76e-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="cf76e-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf76e-161">This property is read-only.</span></span>|
|<span data-ttu-id="cf76e-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="cf76e-162">runAsAccount</span></span>|[<span data-ttu-id="cf76e-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="cf76e-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="cf76e-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="cf76e-164">Indicates the type of execution context.</span></span> <span data-ttu-id="cf76e-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="cf76e-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="cf76e-166">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="cf76e-166">enforceSignatureCheck</span></span>|<span data-ttu-id="cf76e-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf76e-167">Boolean</span></span>|<span data-ttu-id="cf76e-168">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="cf76e-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="cf76e-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="cf76e-169">runAs32Bit</span></span>|<span data-ttu-id="cf76e-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf76e-170">Boolean</span></span>|<span data-ttu-id="cf76e-171">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="cf76e-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="cf76e-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cf76e-172">roleScopeTagIds</span></span>|<span data-ttu-id="cf76e-173">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cf76e-173">String collection</span></span>|<span data-ttu-id="cf76e-174">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="cf76e-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="cf76e-175">исглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="cf76e-175">isGlobalScript</span></span>|<span data-ttu-id="cf76e-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf76e-176">Boolean</span></span>|<span data-ttu-id="cf76e-177">Определяет, является ли этот сценарий фирменным (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="cf76e-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="cf76e-178">Специальные сценарии доступны только для чтения</span><span class="sxs-lookup"><span data-stu-id="cf76e-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="cf76e-179">хигхеставаилаблеверсион</span><span class="sxs-lookup"><span data-stu-id="cf76e-179">highestAvailableVersion</span></span>|<span data-ttu-id="cf76e-180">String</span><span class="sxs-lookup"><span data-stu-id="cf76e-180">String</span></span>|<span data-ttu-id="cf76e-181">Самая высокая доступная версия для собственного сценария Майкрософт</span><span class="sxs-lookup"><span data-stu-id="cf76e-181">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="cf76e-182">детектионскриптпараметерс</span><span class="sxs-lookup"><span data-stu-id="cf76e-182">detectionScriptParameters</span></span>|<span data-ttu-id="cf76e-183">Коллекция [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="cf76e-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="cf76e-184">Список объектов Детектионскриптпараметерс в ComplexType.</span><span class="sxs-lookup"><span data-stu-id="cf76e-184">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="cf76e-185">ремедиатионскриптпараметерс</span><span class="sxs-lookup"><span data-stu-id="cf76e-185">remediationScriptParameters</span></span>|<span data-ttu-id="cf76e-186">Коллекция [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="cf76e-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="cf76e-187">Список объектов Ремедиатионскриптпараметерс в ComplexType.</span><span class="sxs-lookup"><span data-stu-id="cf76e-187">List of ComplexType RemediationScriptParameters objects.</span></span>|



## <a name="response"></a><span data-ttu-id="cf76e-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf76e-188">Response</span></span>
<span data-ttu-id="cf76e-189">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf76e-189">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf76e-190">Пример</span><span class="sxs-lookup"><span data-stu-id="cf76e-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf76e-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf76e-191">Request</span></span>
<span data-ttu-id="cf76e-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf76e-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-type: application/json
Content-length: 1221

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
  "highestAvailableVersion": "Highest Available Version value",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="cf76e-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf76e-193">Response</span></span>
<span data-ttu-id="cf76e-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf76e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1393

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
  "highestAvailableVersion": "Highest Available Version value",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ]
}
```




