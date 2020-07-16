---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc741640f5f8762985ccbe7ad2d261524f9ee73c
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122758"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="d6b2d-103">Создание Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="d6b2d-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="d6b2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6b2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6b2d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6b2d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6b2d-107">Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="d6b2d-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6b2d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6b2d-108">Prerequisites</span></span>
<span data-ttu-id="d6b2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6b2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6b2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6b2d-111">Permission type</span></span>|<span data-ttu-id="d6b2d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6b2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6b2d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6b2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6b2d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b2d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6b2d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6b2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6b2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-116">Not supported.</span></span>|
|<span data-ttu-id="d6b2d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6b2d-117">Application</span></span>|<span data-ttu-id="d6b2d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b2d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6b2d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6b2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="d6b2d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6b2d-120">Request headers</span></span>
|<span data-ttu-id="d6b2d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6b2d-121">Header</span></span>|<span data-ttu-id="d6b2d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6b2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6b2d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6b2d-123">Authorization</span></span>|<span data-ttu-id="d6b2d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6b2d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6b2d-125">Accept</span></span>|<span data-ttu-id="d6b2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6b2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6b2d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6b2d-127">Request body</span></span>
<span data-ttu-id="d6b2d-128">В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="d6b2d-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="d6b2d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6b2d-130">Property</span></span>|<span data-ttu-id="d6b2d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6b2d-131">Type</span></span>|<span data-ttu-id="d6b2d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6b2d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6b2d-133">id</span><span class="sxs-lookup"><span data-stu-id="d6b2d-133">id</span></span>|<span data-ttu-id="d6b2d-134">String</span><span class="sxs-lookup"><span data-stu-id="d6b2d-134">String</span></span>|<span data-ttu-id="d6b2d-135">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="d6b2d-135">The template ID</span></span>|
|<span data-ttu-id="d6b2d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d6b2d-136">displayName</span></span>|<span data-ttu-id="d6b2d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d6b2d-137">String</span></span>|<span data-ttu-id="d6b2d-138">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="d6b2d-138">The template's display name</span></span>|
|<span data-ttu-id="d6b2d-139">description</span><span class="sxs-lookup"><span data-stu-id="d6b2d-139">description</span></span>|<span data-ttu-id="d6b2d-140">String</span><span class="sxs-lookup"><span data-stu-id="d6b2d-140">String</span></span>|<span data-ttu-id="d6b2d-141">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="d6b2d-141">The template's description</span></span>|
|<span data-ttu-id="d6b2d-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="d6b2d-142">versionInfo</span></span>|<span data-ttu-id="d6b2d-143">String</span><span class="sxs-lookup"><span data-stu-id="d6b2d-143">String</span></span>|<span data-ttu-id="d6b2d-144">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="d6b2d-144">The template's version information</span></span>|
|<span data-ttu-id="d6b2d-145">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="d6b2d-145">isDeprecated</span></span>|<span data-ttu-id="d6b2d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="d6b2d-146">Boolean</span></span>|<span data-ttu-id="d6b2d-147">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-147">The template is deprecated or not.</span></span> <span data-ttu-id="d6b2d-148">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="d6b2d-149">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="d6b2d-149">intentCount</span></span>|<span data-ttu-id="d6b2d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d6b2d-150">Int32</span></span>|<span data-ttu-id="d6b2d-151">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="d6b2d-152">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="d6b2d-152">templateType</span></span>|[<span data-ttu-id="d6b2d-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="d6b2d-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="d6b2d-154">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-154">The template's type.</span></span> <span data-ttu-id="d6b2d-155">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`.</span></span>|
|<span data-ttu-id="d6b2d-156">platformType</span><span class="sxs-lookup"><span data-stu-id="d6b2d-156">platformType</span></span>|[<span data-ttu-id="d6b2d-157">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="d6b2d-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="d6b2d-158">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-158">The template's platform.</span></span> <span data-ttu-id="d6b2d-159">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="d6b2d-160">темплатесубтипе</span><span class="sxs-lookup"><span data-stu-id="d6b2d-160">templateSubtype</span></span>|[<span data-ttu-id="d6b2d-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="d6b2d-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="d6b2d-162">Подтип шаблона.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-162">The template's subtype.</span></span> <span data-ttu-id="d6b2d-163">Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span></span>|
|<span data-ttu-id="d6b2d-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b2d-164">publishedDateTime</span></span>|<span data-ttu-id="d6b2d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b2d-165">DateTimeOffset</span></span>|<span data-ttu-id="d6b2d-166">При публикации шаблона</span><span class="sxs-lookup"><span data-stu-id="d6b2d-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="d6b2d-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b2d-167">Response</span></span>
<span data-ttu-id="d6b2d-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-168">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6b2d-169">Пример</span><span class="sxs-lookup"><span data-stu-id="d6b2d-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6b2d-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6b2d-170">Request</span></span>
<span data-ttu-id="d6b2d-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6b2d-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b2d-172">Response</span></span>
<span data-ttu-id="d6b2d-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6b2d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



