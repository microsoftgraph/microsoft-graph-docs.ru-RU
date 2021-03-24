---
title: Создание deviceHealthScript
description: Создайте новый объект deviceHealthScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb2fc4cde6aeffd30950e08c7a9183348388aa7b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146393"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="5424a-103">Создание deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="5424a-103">Create deviceHealthScript</span></span>

<span data-ttu-id="5424a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5424a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5424a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5424a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5424a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5424a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5424a-107">Создайте новый [объект deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="5424a-107">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5424a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5424a-108">Prerequisites</span></span>
<span data-ttu-id="5424a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5424a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5424a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5424a-111">Permission type</span></span>|<span data-ttu-id="5424a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5424a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5424a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5424a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5424a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5424a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5424a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5424a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5424a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5424a-116">Not supported.</span></span>|
|<span data-ttu-id="5424a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5424a-117">Application</span></span>|<span data-ttu-id="5424a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5424a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5424a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5424a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="5424a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5424a-120">Request headers</span></span>
|<span data-ttu-id="5424a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5424a-121">Header</span></span>|<span data-ttu-id="5424a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5424a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5424a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5424a-123">Authorization</span></span>|<span data-ttu-id="5424a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5424a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5424a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5424a-125">Accept</span></span>|<span data-ttu-id="5424a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5424a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5424a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5424a-127">Request body</span></span>
<span data-ttu-id="5424a-128">В теле запроса поставляем представление JSON для объекта deviceHealthScript.</span><span class="sxs-lookup"><span data-stu-id="5424a-128">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="5424a-129">В следующей таблице показаны свойства, необходимые при создании устройстваHealthScript.</span><span class="sxs-lookup"><span data-stu-id="5424a-129">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="5424a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5424a-130">Property</span></span>|<span data-ttu-id="5424a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5424a-131">Type</span></span>|<span data-ttu-id="5424a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5424a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5424a-133">id</span><span class="sxs-lookup"><span data-stu-id="5424a-133">id</span></span>|<span data-ttu-id="5424a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5424a-134">String</span></span>|<span data-ttu-id="5424a-135">Уникальный идентификатор для скрипта здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="5424a-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="5424a-136">publisher</span><span class="sxs-lookup"><span data-stu-id="5424a-136">publisher</span></span>|<span data-ttu-id="5424a-137">String</span><span class="sxs-lookup"><span data-stu-id="5424a-137">String</span></span>|<span data-ttu-id="5424a-138">Имя издателя скриптов для здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="5424a-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="5424a-139">version</span><span class="sxs-lookup"><span data-stu-id="5424a-139">version</span></span>|<span data-ttu-id="5424a-140">String</span><span class="sxs-lookup"><span data-stu-id="5424a-140">String</span></span>|<span data-ttu-id="5424a-141">Версия сценария состояния устройства</span><span class="sxs-lookup"><span data-stu-id="5424a-141">Version of the device health script</span></span>|
|<span data-ttu-id="5424a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5424a-142">displayName</span></span>|<span data-ttu-id="5424a-143">Строка</span><span class="sxs-lookup"><span data-stu-id="5424a-143">String</span></span>|<span data-ttu-id="5424a-144">Имя сценария состояния устройства</span><span class="sxs-lookup"><span data-stu-id="5424a-144">Name of the device health script</span></span>|
|<span data-ttu-id="5424a-145">description</span><span class="sxs-lookup"><span data-stu-id="5424a-145">description</span></span>|<span data-ttu-id="5424a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="5424a-146">String</span></span>|<span data-ttu-id="5424a-147">Описание сценария состояния устройства</span><span class="sxs-lookup"><span data-stu-id="5424a-147">Description of the device health script</span></span>|
|<span data-ttu-id="5424a-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="5424a-148">detectionScriptContent</span></span>|<span data-ttu-id="5424a-149">Binary</span><span class="sxs-lookup"><span data-stu-id="5424a-149">Binary</span></span>|<span data-ttu-id="5424a-150">Все содержимое сценария powershell обнаружения</span><span class="sxs-lookup"><span data-stu-id="5424a-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="5424a-151">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="5424a-151">remediationScriptContent</span></span>|<span data-ttu-id="5424a-152">Binary</span><span class="sxs-lookup"><span data-stu-id="5424a-152">Binary</span></span>|<span data-ttu-id="5424a-153">Все содержимое сценария powershell исправлений</span><span class="sxs-lookup"><span data-stu-id="5424a-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="5424a-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5424a-154">createdDateTime</span></span>|<span data-ttu-id="5424a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5424a-155">DateTimeOffset</span></span>|<span data-ttu-id="5424a-156">Время создания скрипта здоровья устройства.</span><span class="sxs-lookup"><span data-stu-id="5424a-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="5424a-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5424a-157">This property is read-only.</span></span>|
|<span data-ttu-id="5424a-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5424a-158">lastModifiedDateTime</span></span>|<span data-ttu-id="5424a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5424a-159">DateTimeOffset</span></span>|<span data-ttu-id="5424a-160">Время изменения скрипта здоровья устройства.</span><span class="sxs-lookup"><span data-stu-id="5424a-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="5424a-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5424a-161">This property is read-only.</span></span>|
|<span data-ttu-id="5424a-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="5424a-162">runAsAccount</span></span>|[<span data-ttu-id="5424a-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="5424a-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="5424a-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="5424a-164">Indicates the type of execution context.</span></span> <span data-ttu-id="5424a-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="5424a-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="5424a-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="5424a-166">enforceSignatureCheck</span></span>|<span data-ttu-id="5424a-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="5424a-167">Boolean</span></span>|<span data-ttu-id="5424a-168">Указать, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="5424a-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="5424a-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="5424a-169">runAs32Bit</span></span>|<span data-ttu-id="5424a-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="5424a-170">Boolean</span></span>|<span data-ttu-id="5424a-171">Указать, должен ли сценарий PowerShell работать как 32-битный</span><span class="sxs-lookup"><span data-stu-id="5424a-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="5424a-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5424a-172">roleScopeTagIds</span></span>|<span data-ttu-id="5424a-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5424a-173">String collection</span></span>|<span data-ttu-id="5424a-174">Список ID-тегов области для скрипта здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="5424a-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="5424a-175">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="5424a-175">isGlobalScript</span></span>|<span data-ttu-id="5424a-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="5424a-176">Boolean</span></span>|<span data-ttu-id="5424a-177">Определяет, является ли это microsoft Proprietary Script.</span><span class="sxs-lookup"><span data-stu-id="5424a-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="5424a-178">Несвободные скрипты являются только для чтения</span><span class="sxs-lookup"><span data-stu-id="5424a-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="5424a-179">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="5424a-179">highestAvailableVersion</span></span>|<span data-ttu-id="5424a-180">Строка</span><span class="sxs-lookup"><span data-stu-id="5424a-180">String</span></span>|<span data-ttu-id="5424a-181">Самая доступная версия для сценария Microsoft Proprietary</span><span class="sxs-lookup"><span data-stu-id="5424a-181">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="5424a-182">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="5424a-182">detectionScriptParameters</span></span>|<span data-ttu-id="5424a-183">[коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="5424a-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="5424a-184">Список объектов ComplexType DetectionScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="5424a-184">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="5424a-185">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="5424a-185">remediationScriptParameters</span></span>|<span data-ttu-id="5424a-186">[коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="5424a-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="5424a-187">Список объектов ComplexType RemediationScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="5424a-187">List of ComplexType RemediationScriptParameters objects.</span></span>|



## <a name="response"></a><span data-ttu-id="5424a-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="5424a-188">Response</span></span>
<span data-ttu-id="5424a-189">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект deviceHealthScript](../resources/intune-devices-devicehealthscript.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5424a-189">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5424a-190">Пример</span><span class="sxs-lookup"><span data-stu-id="5424a-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="5424a-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="5424a-191">Request</span></span>
<span data-ttu-id="5424a-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5424a-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5424a-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="5424a-193">Response</span></span>
<span data-ttu-id="5424a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5424a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




