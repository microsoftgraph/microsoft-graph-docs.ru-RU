---
title: Создание Иослобапппровисионингконфигуратионполицисетитем
description: Создание нового объекта Иослобапппровисионингконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8066d72413206171bd20c37603af3650de3c2b45
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536429"
---
# <a name="create-ioslobappprovisioningconfigurationpolicysetitem"></a><span data-ttu-id="bbb6e-103">Создание Иослобапппровисионингконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="bbb6e-103">Create iosLobAppProvisioningConfigurationPolicySetItem</span></span>

> <span data-ttu-id="bbb6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbb6e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbb6e-106">Создание нового объекта [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="bbb6e-106">Create a new [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbb6e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bbb6e-107">Prerequisites</span></span>
<span data-ttu-id="bbb6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbb6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbb6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbb6e-110">Permission type</span></span>|<span data-ttu-id="bbb6e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbb6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bbb6e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb6e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bbb6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbb6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-115">Not supported.</span></span>|
|<span data-ttu-id="bbb6e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bbb6e-116">Application</span></span>|<span data-ttu-id="bbb6e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbb6e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbb6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbb6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="bbb6e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbb6e-119">Request headers</span></span>
|<span data-ttu-id="bbb6e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbb6e-120">Header</span></span>|<span data-ttu-id="bbb6e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bbb6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbb6e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbb6e-122">Authorization</span></span>|<span data-ttu-id="bbb6e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbb6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bbb6e-124">Accept</span></span>|<span data-ttu-id="bbb6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bbb6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbb6e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbb6e-126">Request body</span></span>
<span data-ttu-id="bbb6e-127">В тексте запроса добавьте представление объекта Иослобапппровисионингконфигуратионполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="bbb6e-128">В следующей таблице приведены свойства, необходимые при создании Иослобапппровисионингконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="bbb6e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbb6e-129">Property</span></span>|<span data-ttu-id="bbb6e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bbb6e-130">Type</span></span>|<span data-ttu-id="bbb6e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bbb6e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbb6e-132">id</span><span class="sxs-lookup"><span data-stu-id="bbb6e-132">id</span></span>|<span data-ttu-id="bbb6e-133">String</span><span class="sxs-lookup"><span data-stu-id="bbb6e-133">String</span></span>|<span data-ttu-id="bbb6e-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="bbb6e-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bbb6e-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbb6e-136">createdDateTime</span></span>|<span data-ttu-id="bbb6e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbb6e-137">DateTimeOffset</span></span>|<span data-ttu-id="bbb6e-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="bbb6e-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bbb6e-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbb6e-140">lastModifiedDateTime</span></span>|<span data-ttu-id="bbb6e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbb6e-141">DateTimeOffset</span></span>|<span data-ttu-id="bbb6e-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="bbb6e-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bbb6e-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="bbb6e-144">payloadId</span></span>|<span data-ttu-id="bbb6e-145">String</span><span class="sxs-lookup"><span data-stu-id="bbb6e-145">String</span></span>|<span data-ttu-id="bbb6e-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="bbb6e-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bbb6e-148">itemType</span><span class="sxs-lookup"><span data-stu-id="bbb6e-148">itemType</span></span>|<span data-ttu-id="bbb6e-149">String</span><span class="sxs-lookup"><span data-stu-id="bbb6e-149">String</span></span>|<span data-ttu-id="bbb6e-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="bbb6e-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bbb6e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="bbb6e-152">displayName</span></span>|<span data-ttu-id="bbb6e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="bbb6e-153">String</span></span>|<span data-ttu-id="bbb6e-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="bbb6e-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bbb6e-156">status</span><span class="sxs-lookup"><span data-stu-id="bbb6e-156">status</span></span>|[<span data-ttu-id="bbb6e-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="bbb6e-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="bbb6e-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="bbb6e-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="bbb6e-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="bbb6e-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="bbb6e-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="bbb6e-161">errorCode</span></span>|[<span data-ttu-id="bbb6e-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="bbb6e-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="bbb6e-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="bbb6e-163">Error code if any occured.</span></span> <span data-ttu-id="bbb6e-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="bbb6e-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="bbb6e-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="bbb6e-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="bbb6e-166">guidedDeploymentTags</span></span>|<span data-ttu-id="bbb6e-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bbb6e-167">String collection</span></span>|<span data-ttu-id="bbb6e-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbb6e-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bbb6e-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbb6e-169">Response</span></span>
<span data-ttu-id="bbb6e-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иослобапппровисионингконфигуратионполицисетитем](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-170">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbb6e-171">Пример</span><span class="sxs-lookup"><span data-stu-id="bbb6e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbb6e-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbb6e-172">Request</span></span>
<span data-ttu-id="bbb6e-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bbb6e-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbb6e-174">Response</span></span>
<span data-ttu-id="bbb6e-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbb6e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






