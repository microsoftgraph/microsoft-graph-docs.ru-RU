---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ded97215536cc2abf3950d497da8eff63d76095e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945503"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="abb5f-103">Создание Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="abb5f-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="abb5f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abb5f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abb5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abb5f-106">Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="abb5f-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abb5f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="abb5f-107">Prerequisites</span></span>
<span data-ttu-id="abb5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abb5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb5f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abb5f-110">Permission type</span></span>|<span data-ttu-id="abb5f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abb5f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb5f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abb5f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abb5f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb5f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abb5f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abb5f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb5f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb5f-115">Not supported.</span></span>|
|<span data-ttu-id="abb5f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abb5f-116">Application</span></span>|<span data-ttu-id="abb5f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb5f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb5f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abb5f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="abb5f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="abb5f-119">Request headers</span></span>
|<span data-ttu-id="abb5f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abb5f-120">Header</span></span>|<span data-ttu-id="abb5f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="abb5f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abb5f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abb5f-122">Authorization</span></span>|<span data-ttu-id="abb5f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abb5f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abb5f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="abb5f-124">Accept</span></span>|<span data-ttu-id="abb5f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abb5f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb5f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="abb5f-126">Request body</span></span>
<span data-ttu-id="abb5f-127">В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abb5f-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="abb5f-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.</span><span class="sxs-lookup"><span data-stu-id="abb5f-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="abb5f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="abb5f-129">Property</span></span>|<span data-ttu-id="abb5f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="abb5f-130">Type</span></span>|<span data-ttu-id="abb5f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="abb5f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abb5f-132">id</span><span class="sxs-lookup"><span data-stu-id="abb5f-132">id</span></span>|<span data-ttu-id="abb5f-133">String</span><span class="sxs-lookup"><span data-stu-id="abb5f-133">String</span></span>|<span data-ttu-id="abb5f-134">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="abb5f-134">The template ID</span></span>|
|<span data-ttu-id="abb5f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="abb5f-135">displayName</span></span>|<span data-ttu-id="abb5f-136">Строка</span><span class="sxs-lookup"><span data-stu-id="abb5f-136">String</span></span>|<span data-ttu-id="abb5f-137">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="abb5f-137">The template's display name</span></span>|
|<span data-ttu-id="abb5f-138">description</span><span class="sxs-lookup"><span data-stu-id="abb5f-138">description</span></span>|<span data-ttu-id="abb5f-139">String</span><span class="sxs-lookup"><span data-stu-id="abb5f-139">String</span></span>|<span data-ttu-id="abb5f-140">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="abb5f-140">The template's description</span></span>|
|<span data-ttu-id="abb5f-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="abb5f-141">versionInfo</span></span>|<span data-ttu-id="abb5f-142">Строка</span><span class="sxs-lookup"><span data-stu-id="abb5f-142">String</span></span>|<span data-ttu-id="abb5f-143">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="abb5f-143">The template's version information</span></span>|
|<span data-ttu-id="abb5f-144">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="abb5f-144">isDeprecated</span></span>|<span data-ttu-id="abb5f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="abb5f-145">Boolean</span></span>|<span data-ttu-id="abb5f-146">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="abb5f-146">The template is deprecated or not.</span></span> <span data-ttu-id="abb5f-147">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="abb5f-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="abb5f-148">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="abb5f-148">intentCount</span></span>|<span data-ttu-id="abb5f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="abb5f-149">Int32</span></span>|<span data-ttu-id="abb5f-150">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="abb5f-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="abb5f-151">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="abb5f-151">templateType</span></span>|[<span data-ttu-id="abb5f-152">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="abb5f-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="abb5f-153">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="abb5f-153">The template's type.</span></span> <span data-ttu-id="abb5f-154">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span><span class="sxs-lookup"><span data-stu-id="abb5f-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span></span>|
|<span data-ttu-id="abb5f-155">platformType</span><span class="sxs-lookup"><span data-stu-id="abb5f-155">platformType</span></span>|[<span data-ttu-id="abb5f-156">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="abb5f-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="abb5f-157">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="abb5f-157">The template's platform.</span></span> <span data-ttu-id="abb5f-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="abb5f-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="abb5f-159">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="abb5f-159">publishedDateTime</span></span>|<span data-ttu-id="abb5f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abb5f-160">DateTimeOffset</span></span>|<span data-ttu-id="abb5f-161">При публикации шаблона</span><span class="sxs-lookup"><span data-stu-id="abb5f-161">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="abb5f-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="abb5f-162">Response</span></span>
<span data-ttu-id="abb5f-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="abb5f-163">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb5f-164">Пример</span><span class="sxs-lookup"><span data-stu-id="abb5f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="abb5f-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb5f-165">Request</span></span>
<span data-ttu-id="abb5f-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abb5f-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="abb5f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb5f-167">Response</span></span>
<span data-ttu-id="abb5f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abb5f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





