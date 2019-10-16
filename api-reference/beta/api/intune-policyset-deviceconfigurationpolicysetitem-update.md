---
title: Обновление Девицеконфигуратионполицисетитем
description: Обновление свойств объекта Девицеконфигуратионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da9def1dc4c7423bbe31cbf34299768bbf31d941
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537603"
---
# <a name="update-deviceconfigurationpolicysetitem"></a><span data-ttu-id="18969-103">Обновление Девицеконфигуратионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="18969-103">Update deviceConfigurationPolicySetItem</span></span>

> <span data-ttu-id="18969-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18969-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18969-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18969-106">Обновление свойств объекта [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="18969-106">Update the properties of a [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18969-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18969-107">Prerequisites</span></span>
<span data-ttu-id="18969-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18969-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18969-110">Permission type</span></span>|<span data-ttu-id="18969-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18969-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18969-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18969-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18969-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18969-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18969-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18969-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18969-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18969-115">Not supported.</span></span>|
|<span data-ttu-id="18969-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="18969-116">Application</span></span>|<span data-ttu-id="18969-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18969-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18969-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18969-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="18969-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18969-119">Request headers</span></span>
|<span data-ttu-id="18969-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18969-120">Header</span></span>|<span data-ttu-id="18969-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18969-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18969-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18969-122">Authorization</span></span>|<span data-ttu-id="18969-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18969-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18969-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18969-124">Accept</span></span>|<span data-ttu-id="18969-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18969-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18969-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18969-126">Request body</span></span>
<span data-ttu-id="18969-127">В тексте запроса добавьте представление объекта [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18969-127">In the request body, supply a JSON representation for the [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object.</span></span>

<span data-ttu-id="18969-128">В следующей таблице приведены свойства, необходимые при создании [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="18969-128">The following table shows the properties that are required when you create the [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md).</span></span>

|<span data-ttu-id="18969-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18969-129">Property</span></span>|<span data-ttu-id="18969-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18969-130">Type</span></span>|<span data-ttu-id="18969-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18969-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18969-132">id</span><span class="sxs-lookup"><span data-stu-id="18969-132">id</span></span>|<span data-ttu-id="18969-133">String</span><span class="sxs-lookup"><span data-stu-id="18969-133">String</span></span>|<span data-ttu-id="18969-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="18969-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="18969-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="18969-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="18969-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18969-136">createdDateTime</span></span>|<span data-ttu-id="18969-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18969-137">DateTimeOffset</span></span>|<span data-ttu-id="18969-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="18969-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="18969-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="18969-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="18969-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18969-140">lastModifiedDateTime</span></span>|<span data-ttu-id="18969-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18969-141">DateTimeOffset</span></span>|<span data-ttu-id="18969-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="18969-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="18969-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="18969-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="18969-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="18969-144">payloadId</span></span>|<span data-ttu-id="18969-145">String</span><span class="sxs-lookup"><span data-stu-id="18969-145">String</span></span>|<span data-ttu-id="18969-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="18969-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="18969-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="18969-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="18969-148">itemType</span><span class="sxs-lookup"><span data-stu-id="18969-148">itemType</span></span>|<span data-ttu-id="18969-149">String</span><span class="sxs-lookup"><span data-stu-id="18969-149">String</span></span>|<span data-ttu-id="18969-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="18969-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="18969-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="18969-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="18969-152">displayName</span><span class="sxs-lookup"><span data-stu-id="18969-152">displayName</span></span>|<span data-ttu-id="18969-153">Строка</span><span class="sxs-lookup"><span data-stu-id="18969-153">String</span></span>|<span data-ttu-id="18969-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="18969-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="18969-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="18969-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="18969-156">status</span><span class="sxs-lookup"><span data-stu-id="18969-156">status</span></span>|[<span data-ttu-id="18969-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="18969-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="18969-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="18969-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="18969-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="18969-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="18969-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="18969-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="18969-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="18969-161">errorCode</span></span>|[<span data-ttu-id="18969-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="18969-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="18969-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="18969-163">Error code if any occured.</span></span> <span data-ttu-id="18969-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="18969-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="18969-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="18969-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="18969-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="18969-166">guidedDeploymentTags</span></span>|<span data-ttu-id="18969-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="18969-167">String collection</span></span>|<span data-ttu-id="18969-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="18969-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|



## <a name="response"></a><span data-ttu-id="18969-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="18969-169">Response</span></span>
<span data-ttu-id="18969-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18969-170">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18969-171">Пример</span><span class="sxs-lookup"><span data-stu-id="18969-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="18969-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="18969-172">Request</span></span>
<span data-ttu-id="18969-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18969-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
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

### <a name="response"></a><span data-ttu-id="18969-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="18969-174">Response</span></span>
<span data-ttu-id="18969-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18969-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
  "id": "00b1197c-197c-00b1-7c19-b1007c19b100",
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






