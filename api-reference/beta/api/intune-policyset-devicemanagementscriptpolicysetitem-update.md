---
title: Обновление Девицеманажементскриптполицисетитем
description: Обновление свойств объекта Девицеманажементскриптполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09888a7873375b1ffee9626257810509895ee9d9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37192727"
---
# <a name="update-devicemanagementscriptpolicysetitem"></a><span data-ttu-id="33eed-103">Обновление Девицеманажементскриптполицисетитем</span><span class="sxs-lookup"><span data-stu-id="33eed-103">Update deviceManagementScriptPolicySetItem</span></span>

> <span data-ttu-id="33eed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33eed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33eed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33eed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33eed-106">Обновление свойств объекта [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="33eed-106">Update the properties of a [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33eed-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33eed-107">Prerequisites</span></span>
<span data-ttu-id="33eed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33eed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33eed-110">Permission type</span></span>|<span data-ttu-id="33eed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33eed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33eed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33eed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33eed-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33eed-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33eed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33eed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33eed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33eed-115">Not supported.</span></span>|
|<span data-ttu-id="33eed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33eed-116">Application</span></span>|<span data-ttu-id="33eed-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33eed-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33eed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33eed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="33eed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33eed-119">Request headers</span></span>
|<span data-ttu-id="33eed-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33eed-120">Header</span></span>|<span data-ttu-id="33eed-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33eed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33eed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33eed-122">Authorization</span></span>|<span data-ttu-id="33eed-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33eed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33eed-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33eed-124">Accept</span></span>|<span data-ttu-id="33eed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33eed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33eed-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33eed-126">Request body</span></span>
<span data-ttu-id="33eed-127">В тексте запроса добавьте представление объекта [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33eed-127">In the request body, supply a JSON representation for the [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object.</span></span>

<span data-ttu-id="33eed-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="33eed-128">The following table shows the properties that are required when you create the [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md).</span></span>

|<span data-ttu-id="33eed-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="33eed-129">Property</span></span>|<span data-ttu-id="33eed-130">Тип</span><span class="sxs-lookup"><span data-stu-id="33eed-130">Type</span></span>|<span data-ttu-id="33eed-131">Описание</span><span class="sxs-lookup"><span data-stu-id="33eed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33eed-132">id</span><span class="sxs-lookup"><span data-stu-id="33eed-132">id</span></span>|<span data-ttu-id="33eed-133">String</span><span class="sxs-lookup"><span data-stu-id="33eed-133">String</span></span>|<span data-ttu-id="33eed-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="33eed-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="33eed-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33eed-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="33eed-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33eed-136">createdDateTime</span></span>|<span data-ttu-id="33eed-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33eed-137">DateTimeOffset</span></span>|<span data-ttu-id="33eed-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="33eed-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="33eed-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33eed-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="33eed-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33eed-140">lastModifiedDateTime</span></span>|<span data-ttu-id="33eed-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33eed-141">DateTimeOffset</span></span>|<span data-ttu-id="33eed-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="33eed-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="33eed-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33eed-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="33eed-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="33eed-144">payloadId</span></span>|<span data-ttu-id="33eed-145">String.</span><span class="sxs-lookup"><span data-stu-id="33eed-145">String</span></span>|<span data-ttu-id="33eed-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="33eed-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="33eed-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33eed-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="33eed-148">itemType</span><span class="sxs-lookup"><span data-stu-id="33eed-148">itemType</span></span>|<span data-ttu-id="33eed-149">String.</span><span class="sxs-lookup"><span data-stu-id="33eed-149">String</span></span>|<span data-ttu-id="33eed-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="33eed-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="33eed-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33eed-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="33eed-152">displayName</span><span class="sxs-lookup"><span data-stu-id="33eed-152">displayName</span></span>|<span data-ttu-id="33eed-153">Строка</span><span class="sxs-lookup"><span data-stu-id="33eed-153">String</span></span>|<span data-ttu-id="33eed-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="33eed-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="33eed-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33eed-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="33eed-156">status</span><span class="sxs-lookup"><span data-stu-id="33eed-156">status</span></span>|[<span data-ttu-id="33eed-157">полицисетстатус</span><span class="sxs-lookup"><span data-stu-id="33eed-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="33eed-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="33eed-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="33eed-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="33eed-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="33eed-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="33eed-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="33eed-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="33eed-161">errorCode</span></span>|[<span data-ttu-id="33eed-162">Коде</span><span class="sxs-lookup"><span data-stu-id="33eed-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="33eed-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="33eed-163">Error code if any occured.</span></span> <span data-ttu-id="33eed-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="33eed-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="33eed-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="33eed-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="33eed-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="33eed-166">guidedDeploymentTags</span></span>|<span data-ttu-id="33eed-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33eed-167">String collection</span></span>|<span data-ttu-id="33eed-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33eed-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="33eed-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="33eed-169">Response</span></span>
<span data-ttu-id="33eed-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33eed-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33eed-171">Пример</span><span class="sxs-lookup"><span data-stu-id="33eed-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="33eed-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="33eed-172">Request</span></span>
<span data-ttu-id="33eed-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33eed-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="33eed-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="33eed-174">Response</span></span>
<span data-ttu-id="33eed-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33eed-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
  "id": "b6b82c18-2c18-b6b8-182c-b8b6182cb8b6",
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




