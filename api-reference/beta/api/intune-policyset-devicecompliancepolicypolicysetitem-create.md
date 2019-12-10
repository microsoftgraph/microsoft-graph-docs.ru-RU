---
title: Создание Девицекомплианцеполициполицисетитем
description: Создание нового объекта Девицекомплианцеполициполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a0a9e93750ae1512049e6a6f451016b01311877
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941297"
---
# <a name="create-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="77f82-103">Создание Девицекомплианцеполициполицисетитем</span><span class="sxs-lookup"><span data-stu-id="77f82-103">Create deviceCompliancePolicyPolicySetItem</span></span>

> <span data-ttu-id="77f82-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77f82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77f82-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f82-106">Создание нового объекта [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="77f82-106">Create a new [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77f82-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77f82-107">Prerequisites</span></span>
<span data-ttu-id="77f82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f82-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77f82-110">Permission type</span></span>|<span data-ttu-id="77f82-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77f82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77f82-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77f82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77f82-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f82-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77f82-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77f82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77f82-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77f82-115">Not supported.</span></span>|
|<span data-ttu-id="77f82-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77f82-116">Application</span></span>|<span data-ttu-id="77f82-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f82-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77f82-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77f82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="77f82-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77f82-119">Request headers</span></span>
|<span data-ttu-id="77f82-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77f82-120">Header</span></span>|<span data-ttu-id="77f82-121">Значение</span><span class="sxs-lookup"><span data-stu-id="77f82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77f82-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77f82-122">Authorization</span></span>|<span data-ttu-id="77f82-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77f82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77f82-124">Accept</span><span class="sxs-lookup"><span data-stu-id="77f82-124">Accept</span></span>|<span data-ttu-id="77f82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77f82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77f82-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77f82-126">Request body</span></span>
<span data-ttu-id="77f82-127">В тексте запроса добавьте представление объекта Девицекомплианцеполициполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77f82-127">In the request body, supply a JSON representation for the deviceCompliancePolicyPolicySetItem object.</span></span>

<span data-ttu-id="77f82-128">В следующей таблице приведены свойства, необходимые при создании Девицекомплианцеполициполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-128">The following table shows the properties that are required when you create the deviceCompliancePolicyPolicySetItem.</span></span>

|<span data-ttu-id="77f82-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="77f82-129">Property</span></span>|<span data-ttu-id="77f82-130">Тип</span><span class="sxs-lookup"><span data-stu-id="77f82-130">Type</span></span>|<span data-ttu-id="77f82-131">Описание</span><span class="sxs-lookup"><span data-stu-id="77f82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f82-132">id</span><span class="sxs-lookup"><span data-stu-id="77f82-132">id</span></span>|<span data-ttu-id="77f82-133">String</span><span class="sxs-lookup"><span data-stu-id="77f82-133">String</span></span>|<span data-ttu-id="77f82-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="77f82-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="77f82-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="77f82-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77f82-136">createdDateTime</span></span>|<span data-ttu-id="77f82-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f82-137">DateTimeOffset</span></span>|<span data-ttu-id="77f82-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="77f82-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="77f82-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="77f82-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77f82-140">lastModifiedDateTime</span></span>|<span data-ttu-id="77f82-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f82-141">DateTimeOffset</span></span>|<span data-ttu-id="77f82-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="77f82-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="77f82-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="77f82-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="77f82-144">payloadId</span></span>|<span data-ttu-id="77f82-145">Строка</span><span class="sxs-lookup"><span data-stu-id="77f82-145">String</span></span>|<span data-ttu-id="77f82-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="77f82-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="77f82-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="77f82-148">itemType</span><span class="sxs-lookup"><span data-stu-id="77f82-148">itemType</span></span>|<span data-ttu-id="77f82-149">Строка</span><span class="sxs-lookup"><span data-stu-id="77f82-149">String</span></span>|<span data-ttu-id="77f82-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="77f82-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="77f82-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="77f82-152">displayName</span><span class="sxs-lookup"><span data-stu-id="77f82-152">displayName</span></span>|<span data-ttu-id="77f82-153">Строка</span><span class="sxs-lookup"><span data-stu-id="77f82-153">String</span></span>|<span data-ttu-id="77f82-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="77f82-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="77f82-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="77f82-156">status</span><span class="sxs-lookup"><span data-stu-id="77f82-156">status</span></span>|[<span data-ttu-id="77f82-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="77f82-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="77f82-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="77f82-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="77f82-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="77f82-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="77f82-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="77f82-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="77f82-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="77f82-161">errorCode</span></span>|[<span data-ttu-id="77f82-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="77f82-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="77f82-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="77f82-163">Error code if any occured.</span></span> <span data-ttu-id="77f82-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="77f82-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="77f82-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="77f82-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="77f82-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="77f82-166">guidedDeploymentTags</span></span>|<span data-ttu-id="77f82-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="77f82-167">String collection</span></span>|<span data-ttu-id="77f82-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="77f82-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="77f82-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="77f82-169">Response</span></span>
<span data-ttu-id="77f82-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицекомплианцеполициполицисетитем](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77f82-170">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77f82-171">Пример</span><span class="sxs-lookup"><span data-stu-id="77f82-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="77f82-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="77f82-172">Request</span></span>
<span data-ttu-id="77f82-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77f82-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77f82-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="77f82-174">Response</span></span>
<span data-ttu-id="77f82-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77f82-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





