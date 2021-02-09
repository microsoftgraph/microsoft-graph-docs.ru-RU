---
title: Создание mobileAppPolicySetItem
description: Создание объекта mobileAppPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2db884dfec7bf2460b80c30f3fc96155f22e1111
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159320"
---
# <a name="create-mobileapppolicysetitem"></a><span data-ttu-id="1c942-103">Создание mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="1c942-103">Create mobileAppPolicySetItem</span></span>

<span data-ttu-id="1c942-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c942-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c942-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c942-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c942-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c942-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c942-107">Создание объекта [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-107">Create a new [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c942-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c942-108">Prerequisites</span></span>
<span data-ttu-id="1c942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c942-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c942-111">Permission type</span></span>|<span data-ttu-id="1c942-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c942-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c942-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c942-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c942-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c942-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c942-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c942-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c942-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c942-116">Not supported.</span></span>|
|<span data-ttu-id="1c942-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c942-117">Application</span></span>|<span data-ttu-id="1c942-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c942-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c942-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c942-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="1c942-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c942-120">Request headers</span></span>
|<span data-ttu-id="1c942-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c942-121">Header</span></span>|<span data-ttu-id="1c942-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c942-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c942-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c942-123">Authorization</span></span>|<span data-ttu-id="1c942-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c942-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c942-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c942-125">Accept</span></span>|<span data-ttu-id="1c942-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c942-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c942-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c942-127">Request body</span></span>
<span data-ttu-id="1c942-128">В теле запроса укатите представление объекта mobileAppPolicySetItem в JSON.</span><span class="sxs-lookup"><span data-stu-id="1c942-128">In the request body, supply a JSON representation for the mobileAppPolicySetItem object.</span></span>

<span data-ttu-id="1c942-129">В следующей таблице показаны свойства, необходимые при создании объекта mobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-129">The following table shows the properties that are required when you create the mobileAppPolicySetItem.</span></span>

|<span data-ttu-id="1c942-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c942-130">Property</span></span>|<span data-ttu-id="1c942-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c942-131">Type</span></span>|<span data-ttu-id="1c942-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c942-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c942-133">id</span><span class="sxs-lookup"><span data-stu-id="1c942-133">id</span></span>|<span data-ttu-id="1c942-134">String</span><span class="sxs-lookup"><span data-stu-id="1c942-134">String</span></span>|<span data-ttu-id="1c942-135">Ключ MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1c942-136">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c942-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c942-137">createdDateTime</span></span>|<span data-ttu-id="1c942-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c942-138">DateTimeOffset</span></span>|<span data-ttu-id="1c942-139">Время создания policySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="1c942-140">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c942-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c942-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1c942-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c942-142">DateTimeOffset</span></span>|<span data-ttu-id="1c942-143">Время последнего изменения policySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="1c942-144">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c942-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="1c942-145">payloadId</span></span>|<span data-ttu-id="1c942-146">String</span><span class="sxs-lookup"><span data-stu-id="1c942-146">String</span></span>|<span data-ttu-id="1c942-147">PayloadId для PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="1c942-148">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c942-149">itemType</span><span class="sxs-lookup"><span data-stu-id="1c942-149">itemType</span></span>|<span data-ttu-id="1c942-150">String</span><span class="sxs-lookup"><span data-stu-id="1c942-150">String</span></span>|<span data-ttu-id="1c942-151">policySetType для PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="1c942-152">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c942-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1c942-153">displayName</span></span>|<span data-ttu-id="1c942-154">String</span><span class="sxs-lookup"><span data-stu-id="1c942-154">String</span></span>|<span data-ttu-id="1c942-155">DisplayName для PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="1c942-156">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c942-157">status</span><span class="sxs-lookup"><span data-stu-id="1c942-157">status</span></span>|[<span data-ttu-id="1c942-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="1c942-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="1c942-159">Состояние PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="1c942-160">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1c942-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1c942-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1c942-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="1c942-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="1c942-162">errorCode</span></span>|[<span data-ttu-id="1c942-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="1c942-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="1c942-164">Код ошибки, если она произошла.</span><span class="sxs-lookup"><span data-stu-id="1c942-164">Error code if any occured.</span></span> <span data-ttu-id="1c942-165">Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1c942-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1c942-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1c942-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="1c942-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="1c942-167">guidedDeploymentTags</span></span>|<span data-ttu-id="1c942-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1c942-168">String collection</span></span>|<span data-ttu-id="1c942-169">Теги управляемого развертывания. Наследуется [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c942-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c942-170">intent</span><span class="sxs-lookup"><span data-stu-id="1c942-170">intent</span></span>|[<span data-ttu-id="1c942-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="1c942-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1c942-172">Установка намерения MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1c942-173">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1c942-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="1c942-174">settings</span><span class="sxs-lookup"><span data-stu-id="1c942-174">settings</span></span>|[<span data-ttu-id="1c942-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1c942-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="1c942-176">Параметры MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1c942-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="1c942-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c942-177">Response</span></span>
<span data-ttu-id="1c942-178">В случае успеха этот метод возвращает код отклика и объект `201 Created` [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c942-178">If successful, this method returns a `201 Created` response code and a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c942-179">Пример</span><span class="sxs-lookup"><span data-stu-id="1c942-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c942-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c942-180">Request</span></span>
<span data-ttu-id="1c942-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c942-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 540

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```

### <a name="response"></a><span data-ttu-id="1c942-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c942-182">Response</span></span>
<span data-ttu-id="1c942-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c942-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 712

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  }
}
```




