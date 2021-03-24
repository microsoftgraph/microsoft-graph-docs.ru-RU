---
title: Обновление iosLobAppProvisioningConfigurationPolicySetItem
description: Обновление свойств объекта iosLobAppProvisioningConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da31a610291d64666fa41c2265bc60952e4c6003
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141738"
---
# <a name="update-ioslobappprovisioningconfigurationpolicysetitem"></a><span data-ttu-id="dd0e0-103">Обновление iosLobAppProvisioningConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="dd0e0-103">Update iosLobAppProvisioningConfigurationPolicySetItem</span></span>

<span data-ttu-id="dd0e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd0e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd0e0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd0e0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd0e0-107">Обновление свойств объекта [iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-107">Update the properties of a [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd0e0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd0e0-108">Prerequisites</span></span>
<span data-ttu-id="dd0e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd0e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd0e0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd0e0-111">Permission type</span></span>|<span data-ttu-id="dd0e0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd0e0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd0e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd0e0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd0e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-116">Not supported.</span></span>|
|<span data-ttu-id="dd0e0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd0e0-117">Application</span></span>|<span data-ttu-id="dd0e0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd0e0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd0e0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd0e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="dd0e0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd0e0-120">Request headers</span></span>
|<span data-ttu-id="dd0e0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd0e0-121">Header</span></span>|<span data-ttu-id="dd0e0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd0e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd0e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd0e0-123">Authorization</span></span>|<span data-ttu-id="dd0e0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd0e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd0e0-125">Accept</span></span>|<span data-ttu-id="dd0e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd0e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd0e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd0e0-127">Request body</span></span>
<span data-ttu-id="dd0e0-128">В теле запроса поставляем представление JSON для [объекта iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="dd0e0-129">В следующей таблице показаны свойства, необходимые при создании [iosLobAppProvisioningConfigurationPolicySetItem.](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="dd0e0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd0e0-130">Property</span></span>|<span data-ttu-id="dd0e0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd0e0-131">Type</span></span>|<span data-ttu-id="dd0e0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd0e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd0e0-133">id</span><span class="sxs-lookup"><span data-stu-id="dd0e0-133">id</span></span>|<span data-ttu-id="dd0e0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dd0e0-134">String</span></span>|<span data-ttu-id="dd0e0-135">Клавиша MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="dd0e0-136">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dd0e0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd0e0-137">createdDateTime</span></span>|<span data-ttu-id="dd0e0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd0e0-138">DateTimeOffset</span></span>|<span data-ttu-id="dd0e0-139">Время создания PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="dd0e0-140">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dd0e0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd0e0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="dd0e0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd0e0-142">DateTimeOffset</span></span>|<span data-ttu-id="dd0e0-143">Последнее измененное время политикиSetItem.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="dd0e0-144">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dd0e0-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="dd0e0-145">payloadId</span></span>|<span data-ttu-id="dd0e0-146">Строка</span><span class="sxs-lookup"><span data-stu-id="dd0e0-146">String</span></span>|<span data-ttu-id="dd0e0-147">PayloadId of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="dd0e0-148">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dd0e0-149">itemType</span><span class="sxs-lookup"><span data-stu-id="dd0e0-149">itemType</span></span>|<span data-ttu-id="dd0e0-150">Строка</span><span class="sxs-lookup"><span data-stu-id="dd0e0-150">String</span></span>|<span data-ttu-id="dd0e0-151">policySetType policySetItem.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="dd0e0-152">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dd0e0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="dd0e0-153">displayName</span></span>|<span data-ttu-id="dd0e0-154">Строка</span><span class="sxs-lookup"><span data-stu-id="dd0e0-154">String</span></span>|<span data-ttu-id="dd0e0-155">DisplayName of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="dd0e0-156">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="dd0e0-157">status</span><span class="sxs-lookup"><span data-stu-id="dd0e0-157">status</span></span>|[<span data-ttu-id="dd0e0-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="dd0e0-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="dd0e0-159">Состояние PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="dd0e0-160">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="dd0e0-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="dd0e0-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="dd0e0-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="dd0e0-162">errorCode</span></span>|[<span data-ttu-id="dd0e0-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="dd0e0-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="dd0e0-164">Код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-164">Error code if any occured.</span></span> <span data-ttu-id="dd0e0-165">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="dd0e0-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="dd0e0-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="dd0e0-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="dd0e0-167">guidedDeploymentTags</span></span>|<span data-ttu-id="dd0e0-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd0e0-168">String collection</span></span>|<span data-ttu-id="dd0e0-169">Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="dd0e0-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="dd0e0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0e0-170">Response</span></span>
<span data-ttu-id="dd0e0-171">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-171">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationPolicySetItem](../resources/intune-policyset-ioslobappprovisioningconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd0e0-172">Пример</span><span class="sxs-lookup"><span data-stu-id="dd0e0-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd0e0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd0e0-173">Request</span></span>
<span data-ttu-id="dd0e0-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="dd0e0-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd0e0-175">Response</span></span>
<span data-ttu-id="dd0e0-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd0e0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




