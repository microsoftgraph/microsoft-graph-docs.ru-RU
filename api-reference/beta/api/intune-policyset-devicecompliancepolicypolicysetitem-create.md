---
title: Создание Девицекомплианцеполициполицисетитем
description: Создание нового объекта Девицекомплианцеполициполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7a81d824ebbab95a7bf5106c732ac3dc0ce5057
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445298"
---
# <a name="create-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="c737b-103">Создание Девицекомплианцеполициполицисетитем</span><span class="sxs-lookup"><span data-stu-id="c737b-103">Create deviceCompliancePolicyPolicySetItem</span></span>

<span data-ttu-id="c737b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c737b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c737b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c737b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c737b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c737b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c737b-107">Создание нового объекта [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="c737b-107">Create a new [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c737b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c737b-108">Prerequisites</span></span>
<span data-ttu-id="c737b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c737b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c737b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c737b-111">Permission type</span></span>|<span data-ttu-id="c737b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c737b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c737b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c737b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c737b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c737b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c737b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c737b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c737b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c737b-116">Not supported.</span></span>|
|<span data-ttu-id="c737b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c737b-117">Application</span></span>|<span data-ttu-id="c737b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c737b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c737b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c737b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="c737b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c737b-120">Request headers</span></span>
|<span data-ttu-id="c737b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c737b-121">Header</span></span>|<span data-ttu-id="c737b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c737b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c737b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c737b-123">Authorization</span></span>|<span data-ttu-id="c737b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c737b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c737b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c737b-125">Accept</span></span>|<span data-ttu-id="c737b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c737b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c737b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c737b-127">Request body</span></span>
<span data-ttu-id="c737b-128">В тексте запроса добавьте представление объекта Девицекомплианцеполициполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c737b-128">In the request body, supply a JSON representation for the deviceCompliancePolicyPolicySetItem object.</span></span>

<span data-ttu-id="c737b-129">В следующей таблице приведены свойства, необходимые при создании Девицекомплианцеполициполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-129">The following table shows the properties that are required when you create the deviceCompliancePolicyPolicySetItem.</span></span>

|<span data-ttu-id="c737b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c737b-130">Property</span></span>|<span data-ttu-id="c737b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c737b-131">Type</span></span>|<span data-ttu-id="c737b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c737b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c737b-133">id</span><span class="sxs-lookup"><span data-stu-id="c737b-133">id</span></span>|<span data-ttu-id="c737b-134">String</span><span class="sxs-lookup"><span data-stu-id="c737b-134">String</span></span>|<span data-ttu-id="c737b-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="c737b-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c737b-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c737b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c737b-137">createdDateTime</span></span>|<span data-ttu-id="c737b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c737b-138">DateTimeOffset</span></span>|<span data-ttu-id="c737b-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="c737b-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c737b-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c737b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c737b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="c737b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c737b-142">DateTimeOffset</span></span>|<span data-ttu-id="c737b-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="c737b-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c737b-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c737b-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="c737b-145">payloadId</span></span>|<span data-ttu-id="c737b-146">String</span><span class="sxs-lookup"><span data-stu-id="c737b-146">String</span></span>|<span data-ttu-id="c737b-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="c737b-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c737b-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c737b-149">itemType</span><span class="sxs-lookup"><span data-stu-id="c737b-149">itemType</span></span>|<span data-ttu-id="c737b-150">String</span><span class="sxs-lookup"><span data-stu-id="c737b-150">String</span></span>|<span data-ttu-id="c737b-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="c737b-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c737b-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c737b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c737b-153">displayName</span></span>|<span data-ttu-id="c737b-154">Строка</span><span class="sxs-lookup"><span data-stu-id="c737b-154">String</span></span>|<span data-ttu-id="c737b-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="c737b-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c737b-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c737b-157">status</span><span class="sxs-lookup"><span data-stu-id="c737b-157">status</span></span>|[<span data-ttu-id="c737b-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="c737b-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="c737b-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="c737b-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="c737b-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="c737b-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="c737b-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c737b-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="c737b-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="c737b-162">errorCode</span></span>|[<span data-ttu-id="c737b-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="c737b-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="c737b-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="c737b-164">Error code if any occured.</span></span> <span data-ttu-id="c737b-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="c737b-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="c737b-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="c737b-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="c737b-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="c737b-167">guidedDeploymentTags</span></span>|<span data-ttu-id="c737b-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c737b-168">String collection</span></span>|<span data-ttu-id="c737b-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c737b-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c737b-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="c737b-170">Response</span></span>
<span data-ttu-id="c737b-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c737b-171">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c737b-172">Пример</span><span class="sxs-lookup"><span data-stu-id="c737b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="c737b-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="c737b-173">Request</span></span>
<span data-ttu-id="c737b-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c737b-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="c737b-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="c737b-175">Response</span></span>
<span data-ttu-id="c737b-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c737b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyPolicySetItem",
  "id": "5c0bc827-c827-5c0b-27c8-0b5c27c80b5c",
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



