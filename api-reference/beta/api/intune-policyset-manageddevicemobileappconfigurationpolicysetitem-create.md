---
title: Создание Манажеддевицемобилеаппконфигуратионполицисетитем
description: Создание нового объекта Манажеддевицемобилеаппконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 029d98368a18c284be5e4f4a3dfb3c3e8f90dc55
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449930"
---
# <a name="create-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="b4950-103">Создание Манажеддевицемобилеаппконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="b4950-103">Create managedDeviceMobileAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="b4950-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4950-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4950-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4950-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4950-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4950-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4950-107">Создание нового объекта [манажеддевицемобилеаппконфигуратионполицисетитем](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b4950-107">Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4950-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4950-108">Prerequisites</span></span>
<span data-ttu-id="b4950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4950-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4950-111">Permission type</span></span>|<span data-ttu-id="b4950-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4950-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4950-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4950-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4950-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4950-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4950-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4950-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4950-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4950-116">Not supported.</span></span>|
|<span data-ttu-id="b4950-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4950-117">Application</span></span>|<span data-ttu-id="b4950-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4950-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4950-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4950-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="b4950-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4950-120">Request headers</span></span>
|<span data-ttu-id="b4950-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4950-121">Header</span></span>|<span data-ttu-id="b4950-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4950-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4950-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4950-123">Authorization</span></span>|<span data-ttu-id="b4950-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4950-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4950-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4950-125">Accept</span></span>|<span data-ttu-id="b4950-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4950-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4950-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4950-127">Request body</span></span>
<span data-ttu-id="b4950-128">В тексте запроса добавьте представление объекта Манажеддевицемобилеаппконфигуратионполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4950-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="b4950-129">В следующей таблице приведены свойства, необходимые при создании Манажеддевицемобилеаппконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="b4950-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4950-130">Property</span></span>|<span data-ttu-id="b4950-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4950-131">Type</span></span>|<span data-ttu-id="b4950-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4950-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4950-133">id</span><span class="sxs-lookup"><span data-stu-id="b4950-133">id</span></span>|<span data-ttu-id="b4950-134">String</span><span class="sxs-lookup"><span data-stu-id="b4950-134">String</span></span>|<span data-ttu-id="b4950-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b4950-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4950-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b4950-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4950-137">createdDateTime</span></span>|<span data-ttu-id="b4950-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4950-138">DateTimeOffset</span></span>|<span data-ttu-id="b4950-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="b4950-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4950-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b4950-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4950-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b4950-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4950-142">DateTimeOffset</span></span>|<span data-ttu-id="b4950-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="b4950-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4950-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b4950-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="b4950-145">payloadId</span></span>|<span data-ttu-id="b4950-146">String</span><span class="sxs-lookup"><span data-stu-id="b4950-146">String</span></span>|<span data-ttu-id="b4950-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="b4950-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4950-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b4950-149">itemType</span><span class="sxs-lookup"><span data-stu-id="b4950-149">itemType</span></span>|<span data-ttu-id="b4950-150">String</span><span class="sxs-lookup"><span data-stu-id="b4950-150">String</span></span>|<span data-ttu-id="b4950-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="b4950-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4950-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b4950-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b4950-153">displayName</span></span>|<span data-ttu-id="b4950-154">Строка</span><span class="sxs-lookup"><span data-stu-id="b4950-154">String</span></span>|<span data-ttu-id="b4950-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="b4950-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4950-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b4950-157">status</span><span class="sxs-lookup"><span data-stu-id="b4950-157">status</span></span>|[<span data-ttu-id="b4950-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b4950-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b4950-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b4950-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="b4950-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b4950-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b4950-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b4950-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b4950-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="b4950-162">errorCode</span></span>|[<span data-ttu-id="b4950-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="b4950-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b4950-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="b4950-164">Error code if any occured.</span></span> <span data-ttu-id="b4950-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b4950-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b4950-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b4950-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b4950-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="b4950-167">guidedDeploymentTags</span></span>|<span data-ttu-id="b4950-168">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="b4950-168">String collection</span></span>|<span data-ttu-id="b4950-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4950-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b4950-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4950-170">Response</span></span>
<span data-ttu-id="b4950-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажеддевицемобилеаппконфигуратионполицисетитем](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4950-171">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4950-172">Пример</span><span class="sxs-lookup"><span data-stu-id="b4950-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4950-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4950-173">Request</span></span>
<span data-ttu-id="b4950-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4950-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4950-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4950-175">Response</span></span>
<span data-ttu-id="b4950-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4950-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



