---
title: Обновление Енроллментрестриктионсконфигуратионполицисетитем
description: Обновление свойств объекта Енроллментрестриктионсконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: acbd34ddc95dd14902ae3ce65532b26386a48c78
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727612"
---
# <a name="update-enrollmentrestrictionsconfigurationpolicysetitem"></a><span data-ttu-id="26156-103">Обновление Енроллментрестриктионсконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="26156-103">Update enrollmentRestrictionsConfigurationPolicySetItem</span></span>

<span data-ttu-id="26156-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26156-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26156-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26156-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26156-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26156-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26156-107">Обновление свойств объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="26156-107">Update the properties of a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26156-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26156-108">Prerequisites</span></span>
<span data-ttu-id="26156-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26156-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26156-111">Permission type</span></span>|<span data-ttu-id="26156-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26156-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26156-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26156-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26156-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26156-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26156-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26156-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26156-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26156-116">Not supported.</span></span>|
|<span data-ttu-id="26156-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26156-117">Application</span></span>|<span data-ttu-id="26156-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26156-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26156-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26156-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="26156-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26156-120">Request headers</span></span>
|<span data-ttu-id="26156-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26156-121">Header</span></span>|<span data-ttu-id="26156-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26156-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26156-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26156-123">Authorization</span></span>|<span data-ttu-id="26156-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26156-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26156-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26156-125">Accept</span></span>|<span data-ttu-id="26156-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26156-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26156-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26156-127">Request body</span></span>
<span data-ttu-id="26156-128">В тексте запроса добавьте представление объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26156-128">In the request body, supply a JSON representation for the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="26156-129">В следующей таблице приведены свойства, необходимые при создании [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="26156-129">The following table shows the properties that are required when you create the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="26156-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26156-130">Property</span></span>|<span data-ttu-id="26156-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26156-131">Type</span></span>|<span data-ttu-id="26156-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26156-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26156-133">id</span><span class="sxs-lookup"><span data-stu-id="26156-133">id</span></span>|<span data-ttu-id="26156-134">Строка</span><span class="sxs-lookup"><span data-stu-id="26156-134">String</span></span>|<span data-ttu-id="26156-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="26156-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="26156-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="26156-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26156-137">createdDateTime</span></span>|<span data-ttu-id="26156-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26156-138">DateTimeOffset</span></span>|<span data-ttu-id="26156-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="26156-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="26156-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="26156-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26156-141">lastModifiedDateTime</span></span>|<span data-ttu-id="26156-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26156-142">DateTimeOffset</span></span>|<span data-ttu-id="26156-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="26156-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="26156-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="26156-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="26156-145">payloadId</span></span>|<span data-ttu-id="26156-146">Строка</span><span class="sxs-lookup"><span data-stu-id="26156-146">String</span></span>|<span data-ttu-id="26156-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="26156-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="26156-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="26156-149">itemType</span><span class="sxs-lookup"><span data-stu-id="26156-149">itemType</span></span>|<span data-ttu-id="26156-150">Строка</span><span class="sxs-lookup"><span data-stu-id="26156-150">String</span></span>|<span data-ttu-id="26156-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="26156-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="26156-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="26156-153">displayName</span><span class="sxs-lookup"><span data-stu-id="26156-153">displayName</span></span>|<span data-ttu-id="26156-154">Строка</span><span class="sxs-lookup"><span data-stu-id="26156-154">String</span></span>|<span data-ttu-id="26156-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="26156-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="26156-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="26156-157">status</span><span class="sxs-lookup"><span data-stu-id="26156-157">status</span></span>|[<span data-ttu-id="26156-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="26156-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="26156-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="26156-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="26156-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="26156-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="26156-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="26156-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="26156-162">errorCode</span></span>|[<span data-ttu-id="26156-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="26156-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="26156-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="26156-164">Error code if any occured.</span></span> <span data-ttu-id="26156-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="26156-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="26156-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="26156-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="26156-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="26156-167">guidedDeploymentTags</span></span>|<span data-ttu-id="26156-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="26156-168">String collection</span></span>|<span data-ttu-id="26156-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="26156-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="26156-170">priority</span><span class="sxs-lookup"><span data-stu-id="26156-170">priority</span></span>|<span data-ttu-id="26156-171">Int32</span><span class="sxs-lookup"><span data-stu-id="26156-171">Int32</span></span>|<span data-ttu-id="26156-172">Приоритет Енроллментрестриктионсконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-172">Priority of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|
|<span data-ttu-id="26156-173">limit</span><span class="sxs-lookup"><span data-stu-id="26156-173">limit</span></span>|<span data-ttu-id="26156-174">Int32</span><span class="sxs-lookup"><span data-stu-id="26156-174">Int32</span></span>|<span data-ttu-id="26156-175">Ограничения для Енроллментрестриктионсконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="26156-175">Limit of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="26156-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="26156-176">Response</span></span>
<span data-ttu-id="26156-177">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26156-177">If successful, this method returns a `200 OK` response code and an updated [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26156-178">Пример</span><span class="sxs-lookup"><span data-stu-id="26156-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="26156-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="26156-179">Request</span></span>
<span data-ttu-id="26156-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26156-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="26156-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="26156-181">Response</span></span>
<span data-ttu-id="26156-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26156-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
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
  "priority": 8,
  "limit": 5
}
```





