---
title: Обновление устройстваHealthScript
description: Обновление свойств объекта deviceHealthScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a3eb34d13008c4dcf572f3418928215ea435761
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146281"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="c13d7-103">Обновление устройстваHealthScript</span><span class="sxs-lookup"><span data-stu-id="c13d7-103">Update deviceHealthScript</span></span>

<span data-ttu-id="c13d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c13d7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c13d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c13d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c13d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c13d7-107">Обновление свойств объекта [deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="c13d7-107">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c13d7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c13d7-108">Prerequisites</span></span>
<span data-ttu-id="c13d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c13d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c13d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c13d7-111">Permission type</span></span>|<span data-ttu-id="c13d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c13d7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c13d7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c13d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c13d7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13d7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c13d7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c13d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c13d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c13d7-116">Not supported.</span></span>|
|<span data-ttu-id="c13d7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c13d7-117">Application</span></span>|<span data-ttu-id="c13d7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13d7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c13d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c13d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="c13d7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c13d7-120">Request headers</span></span>
|<span data-ttu-id="c13d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c13d7-121">Header</span></span>|<span data-ttu-id="c13d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c13d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c13d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c13d7-123">Authorization</span></span>|<span data-ttu-id="c13d7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c13d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c13d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c13d7-125">Accept</span></span>|<span data-ttu-id="c13d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c13d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c13d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c13d7-127">Request body</span></span>
<span data-ttu-id="c13d7-128">В теле запроса поставляем представление JSON для [объекта deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="c13d7-128">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="c13d7-129">В следующей таблице показаны свойства, необходимые при создании [устройстваHealthScript.](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="c13d7-129">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="c13d7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c13d7-130">Property</span></span>|<span data-ttu-id="c13d7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c13d7-131">Type</span></span>|<span data-ttu-id="c13d7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c13d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c13d7-133">id</span><span class="sxs-lookup"><span data-stu-id="c13d7-133">id</span></span>|<span data-ttu-id="c13d7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c13d7-134">String</span></span>|<span data-ttu-id="c13d7-135">Уникальный идентификатор для скрипта здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="c13d7-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="c13d7-136">publisher</span><span class="sxs-lookup"><span data-stu-id="c13d7-136">publisher</span></span>|<span data-ttu-id="c13d7-137">String</span><span class="sxs-lookup"><span data-stu-id="c13d7-137">String</span></span>|<span data-ttu-id="c13d7-138">Имя издателя скриптов для здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="c13d7-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="c13d7-139">version</span><span class="sxs-lookup"><span data-stu-id="c13d7-139">version</span></span>|<span data-ttu-id="c13d7-140">String</span><span class="sxs-lookup"><span data-stu-id="c13d7-140">String</span></span>|<span data-ttu-id="c13d7-141">Версия сценария состояния устройства</span><span class="sxs-lookup"><span data-stu-id="c13d7-141">Version of the device health script</span></span>|
|<span data-ttu-id="c13d7-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c13d7-142">displayName</span></span>|<span data-ttu-id="c13d7-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c13d7-143">String</span></span>|<span data-ttu-id="c13d7-144">Имя сценария состояния устройства</span><span class="sxs-lookup"><span data-stu-id="c13d7-144">Name of the device health script</span></span>|
|<span data-ttu-id="c13d7-145">description</span><span class="sxs-lookup"><span data-stu-id="c13d7-145">description</span></span>|<span data-ttu-id="c13d7-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c13d7-146">String</span></span>|<span data-ttu-id="c13d7-147">Описание сценария состояния устройства</span><span class="sxs-lookup"><span data-stu-id="c13d7-147">Description of the device health script</span></span>|
|<span data-ttu-id="c13d7-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="c13d7-148">detectionScriptContent</span></span>|<span data-ttu-id="c13d7-149">Binary</span><span class="sxs-lookup"><span data-stu-id="c13d7-149">Binary</span></span>|<span data-ttu-id="c13d7-150">Все содержимое сценария powershell обнаружения</span><span class="sxs-lookup"><span data-stu-id="c13d7-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="c13d7-151">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="c13d7-151">remediationScriptContent</span></span>|<span data-ttu-id="c13d7-152">Binary</span><span class="sxs-lookup"><span data-stu-id="c13d7-152">Binary</span></span>|<span data-ttu-id="c13d7-153">Все содержимое сценария powershell исправлений</span><span class="sxs-lookup"><span data-stu-id="c13d7-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="c13d7-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c13d7-154">createdDateTime</span></span>|<span data-ttu-id="c13d7-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c13d7-155">DateTimeOffset</span></span>|<span data-ttu-id="c13d7-156">Время создания скрипта здоровья устройства.</span><span class="sxs-lookup"><span data-stu-id="c13d7-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="c13d7-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c13d7-157">This property is read-only.</span></span>|
|<span data-ttu-id="c13d7-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c13d7-158">lastModifiedDateTime</span></span>|<span data-ttu-id="c13d7-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c13d7-159">DateTimeOffset</span></span>|<span data-ttu-id="c13d7-160">Время изменения скрипта здоровья устройства.</span><span class="sxs-lookup"><span data-stu-id="c13d7-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="c13d7-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c13d7-161">This property is read-only.</span></span>|
|<span data-ttu-id="c13d7-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c13d7-162">runAsAccount</span></span>|[<span data-ttu-id="c13d7-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c13d7-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c13d7-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="c13d7-164">Indicates the type of execution context.</span></span> <span data-ttu-id="c13d7-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c13d7-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c13d7-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="c13d7-166">enforceSignatureCheck</span></span>|<span data-ttu-id="c13d7-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c13d7-167">Boolean</span></span>|<span data-ttu-id="c13d7-168">Указать, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="c13d7-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="c13d7-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="c13d7-169">runAs32Bit</span></span>|<span data-ttu-id="c13d7-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="c13d7-170">Boolean</span></span>|<span data-ttu-id="c13d7-171">Указать, должен ли сценарий PowerShell работать как 32-битный</span><span class="sxs-lookup"><span data-stu-id="c13d7-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="c13d7-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c13d7-172">roleScopeTagIds</span></span>|<span data-ttu-id="c13d7-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c13d7-173">String collection</span></span>|<span data-ttu-id="c13d7-174">Список ID-тегов области для скрипта здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="c13d7-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="c13d7-175">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="c13d7-175">isGlobalScript</span></span>|<span data-ttu-id="c13d7-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="c13d7-176">Boolean</span></span>|<span data-ttu-id="c13d7-177">Определяет, является ли это microsoft Proprietary Script.</span><span class="sxs-lookup"><span data-stu-id="c13d7-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="c13d7-178">Несвободные скрипты являются только для чтения</span><span class="sxs-lookup"><span data-stu-id="c13d7-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="c13d7-179">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="c13d7-179">highestAvailableVersion</span></span>|<span data-ttu-id="c13d7-180">Строка</span><span class="sxs-lookup"><span data-stu-id="c13d7-180">String</span></span>|<span data-ttu-id="c13d7-181">Самая доступная версия для сценария Microsoft Proprietary</span><span class="sxs-lookup"><span data-stu-id="c13d7-181">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="c13d7-182">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="c13d7-182">detectionScriptParameters</span></span>|<span data-ttu-id="c13d7-183">[коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="c13d7-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="c13d7-184">Список объектов ComplexType DetectionScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="c13d7-184">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="c13d7-185">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="c13d7-185">remediationScriptParameters</span></span>|<span data-ttu-id="c13d7-186">[коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="c13d7-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="c13d7-187">Список объектов ComplexType RemediationScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="c13d7-187">List of ComplexType RemediationScriptParameters objects.</span></span>|



## <a name="response"></a><span data-ttu-id="c13d7-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="c13d7-188">Response</span></span>
<span data-ttu-id="c13d7-189">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект deviceHealthScript](../resources/intune-devices-devicehealthscript.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c13d7-189">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c13d7-190">Пример</span><span class="sxs-lookup"><span data-stu-id="c13d7-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="c13d7-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="c13d7-191">Request</span></span>
<span data-ttu-id="c13d7-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c13d7-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c13d7-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="c13d7-193">Response</span></span>
<span data-ttu-id="c13d7-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c13d7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




