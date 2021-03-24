---
title: Обновление mobileAppPolicySetItem
description: Обновление свойств объекта mobileAppPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd98514fcc16dbc413725cb8d597c7d8cc50ae1d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134650"
---
# <a name="update-mobileapppolicysetitem"></a><span data-ttu-id="bafb4-103">Обновление mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="bafb4-103">Update mobileAppPolicySetItem</span></span>

<span data-ttu-id="bafb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bafb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bafb4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bafb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bafb4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bafb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bafb4-107">Обновление свойств объекта [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-107">Update the properties of a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bafb4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bafb4-108">Prerequisites</span></span>
<span data-ttu-id="bafb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bafb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bafb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bafb4-111">Permission type</span></span>|<span data-ttu-id="bafb4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bafb4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bafb4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bafb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bafb4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bafb4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bafb4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bafb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bafb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bafb4-116">Not supported.</span></span>|
|<span data-ttu-id="bafb4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bafb4-117">Application</span></span>|<span data-ttu-id="bafb4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bafb4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bafb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bafb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="bafb4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bafb4-120">Request headers</span></span>
|<span data-ttu-id="bafb4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bafb4-121">Header</span></span>|<span data-ttu-id="bafb4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bafb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bafb4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bafb4-123">Authorization</span></span>|<span data-ttu-id="bafb4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bafb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bafb4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bafb4-125">Accept</span></span>|<span data-ttu-id="bafb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bafb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bafb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bafb4-127">Request body</span></span>
<span data-ttu-id="bafb4-128">В теле запроса поставляем представление JSON для [объекта mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-128">In the request body, supply a JSON representation for the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

<span data-ttu-id="bafb4-129">В следующей таблице показаны свойства, необходимые при создании [mobileAppPolicySetItem.](../resources/intune-policyset-mobileapppolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-129">The following table shows the properties that are required when you create the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).</span></span>

|<span data-ttu-id="bafb4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bafb4-130">Property</span></span>|<span data-ttu-id="bafb4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bafb4-131">Type</span></span>|<span data-ttu-id="bafb4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bafb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bafb4-133">id</span><span class="sxs-lookup"><span data-stu-id="bafb4-133">id</span></span>|<span data-ttu-id="bafb4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bafb4-134">String</span></span>|<span data-ttu-id="bafb4-135">Клавиша MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="bafb4-136">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bafb4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bafb4-137">createdDateTime</span></span>|<span data-ttu-id="bafb4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafb4-138">DateTimeOffset</span></span>|<span data-ttu-id="bafb4-139">Время создания PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="bafb4-140">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bafb4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bafb4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bafb4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafb4-142">DateTimeOffset</span></span>|<span data-ttu-id="bafb4-143">Последнее измененное время политикиSetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="bafb4-144">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bafb4-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="bafb4-145">payloadId</span></span>|<span data-ttu-id="bafb4-146">Строка</span><span class="sxs-lookup"><span data-stu-id="bafb4-146">String</span></span>|<span data-ttu-id="bafb4-147">PayloadId of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="bafb4-148">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bafb4-149">itemType</span><span class="sxs-lookup"><span data-stu-id="bafb4-149">itemType</span></span>|<span data-ttu-id="bafb4-150">Строка</span><span class="sxs-lookup"><span data-stu-id="bafb4-150">String</span></span>|<span data-ttu-id="bafb4-151">policySetType policySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="bafb4-152">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bafb4-153">displayName</span><span class="sxs-lookup"><span data-stu-id="bafb4-153">displayName</span></span>|<span data-ttu-id="bafb4-154">Строка</span><span class="sxs-lookup"><span data-stu-id="bafb4-154">String</span></span>|<span data-ttu-id="bafb4-155">DisplayName of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="bafb4-156">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bafb4-157">status</span><span class="sxs-lookup"><span data-stu-id="bafb4-157">status</span></span>|[<span data-ttu-id="bafb4-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="bafb4-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="bafb4-159">Состояние PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="bafb4-160">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="bafb4-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="bafb4-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bafb4-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="bafb4-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="bafb4-162">errorCode</span></span>|[<span data-ttu-id="bafb4-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="bafb4-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="bafb4-164">Код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="bafb4-164">Error code if any occured.</span></span> <span data-ttu-id="bafb4-165">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="bafb4-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="bafb4-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="bafb4-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="bafb4-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="bafb4-167">guidedDeploymentTags</span></span>|<span data-ttu-id="bafb4-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bafb4-168">String collection</span></span>|<span data-ttu-id="bafb4-169">Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bafb4-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bafb4-170">intent</span><span class="sxs-lookup"><span data-stu-id="bafb4-170">intent</span></span>|[<span data-ttu-id="bafb4-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="bafb4-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="bafb4-172">Установка намерения MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="bafb4-173">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="bafb4-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="bafb4-174">settings</span><span class="sxs-lookup"><span data-stu-id="bafb4-174">settings</span></span>|[<span data-ttu-id="bafb4-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="bafb4-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="bafb4-176">Параметры MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bafb4-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="bafb4-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="bafb4-177">Response</span></span>
<span data-ttu-id="bafb4-178">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bafb4-178">If successful, this method returns a `200 OK` response code and an updated [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bafb4-179">Пример</span><span class="sxs-lookup"><span data-stu-id="bafb4-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="bafb4-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="bafb4-180">Request</span></span>
<span data-ttu-id="bafb4-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bafb4-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="bafb4-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="bafb4-182">Response</span></span>
<span data-ttu-id="bafb4-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bafb4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




