---
title: Создание Девицекомплианцеполициполицисетитем
description: Создание нового объекта Девицекомплианцеполициполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4b70ffa4fc3889fd59e3b00faa4503c64e9e54c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49305205"
---
# <a name="create-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="4cfd7-103">Создание Девицекомплианцеполициполицисетитем</span><span class="sxs-lookup"><span data-stu-id="4cfd7-103">Create deviceCompliancePolicyPolicySetItem</span></span>

<span data-ttu-id="4cfd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cfd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cfd7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cfd7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cfd7-107">Создание нового объекта [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="4cfd7-107">Create a new [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cfd7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4cfd7-108">Prerequisites</span></span>
<span data-ttu-id="4cfd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cfd7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cfd7-111">Permission type</span></span>|<span data-ttu-id="4cfd7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cfd7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4cfd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cfd7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cfd7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-116">Not supported.</span></span>|
|<span data-ttu-id="4cfd7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cfd7-117">Application</span></span>|<span data-ttu-id="4cfd7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfd7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cfd7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cfd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="4cfd7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4cfd7-120">Request headers</span></span>
|<span data-ttu-id="4cfd7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cfd7-121">Header</span></span>|<span data-ttu-id="4cfd7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4cfd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cfd7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cfd7-123">Authorization</span></span>|<span data-ttu-id="4cfd7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cfd7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4cfd7-125">Accept</span></span>|<span data-ttu-id="4cfd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cfd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cfd7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cfd7-127">Request body</span></span>
<span data-ttu-id="4cfd7-128">В тексте запроса добавьте представление объекта Девицекомплианцеполициполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-128">In the request body, supply a JSON representation for the deviceCompliancePolicyPolicySetItem object.</span></span>

<span data-ttu-id="4cfd7-129">В следующей таблице приведены свойства, необходимые при создании Девицекомплианцеполициполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-129">The following table shows the properties that are required when you create the deviceCompliancePolicyPolicySetItem.</span></span>

|<span data-ttu-id="4cfd7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cfd7-130">Property</span></span>|<span data-ttu-id="4cfd7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4cfd7-131">Type</span></span>|<span data-ttu-id="4cfd7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4cfd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cfd7-133">id</span><span class="sxs-lookup"><span data-stu-id="4cfd7-133">id</span></span>|<span data-ttu-id="4cfd7-134">String</span><span class="sxs-lookup"><span data-stu-id="4cfd7-134">String</span></span>|<span data-ttu-id="4cfd7-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="4cfd7-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4cfd7-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cfd7-137">createdDateTime</span></span>|<span data-ttu-id="4cfd7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cfd7-138">DateTimeOffset</span></span>|<span data-ttu-id="4cfd7-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="4cfd7-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4cfd7-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cfd7-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4cfd7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cfd7-142">DateTimeOffset</span></span>|<span data-ttu-id="4cfd7-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="4cfd7-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4cfd7-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="4cfd7-145">payloadId</span></span>|<span data-ttu-id="4cfd7-146">String</span><span class="sxs-lookup"><span data-stu-id="4cfd7-146">String</span></span>|<span data-ttu-id="4cfd7-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="4cfd7-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4cfd7-149">itemType</span><span class="sxs-lookup"><span data-stu-id="4cfd7-149">itemType</span></span>|<span data-ttu-id="4cfd7-150">String</span><span class="sxs-lookup"><span data-stu-id="4cfd7-150">String</span></span>|<span data-ttu-id="4cfd7-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="4cfd7-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4cfd7-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4cfd7-153">displayName</span></span>|<span data-ttu-id="4cfd7-154">String</span><span class="sxs-lookup"><span data-stu-id="4cfd7-154">String</span></span>|<span data-ttu-id="4cfd7-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="4cfd7-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="4cfd7-157">status</span><span class="sxs-lookup"><span data-stu-id="4cfd7-157">status</span></span>|[<span data-ttu-id="4cfd7-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="4cfd7-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="4cfd7-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="4cfd7-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="4cfd7-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="4cfd7-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="4cfd7-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="4cfd7-162">errorCode</span></span>|[<span data-ttu-id="4cfd7-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="4cfd7-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="4cfd7-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="4cfd7-164">Error code if any occured.</span></span> <span data-ttu-id="4cfd7-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="4cfd7-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="4cfd7-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="4cfd7-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="4cfd7-167">guidedDeploymentTags</span></span>|<span data-ttu-id="4cfd7-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4cfd7-168">String collection</span></span>|<span data-ttu-id="4cfd7-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cfd7-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4cfd7-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cfd7-170">Response</span></span>
<span data-ttu-id="4cfd7-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-171">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cfd7-172">Пример</span><span class="sxs-lookup"><span data-stu-id="4cfd7-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cfd7-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cfd7-173">Request</span></span>
<span data-ttu-id="4cfd7-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4cfd7-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cfd7-175">Response</span></span>
<span data-ttu-id="4cfd7-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cfd7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




