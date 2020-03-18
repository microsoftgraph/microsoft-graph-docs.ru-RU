---
title: Обновление windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Обновление свойств объекта windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ec355aaf5c0afce3c4efaaa24511c30dc2c1e36
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801994"
---
# <a name="update-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="caf21-103">Обновление windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="caf21-103">Update windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

> <span data-ttu-id="caf21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="caf21-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="caf21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caf21-106">Обновление свойств объекта [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="caf21-106">Update the properties of a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="caf21-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="caf21-107">Prerequisites</span></span>
<span data-ttu-id="caf21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caf21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caf21-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caf21-110">Permission type</span></span>|<span data-ttu-id="caf21-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="caf21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caf21-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caf21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="caf21-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf21-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="caf21-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caf21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caf21-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf21-115">Not supported.</span></span>|
|<span data-ttu-id="caf21-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="caf21-116">Application</span></span>|<span data-ttu-id="caf21-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf21-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="caf21-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caf21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="caf21-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="caf21-119">Request headers</span></span>
|<span data-ttu-id="caf21-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="caf21-120">Header</span></span>|<span data-ttu-id="caf21-121">Значение</span><span class="sxs-lookup"><span data-stu-id="caf21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caf21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="caf21-122">Authorization</span></span>|<span data-ttu-id="caf21-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caf21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caf21-124">Accept</span><span class="sxs-lookup"><span data-stu-id="caf21-124">Accept</span></span>|<span data-ttu-id="caf21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="caf21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caf21-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="caf21-126">Request body</span></span>
<span data-ttu-id="caf21-127">В тексте запроса добавьте представление объекта [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="caf21-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="caf21-128">В следующей таблице приведены свойства, необходимые при создании [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="caf21-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="caf21-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="caf21-129">Property</span></span>|<span data-ttu-id="caf21-130">Тип</span><span class="sxs-lookup"><span data-stu-id="caf21-130">Type</span></span>|<span data-ttu-id="caf21-131">Описание</span><span class="sxs-lookup"><span data-stu-id="caf21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caf21-132">id</span><span class="sxs-lookup"><span data-stu-id="caf21-132">id</span></span>|<span data-ttu-id="caf21-133">String</span><span class="sxs-lookup"><span data-stu-id="caf21-133">String</span></span>|<span data-ttu-id="caf21-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="caf21-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="caf21-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="caf21-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="caf21-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caf21-136">createdDateTime</span></span>|<span data-ttu-id="caf21-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caf21-137">DateTimeOffset</span></span>|<span data-ttu-id="caf21-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="caf21-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="caf21-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="caf21-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="caf21-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="caf21-140">lastModifiedDateTime</span></span>|<span data-ttu-id="caf21-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caf21-141">DateTimeOffset</span></span>|<span data-ttu-id="caf21-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="caf21-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="caf21-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="caf21-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="caf21-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="caf21-144">payloadId</span></span>|<span data-ttu-id="caf21-145">String</span><span class="sxs-lookup"><span data-stu-id="caf21-145">String</span></span>|<span data-ttu-id="caf21-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="caf21-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="caf21-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="caf21-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="caf21-148">itemType</span><span class="sxs-lookup"><span data-stu-id="caf21-148">itemType</span></span>|<span data-ttu-id="caf21-149">String</span><span class="sxs-lookup"><span data-stu-id="caf21-149">String</span></span>|<span data-ttu-id="caf21-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="caf21-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="caf21-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="caf21-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="caf21-152">displayName</span><span class="sxs-lookup"><span data-stu-id="caf21-152">displayName</span></span>|<span data-ttu-id="caf21-153">Строка</span><span class="sxs-lookup"><span data-stu-id="caf21-153">String</span></span>|<span data-ttu-id="caf21-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="caf21-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="caf21-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="caf21-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="caf21-156">status</span><span class="sxs-lookup"><span data-stu-id="caf21-156">status</span></span>|[<span data-ttu-id="caf21-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="caf21-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="caf21-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="caf21-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="caf21-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="caf21-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="caf21-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="caf21-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="caf21-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="caf21-161">errorCode</span></span>|[<span data-ttu-id="caf21-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="caf21-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="caf21-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="caf21-163">Error code if any occured.</span></span> <span data-ttu-id="caf21-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="caf21-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="caf21-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="caf21-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="caf21-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="caf21-166">guidedDeploymentTags</span></span>|<span data-ttu-id="caf21-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="caf21-167">String collection</span></span>|<span data-ttu-id="caf21-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="caf21-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="caf21-169">priority</span><span class="sxs-lookup"><span data-stu-id="caf21-169">priority</span></span>|<span data-ttu-id="caf21-170">Int32</span><span class="sxs-lookup"><span data-stu-id="caf21-170">Int32</span></span>|<span data-ttu-id="caf21-171">Приоритет Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="caf21-171">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="caf21-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="caf21-172">Response</span></span>
<span data-ttu-id="caf21-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="caf21-173">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caf21-174">Пример</span><span class="sxs-lookup"><span data-stu-id="caf21-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="caf21-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="caf21-175">Request</span></span>
<span data-ttu-id="caf21-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caf21-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="caf21-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="caf21-177">Response</span></span>
<span data-ttu-id="caf21-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="caf21-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "id": "ebfb1dbb-1dbb-ebfb-bb1d-fbebbb1dfbeb",
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
  "priority": 8
}
```




