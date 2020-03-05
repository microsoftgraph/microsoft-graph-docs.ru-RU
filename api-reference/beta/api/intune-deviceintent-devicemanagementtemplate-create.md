---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 829413729d1ed2abbe55e624034f0b8a243a390b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470436"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="c011f-103">Создание Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="c011f-103">Create deviceManagementTemplate</span></span>

<span data-ttu-id="c011f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c011f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c011f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c011f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c011f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c011f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c011f-107">Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="c011f-107">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c011f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c011f-108">Prerequisites</span></span>
<span data-ttu-id="c011f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c011f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c011f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c011f-111">Permission type</span></span>|<span data-ttu-id="c011f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c011f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c011f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c011f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c011f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c011f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c011f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c011f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c011f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c011f-116">Not supported.</span></span>|
|<span data-ttu-id="c011f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c011f-117">Application</span></span>|<span data-ttu-id="c011f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c011f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c011f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c011f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="c011f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c011f-120">Request headers</span></span>
|<span data-ttu-id="c011f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c011f-121">Header</span></span>|<span data-ttu-id="c011f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c011f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c011f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c011f-123">Authorization</span></span>|<span data-ttu-id="c011f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c011f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c011f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c011f-125">Accept</span></span>|<span data-ttu-id="c011f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c011f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c011f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c011f-127">Request body</span></span>
<span data-ttu-id="c011f-128">В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c011f-128">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="c011f-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.</span><span class="sxs-lookup"><span data-stu-id="c011f-129">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="c011f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c011f-130">Property</span></span>|<span data-ttu-id="c011f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c011f-131">Type</span></span>|<span data-ttu-id="c011f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c011f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c011f-133">id</span><span class="sxs-lookup"><span data-stu-id="c011f-133">id</span></span>|<span data-ttu-id="c011f-134">String</span><span class="sxs-lookup"><span data-stu-id="c011f-134">String</span></span>|<span data-ttu-id="c011f-135">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="c011f-135">The template ID</span></span>|
|<span data-ttu-id="c011f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c011f-136">displayName</span></span>|<span data-ttu-id="c011f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c011f-137">String</span></span>|<span data-ttu-id="c011f-138">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="c011f-138">The template's display name</span></span>|
|<span data-ttu-id="c011f-139">description</span><span class="sxs-lookup"><span data-stu-id="c011f-139">description</span></span>|<span data-ttu-id="c011f-140">String</span><span class="sxs-lookup"><span data-stu-id="c011f-140">String</span></span>|<span data-ttu-id="c011f-141">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="c011f-141">The template's description</span></span>|
|<span data-ttu-id="c011f-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="c011f-142">versionInfo</span></span>|<span data-ttu-id="c011f-143">String</span><span class="sxs-lookup"><span data-stu-id="c011f-143">String</span></span>|<span data-ttu-id="c011f-144">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="c011f-144">The template's version information</span></span>|
|<span data-ttu-id="c011f-145">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="c011f-145">isDeprecated</span></span>|<span data-ttu-id="c011f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c011f-146">Boolean</span></span>|<span data-ttu-id="c011f-147">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="c011f-147">The template is deprecated or not.</span></span> <span data-ttu-id="c011f-148">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="c011f-148">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="c011f-149">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="c011f-149">intentCount</span></span>|<span data-ttu-id="c011f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c011f-150">Int32</span></span>|<span data-ttu-id="c011f-151">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="c011f-151">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="c011f-152">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="c011f-152">templateType</span></span>|[<span data-ttu-id="c011f-153">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="c011f-153">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="c011f-154">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="c011f-154">The template's type.</span></span> <span data-ttu-id="c011f-155">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span><span class="sxs-lookup"><span data-stu-id="c011f-155">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="c011f-156">platformType</span><span class="sxs-lookup"><span data-stu-id="c011f-156">platformType</span></span>|[<span data-ttu-id="c011f-157">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="c011f-157">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="c011f-158">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="c011f-158">The template's platform.</span></span> <span data-ttu-id="c011f-159">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="c011f-159">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="c011f-160">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="c011f-160">publishedDateTime</span></span>|<span data-ttu-id="c011f-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c011f-161">DateTimeOffset</span></span>|<span data-ttu-id="c011f-162">При публикации шаблона</span><span class="sxs-lookup"><span data-stu-id="c011f-162">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="c011f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c011f-163">Response</span></span>
<span data-ttu-id="c011f-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c011f-164">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c011f-165">Пример</span><span class="sxs-lookup"><span data-stu-id="c011f-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c011f-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c011f-166">Request</span></span>
<span data-ttu-id="c011f-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c011f-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c011f-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c011f-168">Response</span></span>
<span data-ttu-id="c011f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c011f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





