---
title: Обновление deviceCompliancePolicyPolicySetItem
description: Обновление свойств объекта deviceCompliancePolicyPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5bf6544c950afdc6521967214eb91799f75ebfb0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145210"
---
# <a name="update-devicecompliancepolicypolicysetitem"></a><span data-ttu-id="1e508-103">Обновление deviceCompliancePolicyPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="1e508-103">Update deviceCompliancePolicyPolicySetItem</span></span>

<span data-ttu-id="1e508-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e508-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e508-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e508-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e508-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e508-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e508-107">Обновление свойств объекта [deviceCompliancePolicyPolicySetItem.](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-107">Update the properties of a [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e508-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1e508-108">Prerequisites</span></span>
<span data-ttu-id="1e508-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e508-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e508-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e508-111">Permission type</span></span>|<span data-ttu-id="1e508-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e508-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e508-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e508-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e508-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e508-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e508-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e508-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e508-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e508-116">Not supported.</span></span>|
|<span data-ttu-id="1e508-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1e508-117">Application</span></span>|<span data-ttu-id="1e508-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e508-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e508-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e508-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="1e508-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1e508-120">Request headers</span></span>
|<span data-ttu-id="1e508-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e508-121">Header</span></span>|<span data-ttu-id="1e508-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1e508-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e508-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e508-123">Authorization</span></span>|<span data-ttu-id="1e508-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e508-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e508-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e508-125">Accept</span></span>|<span data-ttu-id="1e508-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e508-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e508-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e508-127">Request body</span></span>
<span data-ttu-id="1e508-128">В теле запроса поставляем представление JSON для [объекта deviceCompliancePolicyPolicySetItem.](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object.</span></span>

<span data-ttu-id="1e508-129">В следующей таблице показаны свойства, необходимые при создании [устройстваCompliancePolicyPolicySetItem.](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md).</span></span>

|<span data-ttu-id="1e508-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e508-130">Property</span></span>|<span data-ttu-id="1e508-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1e508-131">Type</span></span>|<span data-ttu-id="1e508-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1e508-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e508-133">id</span><span class="sxs-lookup"><span data-stu-id="1e508-133">id</span></span>|<span data-ttu-id="1e508-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1e508-134">String</span></span>|<span data-ttu-id="1e508-135">Клавиша MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1e508-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1e508-136">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1e508-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e508-137">createdDateTime</span></span>|<span data-ttu-id="1e508-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e508-138">DateTimeOffset</span></span>|<span data-ttu-id="1e508-139">Время создания PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1e508-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="1e508-140">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1e508-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e508-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1e508-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e508-142">DateTimeOffset</span></span>|<span data-ttu-id="1e508-143">Последнее измененное время политикиSetItem.</span><span class="sxs-lookup"><span data-stu-id="1e508-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="1e508-144">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1e508-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="1e508-145">payloadId</span></span>|<span data-ttu-id="1e508-146">Строка</span><span class="sxs-lookup"><span data-stu-id="1e508-146">String</span></span>|<span data-ttu-id="1e508-147">PayloadId of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1e508-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="1e508-148">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1e508-149">itemType</span><span class="sxs-lookup"><span data-stu-id="1e508-149">itemType</span></span>|<span data-ttu-id="1e508-150">Строка</span><span class="sxs-lookup"><span data-stu-id="1e508-150">String</span></span>|<span data-ttu-id="1e508-151">policySetType policySetItem.</span><span class="sxs-lookup"><span data-stu-id="1e508-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="1e508-152">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1e508-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1e508-153">displayName</span></span>|<span data-ttu-id="1e508-154">Строка</span><span class="sxs-lookup"><span data-stu-id="1e508-154">String</span></span>|<span data-ttu-id="1e508-155">DisplayName of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1e508-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="1e508-156">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1e508-157">status</span><span class="sxs-lookup"><span data-stu-id="1e508-157">status</span></span>|[<span data-ttu-id="1e508-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="1e508-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="1e508-159">Состояние PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="1e508-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="1e508-160">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1e508-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1e508-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1e508-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="1e508-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="1e508-162">errorCode</span></span>|[<span data-ttu-id="1e508-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="1e508-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="1e508-164">Код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="1e508-164">Error code if any occured.</span></span> <span data-ttu-id="1e508-165">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1e508-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1e508-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1e508-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="1e508-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="1e508-167">guidedDeploymentTags</span></span>|<span data-ttu-id="1e508-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1e508-168">String collection</span></span>|<span data-ttu-id="1e508-169">Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1e508-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1e508-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e508-170">Response</span></span>
<span data-ttu-id="1e508-171">В случае успешного использования этот метод возвращает код отклика и обновленный объект `200 OK` [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1e508-171">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyPolicySetItem](../resources/intune-policyset-devicecompliancepolicypolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e508-172">Пример</span><span class="sxs-lookup"><span data-stu-id="1e508-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e508-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e508-173">Request</span></span>
<span data-ttu-id="1e508-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e508-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="1e508-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e508-175">Response</span></span>
<span data-ttu-id="1e508-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e508-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




