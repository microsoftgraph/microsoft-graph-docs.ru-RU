---
title: Создание Манажеддевицемобилеаппконфигуратионполицисетитем
description: Создание нового объекта Манажеддевицемобилеаппконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71bd4c91727aff9c74b4f318e7df39d4be0f9890
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941087"
---
# <a name="create-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="515dc-103">Создание Манажеддевицемобилеаппконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="515dc-103">Create managedDeviceMobileAppConfigurationPolicySetItem</span></span>

> <span data-ttu-id="515dc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="515dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="515dc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="515dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="515dc-106">Создание нового объекта [манажеддевицемобилеаппконфигуратионполицисетитем](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="515dc-106">Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="515dc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="515dc-107">Prerequisites</span></span>
<span data-ttu-id="515dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="515dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="515dc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="515dc-110">Permission type</span></span>|<span data-ttu-id="515dc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="515dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="515dc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="515dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="515dc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="515dc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="515dc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="515dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="515dc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="515dc-115">Not supported.</span></span>|
|<span data-ttu-id="515dc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="515dc-116">Application</span></span>|<span data-ttu-id="515dc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="515dc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="515dc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="515dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="515dc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="515dc-119">Request headers</span></span>
|<span data-ttu-id="515dc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="515dc-120">Header</span></span>|<span data-ttu-id="515dc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="515dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="515dc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="515dc-122">Authorization</span></span>|<span data-ttu-id="515dc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="515dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="515dc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="515dc-124">Accept</span></span>|<span data-ttu-id="515dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="515dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="515dc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="515dc-126">Request body</span></span>
<span data-ttu-id="515dc-127">В тексте запроса добавьте представление объекта Манажеддевицемобилеаппконфигуратионполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="515dc-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="515dc-128">В следующей таблице приведены свойства, необходимые при создании Манажеддевицемобилеаппконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="515dc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="515dc-129">Property</span></span>|<span data-ttu-id="515dc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="515dc-130">Type</span></span>|<span data-ttu-id="515dc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="515dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="515dc-132">id</span><span class="sxs-lookup"><span data-stu-id="515dc-132">id</span></span>|<span data-ttu-id="515dc-133">String</span><span class="sxs-lookup"><span data-stu-id="515dc-133">String</span></span>|<span data-ttu-id="515dc-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="515dc-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="515dc-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="515dc-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="515dc-136">createdDateTime</span></span>|<span data-ttu-id="515dc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="515dc-137">DateTimeOffset</span></span>|<span data-ttu-id="515dc-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="515dc-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="515dc-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="515dc-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="515dc-140">lastModifiedDateTime</span></span>|<span data-ttu-id="515dc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="515dc-141">DateTimeOffset</span></span>|<span data-ttu-id="515dc-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="515dc-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="515dc-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="515dc-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="515dc-144">payloadId</span></span>|<span data-ttu-id="515dc-145">Строка</span><span class="sxs-lookup"><span data-stu-id="515dc-145">String</span></span>|<span data-ttu-id="515dc-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="515dc-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="515dc-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="515dc-148">itemType</span><span class="sxs-lookup"><span data-stu-id="515dc-148">itemType</span></span>|<span data-ttu-id="515dc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="515dc-149">String</span></span>|<span data-ttu-id="515dc-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="515dc-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="515dc-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="515dc-152">displayName</span><span class="sxs-lookup"><span data-stu-id="515dc-152">displayName</span></span>|<span data-ttu-id="515dc-153">Строка</span><span class="sxs-lookup"><span data-stu-id="515dc-153">String</span></span>|<span data-ttu-id="515dc-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="515dc-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="515dc-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="515dc-156">status</span><span class="sxs-lookup"><span data-stu-id="515dc-156">status</span></span>|[<span data-ttu-id="515dc-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="515dc-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="515dc-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="515dc-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="515dc-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="515dc-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="515dc-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="515dc-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="515dc-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="515dc-161">errorCode</span></span>|[<span data-ttu-id="515dc-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="515dc-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="515dc-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="515dc-163">Error code if any occured.</span></span> <span data-ttu-id="515dc-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="515dc-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="515dc-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="515dc-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="515dc-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="515dc-166">guidedDeploymentTags</span></span>|<span data-ttu-id="515dc-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="515dc-167">String collection</span></span>|<span data-ttu-id="515dc-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="515dc-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="515dc-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="515dc-169">Response</span></span>
<span data-ttu-id="515dc-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажеддевицемобилеаппконфигуратионполицисетитем](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="515dc-170">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="515dc-171">Пример</span><span class="sxs-lookup"><span data-stu-id="515dc-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="515dc-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="515dc-172">Request</span></span>
<span data-ttu-id="515dc-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="515dc-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 330

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="515dc-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="515dc-174">Response</span></span>
<span data-ttu-id="515dc-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="515dc-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationPolicySetItem",
  "id": "bb065442-5442-bb06-4254-06bb425406bb",
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





