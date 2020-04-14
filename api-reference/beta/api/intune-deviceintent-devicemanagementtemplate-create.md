---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01f3c719e0f5ad2b77c48f223dd198aa7b92e96b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381440"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="b991c-103">Создание Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="b991c-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="b991c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b991c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b991c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b991c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b991c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b991c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b991c-107">Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="b991c-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b991c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b991c-108">Prerequisites</span></span>
<span data-ttu-id="b991c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b991c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b991c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b991c-111">Permission type</span></span>|<span data-ttu-id="b991c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b991c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b991c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b991c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b991c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b991c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b991c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b991c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b991c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b991c-116">Not supported.</span></span>|
|<span data-ttu-id="b991c-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b991c-117">Application</span></span>|<span data-ttu-id="b991c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b991c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b991c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b991c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="b991c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b991c-120">Request headers</span></span>
|<span data-ttu-id="b991c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b991c-121">Header</span></span>|<span data-ttu-id="b991c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b991c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b991c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b991c-123">Authorization</span></span>|<span data-ttu-id="b991c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b991c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b991c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b991c-125">Accept</span></span>|<span data-ttu-id="b991c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b991c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b991c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b991c-127">Request body</span></span>
<span data-ttu-id="b991c-128">В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b991c-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="b991c-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.</span><span class="sxs-lookup"><span data-stu-id="b991c-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="b991c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b991c-130">Property</span></span>|<span data-ttu-id="b991c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b991c-131">Type</span></span>|<span data-ttu-id="b991c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b991c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b991c-133">id</span><span class="sxs-lookup"><span data-stu-id="b991c-133">id</span></span>|<span data-ttu-id="b991c-134">String</span><span class="sxs-lookup"><span data-stu-id="b991c-134">String</span></span>|<span data-ttu-id="b991c-135">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="b991c-135">The template ID</span></span>|
|<span data-ttu-id="b991c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b991c-136">displayName</span></span>|<span data-ttu-id="b991c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b991c-137">String</span></span>|<span data-ttu-id="b991c-138">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="b991c-138">The template's display name</span></span>|
|<span data-ttu-id="b991c-139">description</span><span class="sxs-lookup"><span data-stu-id="b991c-139">description</span></span>|<span data-ttu-id="b991c-140">String</span><span class="sxs-lookup"><span data-stu-id="b991c-140">String</span></span>|<span data-ttu-id="b991c-141">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="b991c-141">The template's description</span></span>|
|<span data-ttu-id="b991c-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="b991c-142">versionInfo</span></span>|<span data-ttu-id="b991c-143">String</span><span class="sxs-lookup"><span data-stu-id="b991c-143">String</span></span>|<span data-ttu-id="b991c-144">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="b991c-144">The template's version information</span></span>|
|<span data-ttu-id="b991c-145">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="b991c-145">isDeprecated</span></span>|<span data-ttu-id="b991c-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="b991c-146">Boolean</span></span>|<span data-ttu-id="b991c-147">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="b991c-147">The template is deprecated or not.</span></span> <span data-ttu-id="b991c-148">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="b991c-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="b991c-149">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="b991c-149">intentCount</span></span>|<span data-ttu-id="b991c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b991c-150">Int32</span></span>|<span data-ttu-id="b991c-151">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="b991c-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="b991c-152">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="b991c-152">templateType</span></span>|[<span data-ttu-id="b991c-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="b991c-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="b991c-154">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="b991c-154">The template's type.</span></span> <span data-ttu-id="b991c-155">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span><span class="sxs-lookup"><span data-stu-id="b991c-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="b991c-156">platformType</span><span class="sxs-lookup"><span data-stu-id="b991c-156">platformType</span></span>|[<span data-ttu-id="b991c-157">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="b991c-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="b991c-158">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="b991c-158">The template's platform.</span></span> <span data-ttu-id="b991c-159">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b991c-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="b991c-160">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="b991c-160">publishedDateTime</span></span>|<span data-ttu-id="b991c-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b991c-161">DateTimeOffset</span></span>|<span data-ttu-id="b991c-162">При публикации шаблона</span><span class="sxs-lookup"><span data-stu-id="b991c-162">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="b991c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b991c-163">Response</span></span>
<span data-ttu-id="b991c-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b991c-164">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b991c-165">Пример</span><span class="sxs-lookup"><span data-stu-id="b991c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="b991c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="b991c-166">Request</span></span>
<span data-ttu-id="b991c-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b991c-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b991c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="b991c-168">Response</span></span>
<span data-ttu-id="b991c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b991c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 420

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
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```



