---
title: Обновление Енроллментрестриктионсконфигуратионполицисетитем
description: Обновление свойств объекта Енроллментрестриктионсконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8fdb6a42022fc00173273b04cbbd0b2506273a6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941164"
---
# <a name="update-enrollmentrestrictionsconfigurationpolicysetitem"></a><span data-ttu-id="f5a2c-103">Обновление Енроллментрестриктионсконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="f5a2c-103">Update enrollmentRestrictionsConfigurationPolicySetItem</span></span>

> <span data-ttu-id="f5a2c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5a2c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5a2c-106">Обновление свойств объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="f5a2c-106">Update the properties of a [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5a2c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f5a2c-107">Prerequisites</span></span>
<span data-ttu-id="f5a2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5a2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5a2c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5a2c-110">Permission type</span></span>|<span data-ttu-id="f5a2c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5a2c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5a2c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5a2c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5a2c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5a2c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-115">Not supported.</span></span>|
|<span data-ttu-id="f5a2c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5a2c-116">Application</span></span>|<span data-ttu-id="f5a2c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5a2c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5a2c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5a2c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="f5a2c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5a2c-119">Request headers</span></span>
|<span data-ttu-id="f5a2c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5a2c-120">Header</span></span>|<span data-ttu-id="f5a2c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f5a2c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5a2c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5a2c-122">Authorization</span></span>|<span data-ttu-id="f5a2c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5a2c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f5a2c-124">Accept</span></span>|<span data-ttu-id="f5a2c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5a2c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5a2c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f5a2c-126">Request body</span></span>
<span data-ttu-id="f5a2c-127">В тексте запроса добавьте представление объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-127">In the request body, supply a JSON representation for the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="f5a2c-128">В следующей таблице приведены свойства, необходимые при создании [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="f5a2c-128">The following table shows the properties that are required when you create the [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="f5a2c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5a2c-129">Property</span></span>|<span data-ttu-id="f5a2c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f5a2c-130">Type</span></span>|<span data-ttu-id="f5a2c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f5a2c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5a2c-132">id</span><span class="sxs-lookup"><span data-stu-id="f5a2c-132">id</span></span>|<span data-ttu-id="f5a2c-133">String</span><span class="sxs-lookup"><span data-stu-id="f5a2c-133">String</span></span>|<span data-ttu-id="f5a2c-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="f5a2c-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f5a2c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5a2c-136">createdDateTime</span></span>|<span data-ttu-id="f5a2c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5a2c-137">DateTimeOffset</span></span>|<span data-ttu-id="f5a2c-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="f5a2c-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f5a2c-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5a2c-140">lastModifiedDateTime</span></span>|<span data-ttu-id="f5a2c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5a2c-141">DateTimeOffset</span></span>|<span data-ttu-id="f5a2c-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="f5a2c-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f5a2c-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="f5a2c-144">payloadId</span></span>|<span data-ttu-id="f5a2c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="f5a2c-145">String</span></span>|<span data-ttu-id="f5a2c-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="f5a2c-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f5a2c-148">itemType</span><span class="sxs-lookup"><span data-stu-id="f5a2c-148">itemType</span></span>|<span data-ttu-id="f5a2c-149">Строка</span><span class="sxs-lookup"><span data-stu-id="f5a2c-149">String</span></span>|<span data-ttu-id="f5a2c-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="f5a2c-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f5a2c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f5a2c-152">displayName</span></span>|<span data-ttu-id="f5a2c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="f5a2c-153">String</span></span>|<span data-ttu-id="f5a2c-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="f5a2c-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f5a2c-156">status</span><span class="sxs-lookup"><span data-stu-id="f5a2c-156">status</span></span>|[<span data-ttu-id="f5a2c-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="f5a2c-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="f5a2c-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="f5a2c-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="f5a2c-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="f5a2c-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="f5a2c-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="f5a2c-161">errorCode</span></span>|[<span data-ttu-id="f5a2c-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="f5a2c-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="f5a2c-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="f5a2c-163">Error code if any occured.</span></span> <span data-ttu-id="f5a2c-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="f5a2c-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="f5a2c-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="f5a2c-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="f5a2c-166">guidedDeploymentTags</span></span>|<span data-ttu-id="f5a2c-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f5a2c-167">String collection</span></span>|<span data-ttu-id="f5a2c-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5a2c-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="f5a2c-169">priority</span><span class="sxs-lookup"><span data-stu-id="f5a2c-169">priority</span></span>|<span data-ttu-id="f5a2c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f5a2c-170">Int32</span></span>|<span data-ttu-id="f5a2c-171">Приоритет Енроллментрестриктионсконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-171">Priority of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|
|<span data-ttu-id="f5a2c-172">limit</span><span class="sxs-lookup"><span data-stu-id="f5a2c-172">limit</span></span>|<span data-ttu-id="f5a2c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="f5a2c-173">Int32</span></span>|<span data-ttu-id="f5a2c-174">Ограничения для Енроллментрестриктионсконфигуратионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-174">Limit of the EnrollmentRestrictionsConfigurationPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="f5a2c-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5a2c-175">Response</span></span>
<span data-ttu-id="f5a2c-176">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-176">If successful, this method returns a `200 OK` response code and an updated [enrollmentRestrictionsConfigurationPolicySetItem](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5a2c-177">Пример</span><span class="sxs-lookup"><span data-stu-id="f5a2c-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5a2c-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5a2c-178">Request</span></span>
<span data-ttu-id="f5a2c-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5a2c-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5a2c-180">Response</span></span>
<span data-ttu-id="f5a2c-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5a2c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





