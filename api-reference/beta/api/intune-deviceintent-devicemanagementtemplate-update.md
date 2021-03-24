---
title: Обновление deviceManagementTemplate
description: Обновление свойств объекта deviceManagementTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1134dc4a8c519d6c56ed1c2ad490a30fd72bc223
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130863"
---
# <a name="update-devicemanagementtemplate"></a><span data-ttu-id="f09ac-103">Обновление deviceManagementTemplate</span><span class="sxs-lookup"><span data-stu-id="f09ac-103">Update deviceManagementTemplate</span></span>

<span data-ttu-id="f09ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f09ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f09ac-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f09ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f09ac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f09ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f09ac-107">Обновление свойств объекта [deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f09ac-107">Update the properties of a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f09ac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f09ac-108">Prerequisites</span></span>
<span data-ttu-id="f09ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f09ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f09ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f09ac-111">Permission type</span></span>|<span data-ttu-id="f09ac-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f09ac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f09ac-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f09ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f09ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f09ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f09ac-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f09ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f09ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f09ac-116">Not supported.</span></span>|
|<span data-ttu-id="f09ac-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f09ac-117">Application</span></span>|<span data-ttu-id="f09ac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f09ac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f09ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f09ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="f09ac-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f09ac-120">Request headers</span></span>
|<span data-ttu-id="f09ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f09ac-121">Header</span></span>|<span data-ttu-id="f09ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f09ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f09ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f09ac-123">Authorization</span></span>|<span data-ttu-id="f09ac-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f09ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f09ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f09ac-125">Accept</span></span>|<span data-ttu-id="f09ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f09ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f09ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f09ac-127">Request body</span></span>
<span data-ttu-id="f09ac-128">В теле запроса поставляем представление JSON для [объекта deviceManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f09ac-128">In the request body, supply a JSON representation for the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

<span data-ttu-id="f09ac-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementTemplate.](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f09ac-129">The following table shows the properties that are required when you create the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span>

|<span data-ttu-id="f09ac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f09ac-130">Property</span></span>|<span data-ttu-id="f09ac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f09ac-131">Type</span></span>|<span data-ttu-id="f09ac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f09ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f09ac-133">id</span><span class="sxs-lookup"><span data-stu-id="f09ac-133">id</span></span>|<span data-ttu-id="f09ac-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f09ac-134">String</span></span>|<span data-ttu-id="f09ac-135">ID шаблона</span><span class="sxs-lookup"><span data-stu-id="f09ac-135">The template ID</span></span>|
|<span data-ttu-id="f09ac-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f09ac-136">displayName</span></span>|<span data-ttu-id="f09ac-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f09ac-137">String</span></span>|<span data-ttu-id="f09ac-138">Имя отображения шаблона</span><span class="sxs-lookup"><span data-stu-id="f09ac-138">The template's display name</span></span>|
|<span data-ttu-id="f09ac-139">description</span><span class="sxs-lookup"><span data-stu-id="f09ac-139">description</span></span>|<span data-ttu-id="f09ac-140">Строка</span><span class="sxs-lookup"><span data-stu-id="f09ac-140">String</span></span>|<span data-ttu-id="f09ac-141">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="f09ac-141">The template's description</span></span>|
|<span data-ttu-id="f09ac-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="f09ac-142">versionInfo</span></span>|<span data-ttu-id="f09ac-143">Строка</span><span class="sxs-lookup"><span data-stu-id="f09ac-143">String</span></span>|<span data-ttu-id="f09ac-144">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="f09ac-144">The template's version information</span></span>|
|<span data-ttu-id="f09ac-145">isDeprecated</span><span class="sxs-lookup"><span data-stu-id="f09ac-145">isDeprecated</span></span>|<span data-ttu-id="f09ac-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f09ac-146">Boolean</span></span>|<span data-ttu-id="f09ac-147">Шаблон обесценив или нет.</span><span class="sxs-lookup"><span data-stu-id="f09ac-147">The template is deprecated or not.</span></span> <span data-ttu-id="f09ac-148">Намерения не могут быть созданы из шаблона с законтятой расшифровкой.</span><span class="sxs-lookup"><span data-stu-id="f09ac-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="f09ac-149">intentCount</span><span class="sxs-lookup"><span data-stu-id="f09ac-149">intentCount</span></span>|<span data-ttu-id="f09ac-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f09ac-150">Int32</span></span>|<span data-ttu-id="f09ac-151">Количество намерений, созданных из этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="f09ac-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="f09ac-152">templateType</span><span class="sxs-lookup"><span data-stu-id="f09ac-152">templateType</span></span>|[<span data-ttu-id="f09ac-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="f09ac-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="f09ac-154">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="f09ac-154">The template's type.</span></span> <span data-ttu-id="f09ac-155">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span><span class="sxs-lookup"><span data-stu-id="f09ac-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`, `firewallSharedSettings`.</span></span>|
|<span data-ttu-id="f09ac-156">platformType</span><span class="sxs-lookup"><span data-stu-id="f09ac-156">platformType</span></span>|[<span data-ttu-id="f09ac-157">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="f09ac-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="f09ac-158">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="f09ac-158">The template's platform.</span></span> <span data-ttu-id="f09ac-159">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="f09ac-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="f09ac-160">templateSubtype</span><span class="sxs-lookup"><span data-stu-id="f09ac-160">templateSubtype</span></span>|[<span data-ttu-id="f09ac-161">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="f09ac-161">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="f09ac-162">Подтип шаблона.</span><span class="sxs-lookup"><span data-stu-id="f09ac-162">The template's subtype.</span></span> <span data-ttu-id="f09ac-163">Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span><span class="sxs-lookup"><span data-stu-id="f09ac-163">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`, `firewallSharedAppList`, `firewallSharedIpList`, `firewallSharedPortlist`.</span></span>|
|<span data-ttu-id="f09ac-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f09ac-164">publishedDateTime</span></span>|<span data-ttu-id="f09ac-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f09ac-165">DateTimeOffset</span></span>|<span data-ttu-id="f09ac-166">После публикации шаблона</span><span class="sxs-lookup"><span data-stu-id="f09ac-166">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="f09ac-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f09ac-167">Response</span></span>
<span data-ttu-id="f09ac-168">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f09ac-168">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f09ac-169">Пример</span><span class="sxs-lookup"><span data-stu-id="f09ac-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="f09ac-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="f09ac-170">Request</span></span>
<span data-ttu-id="f09ac-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f09ac-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="f09ac-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="f09ac-172">Response</span></span>
<span data-ttu-id="f09ac-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f09ac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




