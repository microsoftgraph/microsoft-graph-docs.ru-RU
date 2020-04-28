---
title: Создание Секуритибаселинетемплате
description: Создание нового объекта Секуритибаселинетемплате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e1156255a9c936a7440091040443ace8d7bfd0b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427243"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="35727-103">Создание Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="35727-103">Create securityBaselineTemplate</span></span>

<span data-ttu-id="35727-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35727-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35727-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35727-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35727-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35727-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35727-107">Создание нового объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="35727-107">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35727-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35727-108">Prerequisites</span></span>
<span data-ttu-id="35727-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35727-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35727-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35727-111">Permission type</span></span>|<span data-ttu-id="35727-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35727-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35727-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35727-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35727-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35727-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35727-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35727-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35727-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35727-116">Not supported.</span></span>|
|<span data-ttu-id="35727-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35727-117">Application</span></span>|<span data-ttu-id="35727-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35727-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35727-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35727-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="35727-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="35727-120">Request headers</span></span>
|<span data-ttu-id="35727-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35727-121">Header</span></span>|<span data-ttu-id="35727-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35727-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35727-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35727-123">Authorization</span></span>|<span data-ttu-id="35727-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35727-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35727-125">Accept</span><span class="sxs-lookup"><span data-stu-id="35727-125">Accept</span></span>|<span data-ttu-id="35727-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35727-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35727-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35727-127">Request body</span></span>
<span data-ttu-id="35727-128">В тексте запроса добавьте представление объекта Секуритибаселинетемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35727-128">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="35727-129">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинетемплате.</span><span class="sxs-lookup"><span data-stu-id="35727-129">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="35727-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="35727-130">Property</span></span>|<span data-ttu-id="35727-131">Тип</span><span class="sxs-lookup"><span data-stu-id="35727-131">Type</span></span>|<span data-ttu-id="35727-132">Описание</span><span class="sxs-lookup"><span data-stu-id="35727-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35727-133">id</span><span class="sxs-lookup"><span data-stu-id="35727-133">id</span></span>|<span data-ttu-id="35727-134">String</span><span class="sxs-lookup"><span data-stu-id="35727-134">String</span></span>|<span data-ttu-id="35727-135">Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="35727-135">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="35727-136">displayName</span><span class="sxs-lookup"><span data-stu-id="35727-136">displayName</span></span>|<span data-ttu-id="35727-137">Строка</span><span class="sxs-lookup"><span data-stu-id="35727-137">String</span></span>|<span data-ttu-id="35727-138">Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="35727-138">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="35727-139">description</span><span class="sxs-lookup"><span data-stu-id="35727-139">description</span></span>|<span data-ttu-id="35727-140">String</span><span class="sxs-lookup"><span data-stu-id="35727-140">String</span></span>|<span data-ttu-id="35727-141">Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="35727-141">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="35727-142">versionInfo</span><span class="sxs-lookup"><span data-stu-id="35727-142">versionInfo</span></span>|<span data-ttu-id="35727-143">String</span><span class="sxs-lookup"><span data-stu-id="35727-143">String</span></span>|<span data-ttu-id="35727-144">Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="35727-144">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="35727-145">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="35727-145">isDeprecated</span></span>|<span data-ttu-id="35727-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="35727-146">Boolean</span></span>|<span data-ttu-id="35727-147">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="35727-147">The template is deprecated or not.</span></span> <span data-ttu-id="35727-148">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="35727-148">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="35727-149">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="35727-149">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="35727-150">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="35727-150">intentCount</span></span>|<span data-ttu-id="35727-151">Int32</span><span class="sxs-lookup"><span data-stu-id="35727-151">Int32</span></span>|<span data-ttu-id="35727-152">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="35727-152">Number of Intents created from this template.</span></span> <span data-ttu-id="35727-153">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="35727-153">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="35727-154">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="35727-154">templateType</span></span>|[<span data-ttu-id="35727-155">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="35727-155">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="35727-156">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="35727-156">The template's type.</span></span> <span data-ttu-id="35727-157">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="35727-157">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="35727-158">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span><span class="sxs-lookup"><span data-stu-id="35727-158">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.</span></span>|
|<span data-ttu-id="35727-159">platformType</span><span class="sxs-lookup"><span data-stu-id="35727-159">platformType</span></span>|[<span data-ttu-id="35727-160">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="35727-160">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="35727-161">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="35727-161">The template's platform.</span></span> <span data-ttu-id="35727-162">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="35727-162">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="35727-163">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="35727-163">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="35727-164">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="35727-164">publishedDateTime</span></span>|<span data-ttu-id="35727-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35727-165">DateTimeOffset</span></span>|<span data-ttu-id="35727-166">При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="35727-166">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="35727-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="35727-167">Response</span></span>
<span data-ttu-id="35727-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35727-168">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35727-169">Пример</span><span class="sxs-lookup"><span data-stu-id="35727-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="35727-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="35727-170">Request</span></span>
<span data-ttu-id="35727-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35727-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
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

### <a name="response"></a><span data-ttu-id="35727-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="35727-172">Response</span></span>
<span data-ttu-id="35727-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35727-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 420

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
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```



