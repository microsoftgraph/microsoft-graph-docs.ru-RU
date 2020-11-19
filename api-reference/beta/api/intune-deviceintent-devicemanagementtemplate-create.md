---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85a3640fd3822788e2ef7301191c729482add55c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286278"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="c23a8-103">Создание Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="c23a8-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="c23a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c23a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c23a8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c23a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c23a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c23a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c23a8-107">Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="c23a8-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c23a8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c23a8-108">Prerequisites</span></span>
<span data-ttu-id="c23a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c23a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c23a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c23a8-111">Permission type</span></span>|<span data-ttu-id="c23a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c23a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c23a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c23a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c23a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c23a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c23a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c23a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c23a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c23a8-116">Not supported.</span></span>|
|<span data-ttu-id="c23a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c23a8-117">Application</span></span>|<span data-ttu-id="c23a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c23a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c23a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c23a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="c23a8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c23a8-120">Request headers</span></span>
|<span data-ttu-id="c23a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c23a8-121">Header</span></span>|<span data-ttu-id="c23a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c23a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c23a8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c23a8-123">Authorization</span></span>|<span data-ttu-id="c23a8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c23a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c23a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c23a8-125">Accept</span></span>|<span data-ttu-id="c23a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c23a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c23a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c23a8-127">Request body</span></span>
<span data-ttu-id="c23a8-128">В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c23a8-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="c23a8-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.</span><span class="sxs-lookup"><span data-stu-id="c23a8-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="c23a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c23a8-130">Property</span></span>|<span data-ttu-id="c23a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c23a8-131">Type</span></span>|<span data-ttu-id="c23a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c23a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c23a8-133">id</span><span class="sxs-lookup"><span data-stu-id="c23a8-133">id</span></span>|<span data-ttu-id="c23a8-134">String</span><span class="sxs-lookup"><span data-stu-id="c23a8-134">String</span></span>|<span data-ttu-id="c23a8-135">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="c23a8-135">The template ID</span></span>|
|<span data-ttu-id="c23a8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c23a8-136">displayName</span></span>|<span data-ttu-id="c23a8-137">String</span><span class="sxs-lookup"><span data-stu-id="c23a8-137">String</span></span>|<span data-ttu-id="c23a8-138">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="c23a8-138">The template's display name</span></span>|
|<span data-ttu-id="c23a8-139">description</span><span class="sxs-lookup"><span data-stu-id="c23a8-139">description</span></span>|<span data-ttu-id="c23a8-140">String</span><span class="sxs-lookup"><span data-stu-id="c23a8-140">String</span></span>|<span data-ttu-id="c23a8-141">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="c23a8-141">The template's description</span></span>|
|<span data-ttu-id="c23a8-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="c23a8-142">versionInfo</span></span>|<span data-ttu-id="c23a8-143">String</span><span class="sxs-lookup"><span data-stu-id="c23a8-143">String</span></span>|<span data-ttu-id="c23a8-144">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="c23a8-144">The template's version information</span></span>|
|<span data-ttu-id="c23a8-145">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="c23a8-145">isDeprecated</span></span>|<span data-ttu-id="c23a8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c23a8-146">Boolean</span></span>|<span data-ttu-id="c23a8-147">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="c23a8-147">The template is deprecated or not.</span></span> <span data-ttu-id="c23a8-148">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="c23a8-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="c23a8-149">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="c23a8-149">intentCount</span></span>|<span data-ttu-id="c23a8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c23a8-150">Int32</span></span>|<span data-ttu-id="c23a8-151">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="c23a8-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="c23a8-152">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="c23a8-152">templateType</span></span>|[<span data-ttu-id="c23a8-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="c23a8-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="c23a8-154">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="c23a8-154">The template's type.</span></span> <span data-ttu-id="c23a8-155">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span><span class="sxs-lookup"><span data-stu-id="c23a8-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="c23a8-156">platformType</span><span class="sxs-lookup"><span data-stu-id="c23a8-156">platformType</span></span>|[<span data-ttu-id="c23a8-157">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="c23a8-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="c23a8-158">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="c23a8-158">The template's platform.</span></span> <span data-ttu-id="c23a8-159">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="c23a8-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="c23a8-160">темплатесубтипе</span><span class="sxs-lookup"><span data-stu-id="c23a8-160">templateSubtype</span></span>|[<span data-ttu-id="c23a8-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="c23a8-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="c23a8-162">Подтип шаблона.</span><span class="sxs-lookup"><span data-stu-id="c23a8-162">The template's subtype.</span></span> <span data-ttu-id="c23a8-163">Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span><span class="sxs-lookup"><span data-stu-id="c23a8-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="c23a8-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c23a8-164">publishedDateTime</span></span>|<span data-ttu-id="c23a8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c23a8-165">DateTimeOffset</span></span>|<span data-ttu-id="c23a8-166">При публикации шаблона</span><span class="sxs-lookup"><span data-stu-id="c23a8-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="c23a8-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="c23a8-167">Response</span></span>
<span data-ttu-id="c23a8-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c23a8-168">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c23a8-169">Пример</span><span class="sxs-lookup"><span data-stu-id="c23a8-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="c23a8-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="c23a8-170">Request</span></span>
<span data-ttu-id="c23a8-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c23a8-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
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

### <a name="response"></a><span data-ttu-id="c23a8-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="c23a8-172">Response</span></span>
<span data-ttu-id="c23a8-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c23a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
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




