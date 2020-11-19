---
title: Обновление Секуритибаселинетемплате
description: Обновление свойств объекта Секуритибаселинетемплате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc810a78fe811b235006f874c3d7d87254ab720e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49282539"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="950e5-103">Обновление Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="950e5-103">Update securityBaselineTemplate</span></span>

<span data-ttu-id="950e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="950e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="950e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="950e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="950e5-107">Обновление свойств объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="950e5-107">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="950e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="950e5-108">Prerequisites</span></span>
<span data-ttu-id="950e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="950e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="950e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="950e5-111">Permission type</span></span>|<span data-ttu-id="950e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="950e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="950e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="950e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="950e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="950e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="950e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="950e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950e5-116">Not supported.</span></span>|
|<span data-ttu-id="950e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="950e5-117">Application</span></span>|<span data-ttu-id="950e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="950e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="950e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="950e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="950e5-120">Request headers</span></span>
|<span data-ttu-id="950e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="950e5-121">Header</span></span>|<span data-ttu-id="950e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="950e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="950e5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="950e5-123">Authorization</span></span>|<span data-ttu-id="950e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="950e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="950e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="950e5-125">Accept</span></span>|<span data-ttu-id="950e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="950e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="950e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="950e5-127">Request body</span></span>
<span data-ttu-id="950e5-128">В тексте запроса добавьте представление объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="950e5-128">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="950e5-129">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="950e5-129">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="950e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="950e5-130">Property</span></span>|<span data-ttu-id="950e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="950e5-131">Type</span></span>|<span data-ttu-id="950e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="950e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="950e5-133">id</span><span class="sxs-lookup"><span data-stu-id="950e5-133">id</span></span>|<span data-ttu-id="950e5-134">String</span><span class="sxs-lookup"><span data-stu-id="950e5-134">String</span></span>|<span data-ttu-id="950e5-135">Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="950e5-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="950e5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="950e5-136">displayName</span></span>|<span data-ttu-id="950e5-137">String</span><span class="sxs-lookup"><span data-stu-id="950e5-137">String</span></span>|<span data-ttu-id="950e5-138">Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="950e5-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="950e5-139">description</span><span class="sxs-lookup"><span data-stu-id="950e5-139">description</span></span>|<span data-ttu-id="950e5-140">String</span><span class="sxs-lookup"><span data-stu-id="950e5-140">String</span></span>|<span data-ttu-id="950e5-141">Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="950e5-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="950e5-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="950e5-142">versionInfo</span></span>|<span data-ttu-id="950e5-143">String</span><span class="sxs-lookup"><span data-stu-id="950e5-143">String</span></span>|<span data-ttu-id="950e5-144">Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="950e5-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="950e5-145">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="950e5-145">isDeprecated</span></span>|<span data-ttu-id="950e5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="950e5-146">Boolean</span></span>|<span data-ttu-id="950e5-147">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="950e5-147">The template is deprecated or not.</span></span> <span data-ttu-id="950e5-148">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="950e5-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="950e5-149">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="950e5-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="950e5-150">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="950e5-150">intentCount</span></span>|<span data-ttu-id="950e5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="950e5-151">Int32</span></span>|<span data-ttu-id="950e5-152">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="950e5-152">Number of Intents created from this template.</span></span> <span data-ttu-id="950e5-153">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="950e5-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="950e5-154">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="950e5-154">templateType</span></span>|[<span data-ttu-id="950e5-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="950e5-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="950e5-156">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="950e5-156">The template's type.</span></span> <span data-ttu-id="950e5-157">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="950e5-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="950e5-158">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span><span class="sxs-lookup"><span data-stu-id="950e5-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="950e5-159">platformType</span><span class="sxs-lookup"><span data-stu-id="950e5-159">platformType</span></span>|[<span data-ttu-id="950e5-160">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="950e5-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="950e5-161">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="950e5-161">The template's platform.</span></span> <span data-ttu-id="950e5-162">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="950e5-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="950e5-163">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="950e5-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="950e5-164">темплатесубтипе</span><span class="sxs-lookup"><span data-stu-id="950e5-164">templateSubtype</span></span>|[<span data-ttu-id="950e5-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="950e5-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="950e5-166">Подтип шаблона.</span><span class="sxs-lookup"><span data-stu-id="950e5-166">The template's subtype.</span></span> <span data-ttu-id="950e5-167">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="950e5-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="950e5-168">Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span><span class="sxs-lookup"><span data-stu-id="950e5-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="950e5-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="950e5-169">publishedDateTime</span></span>|<span data-ttu-id="950e5-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950e5-170">DateTimeOffset</span></span>|<span data-ttu-id="950e5-171">При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="950e5-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="950e5-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="950e5-172">Response</span></span>
<span data-ttu-id="950e5-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="950e5-173">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="950e5-174">Пример</span><span class="sxs-lookup"><span data-stu-id="950e5-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="950e5-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="950e5-175">Request</span></span>
<span data-ttu-id="950e5-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="950e5-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="950e5-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="950e5-177">Response</span></span>
<span data-ttu-id="950e5-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="950e5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




