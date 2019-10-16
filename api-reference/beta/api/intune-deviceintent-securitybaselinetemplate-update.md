---
title: Обновление Секуритибаселинетемплате
description: Обновление свойств объекта Секуритибаселинетемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbf27bc75e66e5c00a1d2f631980be70061c1e1d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37531884"
---
# <a name="update-securitybaselinetemplate"></a><span data-ttu-id="e03bc-103">Обновление Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="e03bc-103">Update securityBaselineTemplate</span></span>

> <span data-ttu-id="e03bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e03bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e03bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e03bc-106">Обновление свойств объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="e03bc-106">Update the properties of a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e03bc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e03bc-107">Prerequisites</span></span>
<span data-ttu-id="e03bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e03bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e03bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e03bc-110">Permission type</span></span>|<span data-ttu-id="e03bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e03bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e03bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e03bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e03bc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e03bc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e03bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e03bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e03bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03bc-115">Not supported.</span></span>|
|<span data-ttu-id="e03bc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e03bc-116">Application</span></span>|<span data-ttu-id="e03bc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e03bc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e03bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e03bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="e03bc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e03bc-119">Request headers</span></span>
|<span data-ttu-id="e03bc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e03bc-120">Header</span></span>|<span data-ttu-id="e03bc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e03bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e03bc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e03bc-122">Authorization</span></span>|<span data-ttu-id="e03bc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e03bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e03bc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e03bc-124">Accept</span></span>|<span data-ttu-id="e03bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e03bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e03bc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e03bc-126">Request body</span></span>
<span data-ttu-id="e03bc-127">В тексте запроса добавьте представление объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e03bc-127">In the request body, supply a JSON representation for the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

<span data-ttu-id="e03bc-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e03bc-128">The following table shows the properties that are required when you create the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).</span></span>

|<span data-ttu-id="e03bc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e03bc-129">Property</span></span>|<span data-ttu-id="e03bc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e03bc-130">Type</span></span>|<span data-ttu-id="e03bc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e03bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e03bc-132">id</span><span class="sxs-lookup"><span data-stu-id="e03bc-132">id</span></span>|<span data-ttu-id="e03bc-133">String</span><span class="sxs-lookup"><span data-stu-id="e03bc-133">String</span></span>|<span data-ttu-id="e03bc-134">Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e03bc-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e03bc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e03bc-135">displayName</span></span>|<span data-ttu-id="e03bc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="e03bc-136">String</span></span>|<span data-ttu-id="e03bc-137">Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e03bc-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e03bc-138">description</span><span class="sxs-lookup"><span data-stu-id="e03bc-138">description</span></span>|<span data-ttu-id="e03bc-139">String</span><span class="sxs-lookup"><span data-stu-id="e03bc-139">String</span></span>|<span data-ttu-id="e03bc-140">Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e03bc-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e03bc-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="e03bc-141">versionInfo</span></span>|<span data-ttu-id="e03bc-142">String</span><span class="sxs-lookup"><span data-stu-id="e03bc-142">String</span></span>|<span data-ttu-id="e03bc-143">Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e03bc-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e03bc-144">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="e03bc-144">isDeprecated</span></span>|<span data-ttu-id="e03bc-145">Логический</span><span class="sxs-lookup"><span data-stu-id="e03bc-145">Boolean</span></span>|<span data-ttu-id="e03bc-146">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="e03bc-146">The template is deprecated or not.</span></span> <span data-ttu-id="e03bc-147">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="e03bc-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="e03bc-148">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e03bc-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e03bc-149">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="e03bc-149">intentCount</span></span>|<span data-ttu-id="e03bc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e03bc-150">Int32</span></span>|<span data-ttu-id="e03bc-151">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="e03bc-151">Number of Intents created from this template.</span></span> <span data-ttu-id="e03bc-152">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e03bc-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="e03bc-153">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="e03bc-153">templateType</span></span>|[<span data-ttu-id="e03bc-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="e03bc-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="e03bc-155">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="e03bc-155">The template's type.</span></span> <span data-ttu-id="e03bc-156">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e03bc-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="e03bc-157">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span><span class="sxs-lookup"><span data-stu-id="e03bc-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span></span>|
|<span data-ttu-id="e03bc-158">platformType</span><span class="sxs-lookup"><span data-stu-id="e03bc-158">platformType</span></span>|[<span data-ttu-id="e03bc-159">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="e03bc-159">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="e03bc-160">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="e03bc-160">The template's platform.</span></span> <span data-ttu-id="e03bc-161">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="e03bc-161">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="e03bc-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="e03bc-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="e03bc-163">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e03bc-163">publishedDateTime</span></span>|<span data-ttu-id="e03bc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e03bc-164">DateTimeOffset</span></span>|<span data-ttu-id="e03bc-165">При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e03bc-165">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e03bc-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e03bc-166">Response</span></span>
<span data-ttu-id="e03bc-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e03bc-167">If successful, this method returns a `200 OK` response code and an updated [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e03bc-168">Пример</span><span class="sxs-lookup"><span data-stu-id="e03bc-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="e03bc-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="e03bc-169">Request</span></span>
<span data-ttu-id="e03bc-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e03bc-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
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

### <a name="response"></a><span data-ttu-id="e03bc-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="e03bc-171">Response</span></span>
<span data-ttu-id="e03bc-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e03bc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






