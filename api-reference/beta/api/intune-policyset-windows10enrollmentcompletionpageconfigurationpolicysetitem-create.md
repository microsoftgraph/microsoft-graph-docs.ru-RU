---
title: Создание windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Создание нового объекта windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4831b4ebf2bb70d77494cb0a47aea4aaf6e15292
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536268"
---
# <a name="create-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="5c310-103">Создание windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="5c310-103">Create windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

> <span data-ttu-id="5c310-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c310-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c310-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c310-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c310-106">Создание нового объекта [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="5c310-106">Create a new [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c310-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c310-107">Prerequisites</span></span>
<span data-ttu-id="5c310-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c310-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c310-110">Permission type</span></span>|<span data-ttu-id="5c310-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c310-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c310-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c310-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c310-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c310-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c310-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c310-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c310-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c310-115">Not supported.</span></span>|
|<span data-ttu-id="5c310-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5c310-116">Application</span></span>|<span data-ttu-id="5c310-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c310-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c310-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c310-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="5c310-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c310-119">Request headers</span></span>
|<span data-ttu-id="5c310-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c310-120">Header</span></span>|<span data-ttu-id="5c310-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c310-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c310-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c310-122">Authorization</span></span>|<span data-ttu-id="5c310-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c310-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c310-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c310-124">Accept</span></span>|<span data-ttu-id="5c310-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c310-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c310-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c310-126">Request body</span></span>
<span data-ttu-id="5c310-127">В тексте запроса добавьте представление объекта windows10EnrollmentCompletionPageConfigurationPolicySetItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c310-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfigurationPolicySetItem object.</span></span>

<span data-ttu-id="5c310-128">В следующей таблице приведены свойства, необходимые при создании windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="5c310-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>

|<span data-ttu-id="5c310-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c310-129">Property</span></span>|<span data-ttu-id="5c310-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c310-130">Type</span></span>|<span data-ttu-id="5c310-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c310-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c310-132">id</span><span class="sxs-lookup"><span data-stu-id="5c310-132">id</span></span>|<span data-ttu-id="5c310-133">String</span><span class="sxs-lookup"><span data-stu-id="5c310-133">String</span></span>|<span data-ttu-id="5c310-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="5c310-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="5c310-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c310-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="5c310-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c310-136">createdDateTime</span></span>|<span data-ttu-id="5c310-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c310-137">DateTimeOffset</span></span>|<span data-ttu-id="5c310-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="5c310-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="5c310-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c310-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="5c310-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c310-140">lastModifiedDateTime</span></span>|<span data-ttu-id="5c310-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c310-141">DateTimeOffset</span></span>|<span data-ttu-id="5c310-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="5c310-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="5c310-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c310-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="5c310-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="5c310-144">payloadId</span></span>|<span data-ttu-id="5c310-145">String</span><span class="sxs-lookup"><span data-stu-id="5c310-145">String</span></span>|<span data-ttu-id="5c310-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="5c310-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="5c310-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c310-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="5c310-148">itemType</span><span class="sxs-lookup"><span data-stu-id="5c310-148">itemType</span></span>|<span data-ttu-id="5c310-149">String</span><span class="sxs-lookup"><span data-stu-id="5c310-149">String</span></span>|<span data-ttu-id="5c310-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="5c310-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="5c310-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c310-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="5c310-152">displayName</span><span class="sxs-lookup"><span data-stu-id="5c310-152">displayName</span></span>|<span data-ttu-id="5c310-153">Строка</span><span class="sxs-lookup"><span data-stu-id="5c310-153">String</span></span>|<span data-ttu-id="5c310-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="5c310-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="5c310-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c310-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="5c310-156">status</span><span class="sxs-lookup"><span data-stu-id="5c310-156">status</span></span>|[<span data-ttu-id="5c310-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="5c310-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="5c310-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="5c310-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="5c310-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="5c310-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="5c310-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5c310-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="5c310-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="5c310-161">errorCode</span></span>|[<span data-ttu-id="5c310-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="5c310-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="5c310-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="5c310-163">Error code if any occured.</span></span> <span data-ttu-id="5c310-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="5c310-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="5c310-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="5c310-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="5c310-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="5c310-166">guidedDeploymentTags</span></span>|<span data-ttu-id="5c310-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5c310-167">String collection</span></span>|<span data-ttu-id="5c310-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="5c310-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="5c310-169">priority</span><span class="sxs-lookup"><span data-stu-id="5c310-169">priority</span></span>|<span data-ttu-id="5c310-170">Int32</span><span class="sxs-lookup"><span data-stu-id="5c310-170">Int32</span></span>|<span data-ttu-id="5c310-171">Приоритет Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="5c310-171">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="5c310-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c310-172">Response</span></span>
<span data-ttu-id="5c310-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c310-173">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c310-174">Пример</span><span class="sxs-lookup"><span data-stu-id="5c310-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c310-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c310-175">Request</span></span>
<span data-ttu-id="5c310-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c310-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c310-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c310-177">Response</span></span>
<span data-ttu-id="5c310-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c310-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






