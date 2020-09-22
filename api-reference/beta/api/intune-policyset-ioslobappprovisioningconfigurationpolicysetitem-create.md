---
title: Создание Иослобапппровисионингконфигуратионполицисетитем
description: Создание нового объекта Иослобапппровисионингконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3ae4eb461d82e96733dd7a2746f61522d570e55
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093506"
---
# <a name="create-ioslobappprovisioningconfigurationpolicysetitem"></a><span data-ttu-id="79da0-103">Создание Иослобапппровисионингконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="79da0-103">Create iosLobAppProvisioningConfigurationPolicySetItem</span></span>

<span data-ttu-id="79da0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79da0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79da0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79da0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79da0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79da0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79da0-107">Создание нового объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="79da0-107">Create a new [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79da0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="79da0-108">Prerequisites</span></span>
<span data-ttu-id="79da0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79da0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79da0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79da0-111">Permission type</span></span>|<span data-ttu-id="79da0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79da0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79da0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79da0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79da0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79da0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79da0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79da0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79da0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79da0-116">Not supported.</span></span>|
|<span data-ttu-id="79da0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79da0-117">Application</span></span>|<span data-ttu-id="79da0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79da0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79da0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79da0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="79da0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="79da0-120">Request headers</span></span>
|<span data-ttu-id="79da0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79da0-121">Header</span></span>|<span data-ttu-id="79da0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="79da0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79da0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79da0-123">Authorization</span></span>|<span data-ttu-id="79da0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79da0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79da0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79da0-125">Accept</span></span>|<span data-ttu-id="79da0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79da0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79da0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79da0-127">Request body</span></span>
<span data-ttu-id="79da0-128">В тексте запроса добавьте представление объекта Иослобапппровисионингконфигуратионполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79da0-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="79da0-129">В следующей таблице приведены свойства, необходимые при создании Иослобапппровисионингконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="79da0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="79da0-130">Property</span></span>|<span data-ttu-id="79da0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="79da0-131">Type</span></span>|<span data-ttu-id="79da0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="79da0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79da0-133">id</span><span class="sxs-lookup"><span data-stu-id="79da0-133">id</span></span>|<span data-ttu-id="79da0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="79da0-134">String</span></span>|<span data-ttu-id="79da0-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="79da0-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="79da0-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="79da0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79da0-137">createdDateTime</span></span>|<span data-ttu-id="79da0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79da0-138">DateTimeOffset</span></span>|<span data-ttu-id="79da0-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="79da0-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="79da0-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="79da0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79da0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="79da0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79da0-142">DateTimeOffset</span></span>|<span data-ttu-id="79da0-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="79da0-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="79da0-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="79da0-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="79da0-145">payloadId</span></span>|<span data-ttu-id="79da0-146">Строка</span><span class="sxs-lookup"><span data-stu-id="79da0-146">String</span></span>|<span data-ttu-id="79da0-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="79da0-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="79da0-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="79da0-149">itemType</span><span class="sxs-lookup"><span data-stu-id="79da0-149">itemType</span></span>|<span data-ttu-id="79da0-150">Строка</span><span class="sxs-lookup"><span data-stu-id="79da0-150">String</span></span>|<span data-ttu-id="79da0-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="79da0-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="79da0-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="79da0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="79da0-153">displayName</span></span>|<span data-ttu-id="79da0-154">Строка</span><span class="sxs-lookup"><span data-stu-id="79da0-154">String</span></span>|<span data-ttu-id="79da0-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="79da0-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="79da0-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="79da0-157">status</span><span class="sxs-lookup"><span data-stu-id="79da0-157">status</span></span>|[<span data-ttu-id="79da0-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="79da0-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="79da0-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="79da0-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="79da0-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="79da0-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="79da0-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="79da0-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="79da0-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="79da0-162">errorCode</span></span>|[<span data-ttu-id="79da0-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="79da0-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="79da0-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="79da0-164">Error code if any occured.</span></span> <span data-ttu-id="79da0-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="79da0-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="79da0-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="79da0-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="79da0-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="79da0-167">guidedDeploymentTags</span></span>|<span data-ttu-id="79da0-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="79da0-168">String collection</span></span>|<span data-ttu-id="79da0-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="79da0-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="79da0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="79da0-170">Response</span></span>
<span data-ttu-id="79da0-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79da0-171">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79da0-172">Пример</span><span class="sxs-lookup"><span data-stu-id="79da0-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="79da0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="79da0-173">Request</span></span>
<span data-ttu-id="79da0-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79da0-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 329

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="79da0-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="79da0-175">Response</span></span>
<span data-ttu-id="79da0-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79da0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 501

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationPolicySetItem",
  "id": "6a978d58-8d58-6a97-588d-976a588d976a",
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






