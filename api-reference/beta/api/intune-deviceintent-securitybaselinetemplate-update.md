---
title: Обновление securityBaselineTemplate
description: Обновление свойств объекта securityBaselineTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d02edd088f1fd3d65ecb53293cf20ca85f9f835
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136547"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="86ccf-103">Обновление securityBaselineTemplate</span><span class="sxs-lookup"><span data-stu-id="86ccf-103">Update securityBaselineTemplate</span></span>

<span data-ttu-id="86ccf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86ccf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86ccf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ccf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86ccf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86ccf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86ccf-107">Обновление свойств объекта [securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-107">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86ccf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86ccf-108">Prerequisites</span></span>
<span data-ttu-id="86ccf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ccf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86ccf-111">Permission type</span></span>|<span data-ttu-id="86ccf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86ccf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86ccf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86ccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86ccf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ccf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86ccf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86ccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86ccf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ccf-116">Not supported.</span></span>|
|<span data-ttu-id="86ccf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="86ccf-117">Application</span></span>|<span data-ttu-id="86ccf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ccf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86ccf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86ccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="86ccf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86ccf-120">Request headers</span></span>
|<span data-ttu-id="86ccf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86ccf-121">Header</span></span>|<span data-ttu-id="86ccf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86ccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86ccf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86ccf-123">Authorization</span></span>|<span data-ttu-id="86ccf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86ccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86ccf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86ccf-125">Accept</span></span>|<span data-ttu-id="86ccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86ccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ccf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86ccf-127">Request body</span></span>
<span data-ttu-id="86ccf-128">В теле запроса поставляем представление JSON для [объекта securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-128">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="86ccf-129">В следующей таблице показаны свойства, необходимые при создании [securityBaselineTemplate.](../resources/intune-deviceintent-securitybaselinetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-129">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="86ccf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86ccf-130">Property</span></span>|<span data-ttu-id="86ccf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86ccf-131">Type</span></span>|<span data-ttu-id="86ccf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86ccf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ccf-133">id</span><span class="sxs-lookup"><span data-stu-id="86ccf-133">id</span></span>|<span data-ttu-id="86ccf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="86ccf-134">String</span></span>|<span data-ttu-id="86ccf-135">ID шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="86ccf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="86ccf-136">displayName</span></span>|<span data-ttu-id="86ccf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="86ccf-137">String</span></span>|<span data-ttu-id="86ccf-138">Имя отображения шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="86ccf-139">description</span><span class="sxs-lookup"><span data-stu-id="86ccf-139">description</span></span>|<span data-ttu-id="86ccf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="86ccf-140">String</span></span>|<span data-ttu-id="86ccf-141">Описание шаблона, унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="86ccf-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="86ccf-142">versionInfo</span></span>|<span data-ttu-id="86ccf-143">Строка</span><span class="sxs-lookup"><span data-stu-id="86ccf-143">String</span></span>|<span data-ttu-id="86ccf-144">Сведения о версии шаблона, унаследованные от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="86ccf-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="86ccf-145">isDeprecated</span></span>|<span data-ttu-id="86ccf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ccf-146">Boolean</span></span>|<span data-ttu-id="86ccf-147">Шаблон обесценив или нет.</span><span class="sxs-lookup"><span data-stu-id="86ccf-147">The template is deprecated or not.</span></span> <span data-ttu-id="86ccf-148">Намерения не могут быть созданы из шаблона с законтятой расшифровкой.</span><span class="sxs-lookup"><span data-stu-id="86ccf-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="86ccf-149">Унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="86ccf-150">intentCount</span><span class="sxs-lookup"><span data-stu-id="86ccf-150">intentCount</span></span>|<span data-ttu-id="86ccf-151">Int32</span><span class="sxs-lookup"><span data-stu-id="86ccf-151">Int32</span></span>|<span data-ttu-id="86ccf-152">Количество намерений, созданных из этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="86ccf-152">Number of Intents created from this template.</span></span> <span data-ttu-id="86ccf-153">Унаследованный от [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="86ccf-154">templateType</span><span class="sxs-lookup"><span data-stu-id="86ccf-154">templateType</span></span>|[<span data-ttu-id="86ccf-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="86ccf-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="86ccf-156">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="86ccf-156">The template's type.</span></span> <span data-ttu-id="86ccf-157">Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="86ccf-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="86ccf-158">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span><span class="sxs-lookup"><span data-stu-id="86ccf-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="86ccf-159">platformType</span><span class="sxs-lookup"><span data-stu-id="86ccf-159">platformType</span></span>|[<span data-ttu-id="86ccf-160">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="86ccf-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="86ccf-161">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="86ccf-161">The template's platform.</span></span> <span data-ttu-id="86ccf-162">Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="86ccf-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="86ccf-163">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="86ccf-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="86ccf-164">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="86ccf-164">templateSubtype</span></span>|[<span data-ttu-id="86ccf-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="86ccf-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="86ccf-166">Подтип шаблона.</span><span class="sxs-lookup"><span data-stu-id="86ccf-166">The template's subtype.</span></span> <span data-ttu-id="86ccf-167">Наследуется [от deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="86ccf-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="86ccf-168">Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span><span class="sxs-lookup"><span data-stu-id="86ccf-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="86ccf-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="86ccf-169">publishedDateTime</span></span>|<span data-ttu-id="86ccf-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ccf-170">DateTimeOffset</span></span>|<span data-ttu-id="86ccf-171">При публикации шаблона наследуется [из deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="86ccf-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="86ccf-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="86ccf-172">Response</span></span>
<span data-ttu-id="86ccf-173">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="86ccf-173">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ccf-174">Пример</span><span class="sxs-lookup"><span data-stu-id="86ccf-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="86ccf-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="86ccf-175">Request</span></span>
<span data-ttu-id="86ccf-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86ccf-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="86ccf-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="86ccf-177">Response</span></span>
<span data-ttu-id="86ccf-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86ccf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




