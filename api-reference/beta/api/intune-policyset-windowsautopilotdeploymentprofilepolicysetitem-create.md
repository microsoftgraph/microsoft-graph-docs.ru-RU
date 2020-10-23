---
title: Создание Виндовсаутопилотдеплойментпрофилеполицисетитем
description: Создание нового объекта Виндовсаутопилотдеплойментпрофилеполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbe9999551ccfc96df95265145f9275cfce19ad8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731507"
---
# <a name="create-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="020aa-103">Создание Виндовсаутопилотдеплойментпрофилеполицисетитем</span><span class="sxs-lookup"><span data-stu-id="020aa-103">Create windowsAutopilotDeploymentProfilePolicySetItem</span></span>

<span data-ttu-id="020aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="020aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="020aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="020aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="020aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="020aa-107">Создание нового объекта [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="020aa-107">Create a new [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="020aa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="020aa-108">Prerequisites</span></span>
<span data-ttu-id="020aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="020aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="020aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="020aa-111">Permission type</span></span>|<span data-ttu-id="020aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="020aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="020aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="020aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="020aa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="020aa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="020aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="020aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="020aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="020aa-116">Not supported.</span></span>|
|<span data-ttu-id="020aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="020aa-117">Application</span></span>|<span data-ttu-id="020aa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="020aa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="020aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="020aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="020aa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="020aa-120">Request headers</span></span>
|<span data-ttu-id="020aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="020aa-121">Header</span></span>|<span data-ttu-id="020aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="020aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="020aa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="020aa-123">Authorization</span></span>|<span data-ttu-id="020aa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="020aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="020aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="020aa-125">Accept</span></span>|<span data-ttu-id="020aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="020aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="020aa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="020aa-127">Request body</span></span>
<span data-ttu-id="020aa-128">В тексте запроса добавьте представление объекта Виндовсаутопилотдеплойментпрофилеполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="020aa-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfilePolicySetItem object.</span></span>

<span data-ttu-id="020aa-129">В следующей таблице приведены свойства, необходимые при создании Виндовсаутопилотдеплойментпрофилеполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfilePolicySetItem.</span></span>

|<span data-ttu-id="020aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="020aa-130">Property</span></span>|<span data-ttu-id="020aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="020aa-131">Type</span></span>|<span data-ttu-id="020aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="020aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="020aa-133">id</span><span class="sxs-lookup"><span data-stu-id="020aa-133">id</span></span>|<span data-ttu-id="020aa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="020aa-134">String</span></span>|<span data-ttu-id="020aa-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="020aa-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="020aa-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="020aa-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="020aa-137">createdDateTime</span></span>|<span data-ttu-id="020aa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="020aa-138">DateTimeOffset</span></span>|<span data-ttu-id="020aa-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="020aa-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="020aa-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="020aa-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="020aa-141">lastModifiedDateTime</span></span>|<span data-ttu-id="020aa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="020aa-142">DateTimeOffset</span></span>|<span data-ttu-id="020aa-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="020aa-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="020aa-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="020aa-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="020aa-145">payloadId</span></span>|<span data-ttu-id="020aa-146">Строка</span><span class="sxs-lookup"><span data-stu-id="020aa-146">String</span></span>|<span data-ttu-id="020aa-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="020aa-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="020aa-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="020aa-149">itemType</span><span class="sxs-lookup"><span data-stu-id="020aa-149">itemType</span></span>|<span data-ttu-id="020aa-150">Строка</span><span class="sxs-lookup"><span data-stu-id="020aa-150">String</span></span>|<span data-ttu-id="020aa-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="020aa-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="020aa-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="020aa-153">displayName</span><span class="sxs-lookup"><span data-stu-id="020aa-153">displayName</span></span>|<span data-ttu-id="020aa-154">Строка</span><span class="sxs-lookup"><span data-stu-id="020aa-154">String</span></span>|<span data-ttu-id="020aa-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="020aa-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="020aa-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="020aa-157">status</span><span class="sxs-lookup"><span data-stu-id="020aa-157">status</span></span>|[<span data-ttu-id="020aa-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="020aa-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="020aa-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="020aa-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="020aa-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="020aa-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="020aa-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="020aa-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="020aa-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="020aa-162">errorCode</span></span>|[<span data-ttu-id="020aa-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="020aa-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="020aa-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="020aa-164">Error code if any occured.</span></span> <span data-ttu-id="020aa-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="020aa-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="020aa-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="020aa-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="020aa-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="020aa-167">guidedDeploymentTags</span></span>|<span data-ttu-id="020aa-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="020aa-168">String collection</span></span>|<span data-ttu-id="020aa-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="020aa-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="020aa-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="020aa-170">Response</span></span>
<span data-ttu-id="020aa-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсаутопилотдеплойментпрофилеполицисетитем](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="020aa-171">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="020aa-172">Пример</span><span class="sxs-lookup"><span data-stu-id="020aa-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="020aa-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="020aa-173">Request</span></span>
<span data-ttu-id="020aa-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="020aa-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="020aa-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="020aa-175">Response</span></span>
<span data-ttu-id="020aa-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="020aa-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





