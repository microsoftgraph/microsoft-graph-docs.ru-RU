---
title: Создание Девицехеалсскрипт
description: Создание нового объекта Девицехеалсскрипт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11e4e48f1224d7fd91c9372bfdd2e9c8e8c475a3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177074"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="21bdf-103">Создание Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="21bdf-103">Create deviceHealthScript</span></span>

<span data-ttu-id="21bdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21bdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21bdf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bdf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21bdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bdf-107">Создание нового объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="21bdf-107">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21bdf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21bdf-108">Prerequisites</span></span>
<span data-ttu-id="21bdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21bdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21bdf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21bdf-111">Permission type</span></span>|<span data-ttu-id="21bdf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21bdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21bdf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21bdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21bdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21bdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21bdf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21bdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21bdf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bdf-116">Not supported.</span></span>|
|<span data-ttu-id="21bdf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21bdf-117">Application</span></span>|<span data-ttu-id="21bdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21bdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21bdf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21bdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="21bdf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="21bdf-120">Request headers</span></span>
|<span data-ttu-id="21bdf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21bdf-121">Header</span></span>|<span data-ttu-id="21bdf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21bdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21bdf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21bdf-123">Authorization</span></span>|<span data-ttu-id="21bdf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21bdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21bdf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21bdf-125">Accept</span></span>|<span data-ttu-id="21bdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21bdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21bdf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21bdf-127">Request body</span></span>
<span data-ttu-id="21bdf-128">В тексте запроса добавьте представление объекта Девицехеалсскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21bdf-128">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="21bdf-129">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскрипт.</span><span class="sxs-lookup"><span data-stu-id="21bdf-129">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="21bdf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="21bdf-130">Property</span></span>|<span data-ttu-id="21bdf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="21bdf-131">Type</span></span>|<span data-ttu-id="21bdf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="21bdf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bdf-133">id</span><span class="sxs-lookup"><span data-stu-id="21bdf-133">id</span></span>|<span data-ttu-id="21bdf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="21bdf-134">String</span></span>|<span data-ttu-id="21bdf-135">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="21bdf-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="21bdf-136">publisher</span><span class="sxs-lookup"><span data-stu-id="21bdf-136">publisher</span></span>|<span data-ttu-id="21bdf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="21bdf-137">String</span></span>|<span data-ttu-id="21bdf-138">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="21bdf-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="21bdf-139">version</span><span class="sxs-lookup"><span data-stu-id="21bdf-139">version</span></span>|<span data-ttu-id="21bdf-140">String</span><span class="sxs-lookup"><span data-stu-id="21bdf-140">String</span></span>|<span data-ttu-id="21bdf-141">Версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="21bdf-141">Version of the device health script</span></span>|
|<span data-ttu-id="21bdf-142">displayName</span><span class="sxs-lookup"><span data-stu-id="21bdf-142">displayName</span></span>|<span data-ttu-id="21bdf-143">Строка</span><span class="sxs-lookup"><span data-stu-id="21bdf-143">String</span></span>|<span data-ttu-id="21bdf-144">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="21bdf-144">Name of the device health script</span></span>|
|<span data-ttu-id="21bdf-145">description</span><span class="sxs-lookup"><span data-stu-id="21bdf-145">description</span></span>|<span data-ttu-id="21bdf-146">String</span><span class="sxs-lookup"><span data-stu-id="21bdf-146">String</span></span>|<span data-ttu-id="21bdf-147">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="21bdf-147">Description of the device health script</span></span>|
|<span data-ttu-id="21bdf-148">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="21bdf-148">detectionScriptContent</span></span>|<span data-ttu-id="21bdf-149">Binary</span><span class="sxs-lookup"><span data-stu-id="21bdf-149">Binary</span></span>|<span data-ttu-id="21bdf-150">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="21bdf-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="21bdf-151">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="21bdf-151">remediationScriptContent</span></span>|<span data-ttu-id="21bdf-152">Binary</span><span class="sxs-lookup"><span data-stu-id="21bdf-152">Binary</span></span>|<span data-ttu-id="21bdf-153">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="21bdf-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="21bdf-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21bdf-154">createdDateTime</span></span>|<span data-ttu-id="21bdf-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21bdf-155">DateTimeOffset</span></span>|<span data-ttu-id="21bdf-156">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="21bdf-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="21bdf-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21bdf-157">This property is read-only.</span></span>|
|<span data-ttu-id="21bdf-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21bdf-158">lastModifiedDateTime</span></span>|<span data-ttu-id="21bdf-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21bdf-159">DateTimeOffset</span></span>|<span data-ttu-id="21bdf-160">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="21bdf-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="21bdf-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21bdf-161">This property is read-only.</span></span>|
|<span data-ttu-id="21bdf-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="21bdf-162">runAsAccount</span></span>|[<span data-ttu-id="21bdf-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="21bdf-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="21bdf-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="21bdf-164">Indicates the type of execution context.</span></span> <span data-ttu-id="21bdf-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="21bdf-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="21bdf-166">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="21bdf-166">enforceSignatureCheck</span></span>|<span data-ttu-id="21bdf-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="21bdf-167">Boolean</span></span>|<span data-ttu-id="21bdf-168">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="21bdf-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="21bdf-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="21bdf-169">runAs32Bit</span></span>|<span data-ttu-id="21bdf-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="21bdf-170">Boolean</span></span>|<span data-ttu-id="21bdf-171">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="21bdf-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="21bdf-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21bdf-172">roleScopeTagIds</span></span>|<span data-ttu-id="21bdf-173">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="21bdf-173">String collection</span></span>|<span data-ttu-id="21bdf-174">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="21bdf-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="21bdf-175">исглобалскрипт</span><span class="sxs-lookup"><span data-stu-id="21bdf-175">isGlobalScript</span></span>|<span data-ttu-id="21bdf-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="21bdf-176">Boolean</span></span>|<span data-ttu-id="21bdf-177">Определяет, является ли этот сценарий фирменным (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="21bdf-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="21bdf-178">Специальные сценарии доступны только для чтения</span><span class="sxs-lookup"><span data-stu-id="21bdf-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="21bdf-179">хигхеставаилаблеверсион</span><span class="sxs-lookup"><span data-stu-id="21bdf-179">highestAvailableVersion</span></span>|<span data-ttu-id="21bdf-180">Строка</span><span class="sxs-lookup"><span data-stu-id="21bdf-180">String</span></span>|<span data-ttu-id="21bdf-181">Самая высокая доступная версия для собственного сценария Майкрософт</span><span class="sxs-lookup"><span data-stu-id="21bdf-181">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="21bdf-182">детектионскриптпараметерс</span><span class="sxs-lookup"><span data-stu-id="21bdf-182">detectionScriptParameters</span></span>|<span data-ttu-id="21bdf-183">Коллекция [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="21bdf-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="21bdf-184">Список объектов Детектионскриптпараметерс в ComplexType.</span><span class="sxs-lookup"><span data-stu-id="21bdf-184">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="21bdf-185">ремедиатионскриптпараметерс</span><span class="sxs-lookup"><span data-stu-id="21bdf-185">remediationScriptParameters</span></span>|<span data-ttu-id="21bdf-186">Коллекция [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="21bdf-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="21bdf-187">Список объектов Ремедиатионскриптпараметерс в ComplexType.</span><span class="sxs-lookup"><span data-stu-id="21bdf-187">List of ComplexType RemediationScriptParameters objects.</span></span>|



## <a name="response"></a><span data-ttu-id="21bdf-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="21bdf-188">Response</span></span>
<span data-ttu-id="21bdf-189">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21bdf-189">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21bdf-190">Пример</span><span class="sxs-lookup"><span data-stu-id="21bdf-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="21bdf-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="21bdf-191">Request</span></span>
<span data-ttu-id="21bdf-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21bdf-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
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

### <a name="response"></a><span data-ttu-id="21bdf-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="21bdf-193">Response</span></span>
<span data-ttu-id="21bdf-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21bdf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



