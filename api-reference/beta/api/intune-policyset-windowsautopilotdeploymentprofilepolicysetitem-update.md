---
title: Обновление Виндовсаутопилотдеплойментпрофилеполицисетитем
description: Обновление свойств объекта Виндовсаутопилотдеплойментпрофилеполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a69ef208d5f90373189c91e1b30f01ed12575fd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460194"
---
# <a name="update-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="9b9b0-103">Обновление Виндовсаутопилотдеплойментпрофилеполицисетитем</span><span class="sxs-lookup"><span data-stu-id="9b9b0-103">Update windowsAutopilotDeploymentProfilePolicySetItem</span></span>

<span data-ttu-id="9b9b0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9b9b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b9b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b9b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b9b0-107">Обновление свойств объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="9b9b0-107">Update the properties of a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b9b0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b9b0-108">Prerequisites</span></span>
<span data-ttu-id="9b9b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b9b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b9b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b9b0-111">Permission type</span></span>|<span data-ttu-id="9b9b0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b9b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b9b0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b9b0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b9b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b9b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-116">Not supported.</span></span>|
|<span data-ttu-id="9b9b0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b9b0-117">Application</span></span>|<span data-ttu-id="9b9b0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b9b0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b9b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b9b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="9b9b0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9b9b0-120">Request headers</span></span>
|<span data-ttu-id="9b9b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b9b0-121">Header</span></span>|<span data-ttu-id="9b9b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b9b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b9b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b9b0-123">Authorization</span></span>|<span data-ttu-id="9b9b0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b9b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b9b0-125">Accept</span></span>|<span data-ttu-id="9b9b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b9b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b9b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b9b0-127">Request body</span></span>
<span data-ttu-id="9b9b0-128">В тексте запроса добавьте представление объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

<span data-ttu-id="9b9b0-129">В следующей таблице приведены свойства, необходимые при создании [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b9b0-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md).</span></span>

|<span data-ttu-id="9b9b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b9b0-130">Property</span></span>|<span data-ttu-id="9b9b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b9b0-131">Type</span></span>|<span data-ttu-id="9b9b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b9b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b9b0-133">id</span><span class="sxs-lookup"><span data-stu-id="9b9b0-133">id</span></span>|<span data-ttu-id="9b9b0-134">String</span><span class="sxs-lookup"><span data-stu-id="9b9b0-134">String</span></span>|<span data-ttu-id="9b9b0-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="9b9b0-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="9b9b0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b9b0-137">createdDateTime</span></span>|<span data-ttu-id="9b9b0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b9b0-138">DateTimeOffset</span></span>|<span data-ttu-id="9b9b0-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="9b9b0-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="9b9b0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b9b0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9b9b0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b9b0-142">DateTimeOffset</span></span>|<span data-ttu-id="9b9b0-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="9b9b0-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="9b9b0-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="9b9b0-145">payloadId</span></span>|<span data-ttu-id="9b9b0-146">String</span><span class="sxs-lookup"><span data-stu-id="9b9b0-146">String</span></span>|<span data-ttu-id="9b9b0-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="9b9b0-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="9b9b0-149">itemType</span><span class="sxs-lookup"><span data-stu-id="9b9b0-149">itemType</span></span>|<span data-ttu-id="9b9b0-150">String</span><span class="sxs-lookup"><span data-stu-id="9b9b0-150">String</span></span>|<span data-ttu-id="9b9b0-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="9b9b0-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="9b9b0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9b9b0-153">displayName</span></span>|<span data-ttu-id="9b9b0-154">Строка</span><span class="sxs-lookup"><span data-stu-id="9b9b0-154">String</span></span>|<span data-ttu-id="9b9b0-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="9b9b0-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="9b9b0-157">status</span><span class="sxs-lookup"><span data-stu-id="9b9b0-157">status</span></span>|[<span data-ttu-id="9b9b0-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="9b9b0-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="9b9b0-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="9b9b0-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b9b0-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="9b9b0-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="9b9b0-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="9b9b0-162">errorCode</span></span>|[<span data-ttu-id="9b9b0-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="9b9b0-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="9b9b0-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="9b9b0-164">Error code if any occured.</span></span> <span data-ttu-id="9b9b0-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b9b0-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="9b9b0-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="9b9b0-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="9b9b0-167">guidedDeploymentTags</span></span>|<span data-ttu-id="9b9b0-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9b9b0-168">String collection</span></span>|<span data-ttu-id="9b9b0-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b9b0-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9b9b0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b9b0-170">Response</span></span>
<span data-ttu-id="9b9b0-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-171">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b9b0-172">Пример</span><span class="sxs-lookup"><span data-stu-id="9b9b0-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b9b0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b9b0-173">Request</span></span>
<span data-ttu-id="9b9b0-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b9b0-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b9b0-175">Response</span></span>
<span data-ttu-id="9b9b0-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b9b0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





