---
title: Создание managedDeviceMobileAppConfigurationPolicySetItem
description: Создание нового объекта managedDeviceMobileAppConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d957acf8e738f4b1ab470cecf9d9b753c56a226e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141731"
---
# <a name="create-manageddevicemobileappconfigurationpolicysetitem"></a><span data-ttu-id="c93b5-103">Создание managedDeviceMobileAppConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="c93b5-103">Create managedDeviceMobileAppConfigurationPolicySetItem</span></span>

<span data-ttu-id="c93b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c93b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c93b5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c93b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c93b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c93b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c93b5-107">Создание нового [объекта managedDeviceMobileAppConfigurationPolicySetItem.](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-107">Create a new [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c93b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c93b5-108">Prerequisites</span></span>
<span data-ttu-id="c93b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c93b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c93b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c93b5-111">Permission type</span></span>|<span data-ttu-id="c93b5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c93b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c93b5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c93b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c93b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c93b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c93b5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c93b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c93b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c93b5-116">Not supported.</span></span>|
|<span data-ttu-id="c93b5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c93b5-117">Application</span></span>|<span data-ttu-id="c93b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c93b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c93b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c93b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="c93b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c93b5-120">Request headers</span></span>
|<span data-ttu-id="c93b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c93b5-121">Header</span></span>|<span data-ttu-id="c93b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c93b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c93b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c93b5-123">Authorization</span></span>|<span data-ttu-id="c93b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c93b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c93b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c93b5-125">Accept</span></span>|<span data-ttu-id="c93b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c93b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c93b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c93b5-127">Request body</span></span>
<span data-ttu-id="c93b5-128">В теле запроса поставляем представление JSON для объекта managedDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="c93b5-129">В следующей таблице показаны свойства, необходимые при создании управляемогоDeviceMobileAppConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="c93b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c93b5-130">Property</span></span>|<span data-ttu-id="c93b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c93b5-131">Type</span></span>|<span data-ttu-id="c93b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c93b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c93b5-133">id</span><span class="sxs-lookup"><span data-stu-id="c93b5-133">id</span></span>|<span data-ttu-id="c93b5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c93b5-134">String</span></span>|<span data-ttu-id="c93b5-135">Клавиша MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="c93b5-136">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c93b5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c93b5-137">createdDateTime</span></span>|<span data-ttu-id="c93b5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c93b5-138">DateTimeOffset</span></span>|<span data-ttu-id="c93b5-139">Время создания PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="c93b5-140">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c93b5-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c93b5-141">lastModifiedDateTime</span></span>|<span data-ttu-id="c93b5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c93b5-142">DateTimeOffset</span></span>|<span data-ttu-id="c93b5-143">Последнее измененное время политикиSetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="c93b5-144">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c93b5-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="c93b5-145">payloadId</span></span>|<span data-ttu-id="c93b5-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c93b5-146">String</span></span>|<span data-ttu-id="c93b5-147">PayloadId of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="c93b5-148">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c93b5-149">itemType</span><span class="sxs-lookup"><span data-stu-id="c93b5-149">itemType</span></span>|<span data-ttu-id="c93b5-150">Строка</span><span class="sxs-lookup"><span data-stu-id="c93b5-150">String</span></span>|<span data-ttu-id="c93b5-151">policySetType policySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="c93b5-152">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c93b5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c93b5-153">displayName</span></span>|<span data-ttu-id="c93b5-154">Строка</span><span class="sxs-lookup"><span data-stu-id="c93b5-154">String</span></span>|<span data-ttu-id="c93b5-155">DisplayName of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="c93b5-156">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="c93b5-157">status</span><span class="sxs-lookup"><span data-stu-id="c93b5-157">status</span></span>|[<span data-ttu-id="c93b5-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="c93b5-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="c93b5-159">Состояние PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="c93b5-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="c93b5-160">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="c93b5-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="c93b5-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c93b5-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="c93b5-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="c93b5-162">errorCode</span></span>|[<span data-ttu-id="c93b5-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="c93b5-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="c93b5-164">Код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="c93b5-164">Error code if any occured.</span></span> <span data-ttu-id="c93b5-165">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="c93b5-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="c93b5-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="c93b5-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="c93b5-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="c93b5-167">guidedDeploymentTags</span></span>|<span data-ttu-id="c93b5-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c93b5-168">String collection</span></span>|<span data-ttu-id="c93b5-169">Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="c93b5-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c93b5-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="c93b5-170">Response</span></span>
<span data-ttu-id="c93b5-171">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c93b5-171">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationPolicySetItem](../resources/intune-policyset-manageddevicemobileappconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c93b5-172">Пример</span><span class="sxs-lookup"><span data-stu-id="c93b5-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="c93b5-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="c93b5-173">Request</span></span>
<span data-ttu-id="c93b5-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c93b5-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c93b5-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="c93b5-175">Response</span></span>
<span data-ttu-id="c93b5-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c93b5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




