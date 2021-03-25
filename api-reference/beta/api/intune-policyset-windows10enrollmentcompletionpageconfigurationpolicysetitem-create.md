---
title: Создание windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Создайте новый объект Windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 306e3ee5a583498c2d03886ad2cc1d4d9bc2108a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152315"
---
# <a name="create-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="bc1ea-103">Создание windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="bc1ea-103">Create windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

<span data-ttu-id="bc1ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc1ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc1ea-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc1ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc1ea-107">Создайте [новый объект Windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-107">Create a new [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc1ea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bc1ea-108">Prerequisites</span></span>
<span data-ttu-id="bc1ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc1ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc1ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc1ea-111">Permission type</span></span>|<span data-ttu-id="bc1ea-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc1ea-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc1ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc1ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc1ea-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc1ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-116">Not supported.</span></span>|
|<span data-ttu-id="bc1ea-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bc1ea-117">Application</span></span>|<span data-ttu-id="bc1ea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc1ea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc1ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc1ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="bc1ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bc1ea-120">Request headers</span></span>
|<span data-ttu-id="bc1ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc1ea-121">Header</span></span>|<span data-ttu-id="bc1ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bc1ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc1ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc1ea-123">Authorization</span></span>|<span data-ttu-id="bc1ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc1ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc1ea-125">Accept</span></span>|<span data-ttu-id="bc1ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc1ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc1ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc1ea-127">Request body</span></span>
<span data-ttu-id="bc1ea-128">В корпусе запроса предоставляем представление JSON для объекта Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="bc1ea-129">В следующей таблице показаны свойства, необходимые при создании windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="bc1ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc1ea-130">Property</span></span>|<span data-ttu-id="bc1ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bc1ea-131">Type</span></span>|<span data-ttu-id="bc1ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc1ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc1ea-133">id</span><span class="sxs-lookup"><span data-stu-id="bc1ea-133">id</span></span>|<span data-ttu-id="bc1ea-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bc1ea-134">String</span></span>|<span data-ttu-id="bc1ea-135">Клавиша MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="bc1ea-136">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bc1ea-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc1ea-137">createdDateTime</span></span>|<span data-ttu-id="bc1ea-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc1ea-138">DateTimeOffset</span></span>|<span data-ttu-id="bc1ea-139">Время создания PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="bc1ea-140">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bc1ea-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc1ea-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bc1ea-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc1ea-142">DateTimeOffset</span></span>|<span data-ttu-id="bc1ea-143">Последнее измененное время политикиSetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="bc1ea-144">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bc1ea-145">payloadId</span><span class="sxs-lookup"><span data-stu-id="bc1ea-145">payloadId</span></span>|<span data-ttu-id="bc1ea-146">Строка</span><span class="sxs-lookup"><span data-stu-id="bc1ea-146">String</span></span>|<span data-ttu-id="bc1ea-147">PayloadId of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="bc1ea-148">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bc1ea-149">itemType</span><span class="sxs-lookup"><span data-stu-id="bc1ea-149">itemType</span></span>|<span data-ttu-id="bc1ea-150">Строка</span><span class="sxs-lookup"><span data-stu-id="bc1ea-150">String</span></span>|<span data-ttu-id="bc1ea-151">policySetType policySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="bc1ea-152">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bc1ea-153">displayName</span><span class="sxs-lookup"><span data-stu-id="bc1ea-153">displayName</span></span>|<span data-ttu-id="bc1ea-154">Строка</span><span class="sxs-lookup"><span data-stu-id="bc1ea-154">String</span></span>|<span data-ttu-id="bc1ea-155">DisplayName of the PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="bc1ea-156">Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bc1ea-157">status</span><span class="sxs-lookup"><span data-stu-id="bc1ea-157">status</span></span>|[<span data-ttu-id="bc1ea-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="bc1ea-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="bc1ea-159">Состояние PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="bc1ea-160">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="bc1ea-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="bc1ea-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="bc1ea-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="bc1ea-162">errorCode</span></span>|[<span data-ttu-id="bc1ea-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="bc1ea-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="bc1ea-164">Код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-164">Error code if any occured.</span></span> <span data-ttu-id="bc1ea-165">Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="bc1ea-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="bc1ea-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="bc1ea-167">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="bc1ea-167">guidedDeploymentTags</span></span>|<span data-ttu-id="bc1ea-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bc1ea-168">String collection</span></span>|<span data-ttu-id="bc1ea-169">Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc1ea-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="bc1ea-170">priority</span><span class="sxs-lookup"><span data-stu-id="bc1ea-170">priority</span></span>|<span data-ttu-id="bc1ea-171">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1ea-171">Int32</span></span>|<span data-ttu-id="bc1ea-172">Приоритет Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-172">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="bc1ea-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc1ea-173">Response</span></span>
<span data-ttu-id="bc1ea-174">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект Windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-174">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc1ea-175">Пример</span><span class="sxs-lookup"><span data-stu-id="bc1ea-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc1ea-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc1ea-176">Request</span></span>
<span data-ttu-id="bc1ea-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="bc1ea-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc1ea-178">Response</span></span>
<span data-ttu-id="bc1ea-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc1ea-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




