---
title: Создание securityBaselineTemplate
description: Создайте новый объект securityBaselineTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c56758ab2f1cc75149fb63aa77a83a67873d0fb7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154506"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="511dc-103">Создание securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="511dc-103">Create securityBaselineTemplate</span></span>

<span data-ttu-id="511dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="511dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="511dc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="511dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="511dc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="511dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="511dc-107">Создайте новый [объект securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-107">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="511dc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="511dc-108">Prerequisites</span></span>
<span data-ttu-id="511dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="511dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="511dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="511dc-111">Permission type</span></span>|<span data-ttu-id="511dc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="511dc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="511dc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="511dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="511dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="511dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="511dc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="511dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="511dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="511dc-116">Not supported.</span></span>|
|<span data-ttu-id="511dc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="511dc-117">Application</span></span>|<span data-ttu-id="511dc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="511dc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="511dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="511dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="511dc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="511dc-120">Request headers</span></span>
|<span data-ttu-id="511dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="511dc-121">Header</span></span>|<span data-ttu-id="511dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="511dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="511dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="511dc-123">Authorization</span></span>|<span data-ttu-id="511dc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="511dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="511dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="511dc-125">Accept</span></span>|<span data-ttu-id="511dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="511dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="511dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="511dc-127">Request body</span></span>
<span data-ttu-id="511dc-128">В теле запроса поставляем представление JSON для объекта securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="511dc-128">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="511dc-129">В следующей таблице показаны свойства, необходимые при создании securityBaselineTemplate.</span><span class="sxs-lookup"><span data-stu-id="511dc-129">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="511dc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="511dc-130">Property</span></span>|<span data-ttu-id="511dc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="511dc-131">Type</span></span>|<span data-ttu-id="511dc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="511dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="511dc-133">id</span><span class="sxs-lookup"><span data-stu-id="511dc-133">id</span></span>|<span data-ttu-id="511dc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="511dc-134">String</span></span>|<span data-ttu-id="511dc-135">ID шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="511dc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="511dc-136">displayName</span></span>|<span data-ttu-id="511dc-137">Строка</span><span class="sxs-lookup"><span data-stu-id="511dc-137">String</span></span>|<span data-ttu-id="511dc-138">Имя отображения шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="511dc-139">description</span><span class="sxs-lookup"><span data-stu-id="511dc-139">description</span></span>|<span data-ttu-id="511dc-140">Строка</span><span class="sxs-lookup"><span data-stu-id="511dc-140">String</span></span>|<span data-ttu-id="511dc-141">Описание шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="511dc-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="511dc-142">versionInfo</span></span>|<span data-ttu-id="511dc-143">Строка</span><span class="sxs-lookup"><span data-stu-id="511dc-143">String</span></span>|<span data-ttu-id="511dc-144">Сведения о версии шаблона, унаследованные от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="511dc-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="511dc-145">isDeprecated</span></span>|<span data-ttu-id="511dc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="511dc-146">Boolean</span></span>|<span data-ttu-id="511dc-147">Шаблон обесценив или нет.</span><span class="sxs-lookup"><span data-stu-id="511dc-147">The template is deprecated or not.</span></span> <span data-ttu-id="511dc-148">Намерения не могут быть созданы из шаблона с законтятой расшифровкой.</span><span class="sxs-lookup"><span data-stu-id="511dc-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="511dc-149">Унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="511dc-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="511dc-150">intentCount</span></span>|<span data-ttu-id="511dc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="511dc-151">Int32</span></span>|<span data-ttu-id="511dc-152">Количество намерений, созданных из этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="511dc-152">Number of Intents created from this template.</span></span> <span data-ttu-id="511dc-153">Унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="511dc-154">templateType</span><span class="sxs-lookup"><span data-stu-id="511dc-154">templateType</span></span>|[<span data-ttu-id="511dc-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="511dc-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="511dc-156">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="511dc-156">The template's type.</span></span> <span data-ttu-id="511dc-157">Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="511dc-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="511dc-158">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span><span class="sxs-lookup"><span data-stu-id="511dc-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="511dc-159">platformType</span><span class="sxs-lookup"><span data-stu-id="511dc-159">platformType</span></span>|[<span data-ttu-id="511dc-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="511dc-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="511dc-161">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="511dc-161">The template's platform.</span></span> <span data-ttu-id="511dc-162">Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="511dc-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="511dc-163">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="511dc-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="511dc-164">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="511dc-164">templateSubtype</span></span>|[<span data-ttu-id="511dc-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="511dc-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="511dc-166">Подтип шаблона.</span><span class="sxs-lookup"><span data-stu-id="511dc-166">The template's subtype.</span></span> <span data-ttu-id="511dc-167">Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="511dc-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="511dc-168">Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span><span class="sxs-lookup"><span data-stu-id="511dc-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="511dc-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="511dc-169">publishedDateTime</span></span>|<span data-ttu-id="511dc-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="511dc-170">DateTimeOffset</span></span>|<span data-ttu-id="511dc-171">При публикации шаблона наследуется [из deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="511dc-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="511dc-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="511dc-172">Response</span></span>
<span data-ttu-id="511dc-173">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="511dc-173">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="511dc-174">Пример</span><span class="sxs-lookup"><span data-stu-id="511dc-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="511dc-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="511dc-175">Request</span></span>
<span data-ttu-id="511dc-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="511dc-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="511dc-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="511dc-177">Response</span></span>
<span data-ttu-id="511dc-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="511dc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```




