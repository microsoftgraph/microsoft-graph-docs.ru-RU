---
title: Создание deviceManagementConfigurationPolicyTemplate
description: Создание нового объекта deviceManagementConfigurationPolicyTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbbcabc3d531505ef53aab117cec7e8b6e8e594f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665894"
---
# <a name="create-devicemanagementconfigurationpolicytemplate"></a><span data-ttu-id="f143d-103">Создание deviceManagementConfigurationPolicyTemplate</span><span class="sxs-lookup"><span data-stu-id="f143d-103">Create deviceManagementConfigurationPolicyTemplate</span></span>

<span data-ttu-id="f143d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f143d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f143d-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f143d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f143d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f143d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f143d-107">Создание нового [объекта deviceManagementConfigurationPolicyTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f143d-107">Create a new [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f143d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f143d-108">Prerequisites</span></span>
<span data-ttu-id="f143d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f143d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f143d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f143d-111">Permission type</span></span>|<span data-ttu-id="f143d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f143d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f143d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f143d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f143d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f143d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f143d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f143d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f143d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f143d-116">Not supported.</span></span>|
|<span data-ttu-id="f143d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f143d-117">Application</span></span>|<span data-ttu-id="f143d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f143d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f143d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f143d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicyTemplates
```

## <a name="request-headers"></a><span data-ttu-id="f143d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f143d-120">Request headers</span></span>
|<span data-ttu-id="f143d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f143d-121">Header</span></span>|<span data-ttu-id="f143d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f143d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f143d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f143d-123">Authorization</span></span>|<span data-ttu-id="f143d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f143d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f143d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f143d-125">Accept</span></span>|<span data-ttu-id="f143d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f143d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f143d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f143d-127">Request body</span></span>
<span data-ttu-id="f143d-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationPolicyTemplate.</span><span class="sxs-lookup"><span data-stu-id="f143d-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicyTemplate object.</span></span>

<span data-ttu-id="f143d-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationPolicyTemplate.</span><span class="sxs-lookup"><span data-stu-id="f143d-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicyTemplate.</span></span>

|<span data-ttu-id="f143d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f143d-130">Property</span></span>|<span data-ttu-id="f143d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f143d-131">Type</span></span>|<span data-ttu-id="f143d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f143d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f143d-133">id</span><span class="sxs-lookup"><span data-stu-id="f143d-133">id</span></span>|<span data-ttu-id="f143d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f143d-134">String</span></span>|<span data-ttu-id="f143d-135">Ключ документа шаблона, состоящего из BaseId и Version.</span><span class="sxs-lookup"><span data-stu-id="f143d-135">Key of the template document, composed of BaseId and Version.</span></span> <span data-ttu-id="f143d-136">Автоматически созданный.</span><span class="sxs-lookup"><span data-stu-id="f143d-136">Automatically generated.</span></span>|
|<span data-ttu-id="f143d-137">baseId</span><span class="sxs-lookup"><span data-stu-id="f143d-137">baseId</span></span>|<span data-ttu-id="f143d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f143d-138">String</span></span>|<span data-ttu-id="f143d-139">Идентификатор базы шаблонов</span><span class="sxs-lookup"><span data-stu-id="f143d-139">Template base identifier</span></span>|
|<span data-ttu-id="f143d-140">version</span><span class="sxs-lookup"><span data-stu-id="f143d-140">version</span></span>|<span data-ttu-id="f143d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f143d-141">Int32</span></span>|<span data-ttu-id="f143d-142">Версия шаблона.</span><span class="sxs-lookup"><span data-stu-id="f143d-142">Template version.</span></span> <span data-ttu-id="f143d-143">Допустимые значения от 1 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="f143d-143">Valid values 1 to 2147483647.</span></span> <span data-ttu-id="f143d-144">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f143d-144">This property is read-only.</span></span>|
|<span data-ttu-id="f143d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f143d-145">displayName</span></span>|<span data-ttu-id="f143d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f143d-146">String</span></span>|<span data-ttu-id="f143d-147">Имя отображения шаблона</span><span class="sxs-lookup"><span data-stu-id="f143d-147">Template display name</span></span>|
|<span data-ttu-id="f143d-148">description</span><span class="sxs-lookup"><span data-stu-id="f143d-148">description</span></span>|<span data-ttu-id="f143d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="f143d-149">String</span></span>|<span data-ttu-id="f143d-150">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="f143d-150">Template description</span></span>|
|<span data-ttu-id="f143d-151">displayVersion</span><span class="sxs-lookup"><span data-stu-id="f143d-151">displayVersion</span></span>|<span data-ttu-id="f143d-152">Строка</span><span class="sxs-lookup"><span data-stu-id="f143d-152">String</span></span>|<span data-ttu-id="f143d-153">Описание версии шаблона</span><span class="sxs-lookup"><span data-stu-id="f143d-153">Description of template version</span></span>|
|<span data-ttu-id="f143d-154">lifecycleState</span><span class="sxs-lookup"><span data-stu-id="f143d-154">lifecycleState</span></span>|[<span data-ttu-id="f143d-155">deviceManagementTemplateLifecycleState</span><span class="sxs-lookup"><span data-stu-id="f143d-155">deviceManagementTemplateLifecycleState</span></span>](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|<span data-ttu-id="f143d-156">Указать текущее состояние жизненного цикла шаблона.</span><span class="sxs-lookup"><span data-stu-id="f143d-156">Indicate current lifecycle state of template.</span></span> <span data-ttu-id="f143d-157">Возможные значения: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.</span><span class="sxs-lookup"><span data-stu-id="f143d-157">Possible values are: `invalid`, `draft`, `active`, `superseded`, `deprecated`, `retired`.</span></span>|
|<span data-ttu-id="f143d-158">платформы</span><span class="sxs-lookup"><span data-stu-id="f143d-158">platforms</span></span>|[<span data-ttu-id="f143d-159">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="f143d-159">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="f143d-160">Платформы для этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="f143d-160">Platforms for this template.</span></span> <span data-ttu-id="f143d-161">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="f143d-161">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="f143d-162">технологии</span><span class="sxs-lookup"><span data-stu-id="f143d-162">technologies</span></span>|[<span data-ttu-id="f143d-163">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="f143d-163">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="f143d-164">Технологии для этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="f143d-164">Technologies for this template.</span></span> <span data-ttu-id="f143d-165">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span><span class="sxs-lookup"><span data-stu-id="f143d-165">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="f143d-166">templateFamily</span><span class="sxs-lookup"><span data-stu-id="f143d-166">templateFamily</span></span>|[<span data-ttu-id="f143d-167">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="f143d-167">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="f143d-168">TemplateFamily для этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="f143d-168">TemplateFamily for this template.</span></span> <span data-ttu-id="f143d-169">Возможные значения: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span><span class="sxs-lookup"><span data-stu-id="f143d-169">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="f143d-170">allowUnmanagedSettings</span><span class="sxs-lookup"><span data-stu-id="f143d-170">allowUnmanagedSettings</span></span>|<span data-ttu-id="f143d-171">Логический</span><span class="sxs-lookup"><span data-stu-id="f143d-171">Boolean</span></span>|<span data-ttu-id="f143d-172">Разрешить неугодные шаблоны параметров</span><span class="sxs-lookup"><span data-stu-id="f143d-172">Allow unmanaged setting templates</span></span>|
|<span data-ttu-id="f143d-173">settingTemplateCount</span><span class="sxs-lookup"><span data-stu-id="f143d-173">settingTemplateCount</span></span>|<span data-ttu-id="f143d-174">Int32</span><span class="sxs-lookup"><span data-stu-id="f143d-174">Int32</span></span>|<span data-ttu-id="f143d-175">Количество шаблонов параметров.</span><span class="sxs-lookup"><span data-stu-id="f143d-175">Number of setting templates.</span></span> <span data-ttu-id="f143d-176">Допустимые значения от 0 до 2147483647.</span><span class="sxs-lookup"><span data-stu-id="f143d-176">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="f143d-177">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f143d-177">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="f143d-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="f143d-178">Response</span></span>
<span data-ttu-id="f143d-179">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f143d-179">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f143d-180">Пример</span><span class="sxs-lookup"><span data-stu-id="f143d-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="f143d-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="f143d-181">Request</span></span>
<span data-ttu-id="f143d-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f143d-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```

### <a name="response"></a><span data-ttu-id="f143d-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="f143d-183">Response</span></span>
<span data-ttu-id="f143d-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f143d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "macOS",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```




