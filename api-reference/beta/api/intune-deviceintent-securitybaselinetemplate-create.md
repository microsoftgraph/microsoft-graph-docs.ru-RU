---
title: Создание Секуритибаселинетемплате
description: Создание нового объекта Секуритибаселинетемплате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c239155870659d4d9d66bb8395524ef0b8c7706
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723303"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="c04bd-103">Создание Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="c04bd-103">Create securityBaselineTemplate</span></span>

<span data-ttu-id="c04bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c04bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c04bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c04bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c04bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c04bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c04bd-107">Создание нового объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="c04bd-107">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c04bd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c04bd-108">Prerequisites</span></span>
<span data-ttu-id="c04bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c04bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c04bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c04bd-111">Permission type</span></span>|<span data-ttu-id="c04bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c04bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c04bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c04bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c04bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c04bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c04bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c04bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c04bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c04bd-116">Not supported.</span></span>|
|<span data-ttu-id="c04bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c04bd-117">Application</span></span>|<span data-ttu-id="c04bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c04bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c04bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c04bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="c04bd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c04bd-120">Request headers</span></span>
|<span data-ttu-id="c04bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c04bd-121">Header</span></span>|<span data-ttu-id="c04bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c04bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c04bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c04bd-123">Authorization</span></span>|<span data-ttu-id="c04bd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c04bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c04bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c04bd-125">Accept</span></span>|<span data-ttu-id="c04bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c04bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c04bd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c04bd-127">Request body</span></span>
<span data-ttu-id="c04bd-128">В тексте запроса добавьте представление объекта Секуритибаселинетемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c04bd-128">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="c04bd-129">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинетемплате.</span><span class="sxs-lookup"><span data-stu-id="c04bd-129">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="c04bd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c04bd-130">Property</span></span>|<span data-ttu-id="c04bd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c04bd-131">Type</span></span>|<span data-ttu-id="c04bd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c04bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c04bd-133">id</span><span class="sxs-lookup"><span data-stu-id="c04bd-133">id</span></span>|<span data-ttu-id="c04bd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c04bd-134">String</span></span>|<span data-ttu-id="c04bd-135">Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c04bd-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="c04bd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c04bd-136">displayName</span></span>|<span data-ttu-id="c04bd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c04bd-137">String</span></span>|<span data-ttu-id="c04bd-138">Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c04bd-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="c04bd-139">description</span><span class="sxs-lookup"><span data-stu-id="c04bd-139">description</span></span>|<span data-ttu-id="c04bd-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c04bd-140">String</span></span>|<span data-ttu-id="c04bd-141">Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c04bd-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="c04bd-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="c04bd-142">versionInfo</span></span>|<span data-ttu-id="c04bd-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c04bd-143">String</span></span>|<span data-ttu-id="c04bd-144">Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c04bd-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="c04bd-145">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="c04bd-145">isDeprecated</span></span>|<span data-ttu-id="c04bd-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c04bd-146">Boolean</span></span>|<span data-ttu-id="c04bd-147">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="c04bd-147">The template is deprecated or not.</span></span> <span data-ttu-id="c04bd-148">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="c04bd-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="c04bd-149">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c04bd-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="c04bd-150">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="c04bd-150">intentCount</span></span>|<span data-ttu-id="c04bd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c04bd-151">Int32</span></span>|<span data-ttu-id="c04bd-152">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="c04bd-152">Number of Intents created from this template.</span></span> <span data-ttu-id="c04bd-153">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c04bd-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="c04bd-154">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="c04bd-154">templateType</span></span>|[<span data-ttu-id="c04bd-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="c04bd-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="c04bd-156">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="c04bd-156">The template's type.</span></span> <span data-ttu-id="c04bd-157">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c04bd-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="c04bd-158">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`.</span><span class="sxs-lookup"><span data-stu-id="c04bd-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`.</span></span>|
|<span data-ttu-id="c04bd-159">platformType</span><span class="sxs-lookup"><span data-stu-id="c04bd-159">platformType</span></span>|[<span data-ttu-id="c04bd-160">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="c04bd-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="c04bd-161">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="c04bd-161">The template's platform.</span></span> <span data-ttu-id="c04bd-162">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c04bd-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="c04bd-163">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="c04bd-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="c04bd-164">темплатесубтипе</span><span class="sxs-lookup"><span data-stu-id="c04bd-164">templateSubtype</span></span>|[<span data-ttu-id="c04bd-165">deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="c04bd-165">deviceManagementTemplateSubtype</span></span>](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|<span data-ttu-id="c04bd-166">Подтип шаблона.</span><span class="sxs-lookup"><span data-stu-id="c04bd-166">The template's subtype.</span></span> <span data-ttu-id="c04bd-167">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c04bd-167">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="c04bd-168">Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span><span class="sxs-lookup"><span data-stu-id="c04bd-168">Possible values are: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.</span></span>|
|<span data-ttu-id="c04bd-169">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c04bd-169">publishedDateTime</span></span>|<span data-ttu-id="c04bd-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c04bd-170">DateTimeOffset</span></span>|<span data-ttu-id="c04bd-171">При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c04bd-171">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c04bd-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="c04bd-172">Response</span></span>
<span data-ttu-id="c04bd-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c04bd-173">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c04bd-174">Пример</span><span class="sxs-lookup"><span data-stu-id="c04bd-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="c04bd-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="c04bd-175">Request</span></span>
<span data-ttu-id="c04bd-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c04bd-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c04bd-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c04bd-177">Response</span></span>
<span data-ttu-id="c04bd-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c04bd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





