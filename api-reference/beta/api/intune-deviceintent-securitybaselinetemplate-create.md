---
title: Создание Секуритибаселинетемплате
description: Создание нового объекта Секуритибаселинетемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ecf477b0ad24232cd9a42e7e1070dcf266d6d14
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945342"
---
# <a name="create-securitybaselinetemplate"></a><span data-ttu-id="1a928-103">Создание Секуритибаселинетемплате</span><span class="sxs-lookup"><span data-stu-id="1a928-103">Create securityBaselineTemplate</span></span>

> <span data-ttu-id="1a928-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a928-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a928-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a928-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a928-106">Создание нового объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="1a928-106">Create a new [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a928-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1a928-107">Prerequisites</span></span>
<span data-ttu-id="1a928-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a928-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a928-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a928-110">Permission type</span></span>|<span data-ttu-id="1a928-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a928-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a928-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a928-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a928-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a928-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a928-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a928-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a928-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a928-115">Not supported.</span></span>|
|<span data-ttu-id="1a928-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a928-116">Application</span></span>|<span data-ttu-id="1a928-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a928-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a928-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a928-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="1a928-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1a928-119">Request headers</span></span>
|<span data-ttu-id="1a928-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a928-120">Header</span></span>|<span data-ttu-id="1a928-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a928-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a928-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a928-122">Authorization</span></span>|<span data-ttu-id="1a928-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a928-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a928-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a928-124">Accept</span></span>|<span data-ttu-id="1a928-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a928-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a928-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a928-126">Request body</span></span>
<span data-ttu-id="1a928-127">В тексте запроса добавьте представление объекта Секуритибаселинетемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a928-127">In the request body, supply a JSON representation for the securityBaselineTemplate object.</span></span>

<span data-ttu-id="1a928-128">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинетемплате.</span><span class="sxs-lookup"><span data-stu-id="1a928-128">The following table shows the properties that are required when you create the securityBaselineTemplate.</span></span>

|<span data-ttu-id="1a928-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a928-129">Property</span></span>|<span data-ttu-id="1a928-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a928-130">Type</span></span>|<span data-ttu-id="1a928-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a928-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a928-132">id</span><span class="sxs-lookup"><span data-stu-id="1a928-132">id</span></span>|<span data-ttu-id="1a928-133">String</span><span class="sxs-lookup"><span data-stu-id="1a928-133">String</span></span>|<span data-ttu-id="1a928-134">Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1a928-134">The template ID Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1a928-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1a928-135">displayName</span></span>|<span data-ttu-id="1a928-136">Строка</span><span class="sxs-lookup"><span data-stu-id="1a928-136">String</span></span>|<span data-ttu-id="1a928-137">Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1a928-137">The template's display name Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1a928-138">description</span><span class="sxs-lookup"><span data-stu-id="1a928-138">description</span></span>|<span data-ttu-id="1a928-139">String</span><span class="sxs-lookup"><span data-stu-id="1a928-139">String</span></span>|<span data-ttu-id="1a928-140">Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1a928-140">The template's description Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1a928-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="1a928-141">versionInfo</span></span>|<span data-ttu-id="1a928-142">Строка</span><span class="sxs-lookup"><span data-stu-id="1a928-142">String</span></span>|<span data-ttu-id="1a928-143">Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1a928-143">The template's version information Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1a928-144">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="1a928-144">isDeprecated</span></span>|<span data-ttu-id="1a928-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a928-145">Boolean</span></span>|<span data-ttu-id="1a928-146">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1a928-146">The template is deprecated or not.</span></span> <span data-ttu-id="1a928-147">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="1a928-147">Intents cannot be created from a deprecated template.</span></span> <span data-ttu-id="1a928-148">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1a928-148">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1a928-149">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="1a928-149">intentCount</span></span>|<span data-ttu-id="1a928-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1a928-150">Int32</span></span>|<span data-ttu-id="1a928-151">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="1a928-151">Number of Intents created from this template.</span></span> <span data-ttu-id="1a928-152">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1a928-152">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|
|<span data-ttu-id="1a928-153">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="1a928-153">templateType</span></span>|[<span data-ttu-id="1a928-154">deviceManagementTemplateType</span><span class="sxs-lookup"><span data-stu-id="1a928-154">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="1a928-155">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="1a928-155">The template's type.</span></span> <span data-ttu-id="1a928-156">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="1a928-156">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="1a928-157">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span><span class="sxs-lookup"><span data-stu-id="1a928-157">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.</span></span>|
|<span data-ttu-id="1a928-158">platformType</span><span class="sxs-lookup"><span data-stu-id="1a928-158">platformType</span></span>|[<span data-ttu-id="1a928-159">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="1a928-159">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="1a928-160">Платформа шаблона.</span><span class="sxs-lookup"><span data-stu-id="1a928-160">The template's platform.</span></span> <span data-ttu-id="1a928-161">Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="1a928-161">Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).</span></span> <span data-ttu-id="1a928-162">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="1a928-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="1a928-163">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a928-163">publishedDateTime</span></span>|<span data-ttu-id="1a928-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a928-164">DateTimeOffset</span></span>|<span data-ttu-id="1a928-165">При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="1a928-165">When the template was published Inherited from [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1a928-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a928-166">Response</span></span>
<span data-ttu-id="1a928-167">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a928-167">If successful, this method returns a `201 Created` response code and a [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a928-168">Пример</span><span class="sxs-lookup"><span data-stu-id="1a928-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a928-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a928-169">Request</span></span>
<span data-ttu-id="1a928-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a928-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1a928-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a928-171">Response</span></span>
<span data-ttu-id="1a928-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a928-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





