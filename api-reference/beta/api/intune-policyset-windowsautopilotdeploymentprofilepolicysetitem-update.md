---
title: Обновление Виндовсаутопилотдеплойментпрофилеполицисетитем
description: Обновление свойств объекта Виндовсаутопилотдеплойментпрофилеполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf52e7b5819fa12b0b4b40962f86bc8bef1e2b1b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437893"
---
# <a name="update-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="e89eb-103">Обновление Виндовсаутопилотдеплойментпрофилеполицисетитем</span><span class="sxs-lookup"><span data-stu-id="e89eb-103">Update windowsAutopilotDeploymentProfilePolicySetItem</span></span>

<span data-ttu-id="e89eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e89eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e89eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e89eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e89eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e89eb-107">Обновление свойств объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="e89eb-107">Update the properties of a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e89eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e89eb-108">Prerequisites</span></span>
<span data-ttu-id="e89eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e89eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e89eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e89eb-111">Permission type</span></span>|<span data-ttu-id="e89eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e89eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e89eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e89eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e89eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e89eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e89eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e89eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e89eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89eb-116">Not supported.</span></span>|
|<span data-ttu-id="e89eb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e89eb-117">Application</span></span>|<span data-ttu-id="e89eb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e89eb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e89eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e89eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="e89eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e89eb-120">Request headers</span></span>
|<span data-ttu-id="e89eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e89eb-121">Header</span></span>|<span data-ttu-id="e89eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e89eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e89eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e89eb-123">Authorization</span></span>|<span data-ttu-id="e89eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e89eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e89eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e89eb-125">Accept</span></span>|<span data-ttu-id="e89eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e89eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e89eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e89eb-127">Request body</span></span>
<span data-ttu-id="e89eb-128">В тексте запроса добавьте представление объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e89eb-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

<span data-ttu-id="e89eb-129">В следующей таблице приведены свойства, необходимые при создании [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="e89eb-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span></span>

|<span data-ttu-id="e89eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e89eb-130">Property</span></span>|<span data-ttu-id="e89eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e89eb-131">Type</span></span>|<span data-ttu-id="e89eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e89eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e89eb-133">id</span><span class="sxs-lookup"><span data-stu-id="e89eb-133">id</span></span>|<span data-ttu-id="e89eb-134">String</span><span class="sxs-lookup"><span data-stu-id="e89eb-134">String</span></span>|<span data-ttu-id="e89eb-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="e89eb-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="e89eb-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e89eb-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e89eb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e89eb-137">createdDateTime</span></span>|<span data-ttu-id="e89eb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e89eb-138">DateTimeOffset</span></span>|<span data-ttu-id="e89eb-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="e89eb-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="e89eb-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e89eb-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e89eb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e89eb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e89eb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e89eb-142">DateTimeOffset</span></span>|<span data-ttu-id="e89eb-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="e89eb-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="e89eb-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e89eb-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e89eb-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="e89eb-145">payloadId</span></span>|<span data-ttu-id="e89eb-146">String</span><span class="sxs-lookup"><span data-stu-id="e89eb-146">String</span></span>|<span data-ttu-id="e89eb-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="e89eb-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="e89eb-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e89eb-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e89eb-149">itemType</span><span class="sxs-lookup"><span data-stu-id="e89eb-149">itemType</span></span>|<span data-ttu-id="e89eb-150">String</span><span class="sxs-lookup"><span data-stu-id="e89eb-150">String</span></span>|<span data-ttu-id="e89eb-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="e89eb-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="e89eb-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e89eb-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e89eb-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e89eb-153">displayName</span></span>|<span data-ttu-id="e89eb-154">Строка</span><span class="sxs-lookup"><span data-stu-id="e89eb-154">String</span></span>|<span data-ttu-id="e89eb-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="e89eb-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="e89eb-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e89eb-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="e89eb-157">status</span><span class="sxs-lookup"><span data-stu-id="e89eb-157">status</span></span>|[<span data-ttu-id="e89eb-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="e89eb-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="e89eb-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="e89eb-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="e89eb-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="e89eb-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="e89eb-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e89eb-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="e89eb-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="e89eb-162">errorCode</span></span>|[<span data-ttu-id="e89eb-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="e89eb-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="e89eb-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="e89eb-164">Error code if any occured.</span></span> <span data-ttu-id="e89eb-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="e89eb-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="e89eb-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="e89eb-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="e89eb-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="e89eb-167">guidedDeploymentTags</span></span>|<span data-ttu-id="e89eb-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e89eb-168">String collection</span></span>|<span data-ttu-id="e89eb-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="e89eb-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e89eb-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89eb-170">Response</span></span>
<span data-ttu-id="e89eb-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e89eb-171">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e89eb-172">Пример</span><span class="sxs-lookup"><span data-stu-id="e89eb-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="e89eb-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="e89eb-173">Request</span></span>
<span data-ttu-id="e89eb-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e89eb-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 328

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e89eb-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89eb-175">Response</span></span>
<span data-ttu-id="e89eb-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e89eb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 500

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "id": "850e84d8-84d8-850e-d884-0e85d8840e85",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```



