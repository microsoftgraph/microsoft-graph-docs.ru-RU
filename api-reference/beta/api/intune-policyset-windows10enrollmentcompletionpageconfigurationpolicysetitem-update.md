---
title: Обновление windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Обновление свойств объекта windows10EnrollmentCompletionPageConfigurationPolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c8f4d962baa0ca10b9525f45a415fbf461c0107
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696491"
---
# <a name="update-windows10enrollmentcompletionpageconfigurationpolicysetitem"></a><span data-ttu-id="25c38-103">Обновление windows10EnrollmentCompletionPageConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="25c38-103">Update windows10EnrollmentCompletionPageConfigurationPolicySetItem</span></span>

<span data-ttu-id="25c38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25c38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25c38-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25c38-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25c38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25c38-107">Обновление свойств объекта [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="25c38-107">Update the properties of a [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25c38-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25c38-108">Prerequisites</span></span>
<span data-ttu-id="25c38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25c38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25c38-111">Permission type</span></span>|<span data-ttu-id="25c38-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25c38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25c38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25c38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25c38-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c38-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25c38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25c38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c38-116">Not supported.</span></span>|
|<span data-ttu-id="25c38-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25c38-117">Application</span></span>|<span data-ttu-id="25c38-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c38-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25c38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25c38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="25c38-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25c38-120">Request headers</span></span>
|<span data-ttu-id="25c38-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25c38-121">Header</span></span>|<span data-ttu-id="25c38-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25c38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25c38-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25c38-123">Authorization</span></span>|<span data-ttu-id="25c38-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25c38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25c38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="25c38-125">Accept</span></span>|<span data-ttu-id="25c38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25c38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25c38-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25c38-127">Request body</span></span>
<span data-ttu-id="25c38-128">В тексте запроса добавьте представление объекта [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25c38-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="25c38-129">В следующей таблице приведены свойства, необходимые при создании [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="25c38-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="25c38-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="25c38-130">Property</span></span>|<span data-ttu-id="25c38-131">Тип</span><span class="sxs-lookup"><span data-stu-id="25c38-131">Type</span></span>|<span data-ttu-id="25c38-132">Описание</span><span class="sxs-lookup"><span data-stu-id="25c38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c38-133">id</span><span class="sxs-lookup"><span data-stu-id="25c38-133">id</span></span>|<span data-ttu-id="25c38-134">Строка</span><span class="sxs-lookup"><span data-stu-id="25c38-134">String</span></span>|<span data-ttu-id="25c38-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="25c38-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="25c38-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="25c38-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="25c38-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25c38-137">createdDateTime</span></span>|<span data-ttu-id="25c38-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c38-138">DateTimeOffset</span></span>|<span data-ttu-id="25c38-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="25c38-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="25c38-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="25c38-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="25c38-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25c38-141">lastModifiedDateTime</span></span>|<span data-ttu-id="25c38-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c38-142">DateTimeOffset</span></span>|<span data-ttu-id="25c38-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="25c38-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="25c38-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="25c38-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="25c38-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="25c38-145">payloadId</span></span>|<span data-ttu-id="25c38-146">Строка</span><span class="sxs-lookup"><span data-stu-id="25c38-146">String</span></span>|<span data-ttu-id="25c38-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="25c38-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="25c38-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="25c38-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="25c38-149">itemType</span><span class="sxs-lookup"><span data-stu-id="25c38-149">itemType</span></span>|<span data-ttu-id="25c38-150">Строка</span><span class="sxs-lookup"><span data-stu-id="25c38-150">String</span></span>|<span data-ttu-id="25c38-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="25c38-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="25c38-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="25c38-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="25c38-153">displayName</span><span class="sxs-lookup"><span data-stu-id="25c38-153">displayName</span></span>|<span data-ttu-id="25c38-154">Строка</span><span class="sxs-lookup"><span data-stu-id="25c38-154">String</span></span>|<span data-ttu-id="25c38-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="25c38-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="25c38-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="25c38-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="25c38-157">status</span><span class="sxs-lookup"><span data-stu-id="25c38-157">status</span></span>|[<span data-ttu-id="25c38-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="25c38-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="25c38-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="25c38-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="25c38-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="25c38-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="25c38-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="25c38-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="25c38-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="25c38-162">errorCode</span></span>|[<span data-ttu-id="25c38-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="25c38-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="25c38-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="25c38-164">Error code if any occured.</span></span> <span data-ttu-id="25c38-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="25c38-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="25c38-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="25c38-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="25c38-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="25c38-167">guidedDeploymentTags</span></span>|<span data-ttu-id="25c38-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="25c38-168">String collection</span></span>|<span data-ttu-id="25c38-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="25c38-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="25c38-170">priority</span><span class="sxs-lookup"><span data-stu-id="25c38-170">priority</span></span>|<span data-ttu-id="25c38-171">Int32</span><span class="sxs-lookup"><span data-stu-id="25c38-171">Int32</span></span>|<span data-ttu-id="25c38-172">Приоритет Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="25c38-172">Priority of the Windows10EnrollmentCompletionPageConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="25c38-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="25c38-173">Response</span></span>
<span data-ttu-id="25c38-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25c38-174">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25c38-175">Пример</span><span class="sxs-lookup"><span data-stu-id="25c38-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="25c38-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="25c38-176">Request</span></span>
<span data-ttu-id="25c38-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25c38-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25c38-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c38-178">Response</span></span>
<span data-ttu-id="25c38-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25c38-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





