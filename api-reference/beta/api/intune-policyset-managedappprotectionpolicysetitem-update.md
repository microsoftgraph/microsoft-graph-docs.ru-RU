---
title: Обновление Манажедапппротектионполицисетитем
description: Обновление свойств объекта Манажедапппротектионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ce3f1648eb8d7812934dd06ba5bb737285edee8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37192688"
---
# <a name="update-managedappprotectionpolicysetitem"></a><span data-ttu-id="b318f-103">Обновление Манажедапппротектионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="b318f-103">Update managedAppProtectionPolicySetItem</span></span>

> <span data-ttu-id="b318f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b318f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b318f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b318f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b318f-106">Обновление свойств объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b318f-106">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b318f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b318f-107">Prerequisites</span></span>
<span data-ttu-id="b318f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b318f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b318f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b318f-110">Permission type</span></span>|<span data-ttu-id="b318f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b318f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b318f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b318f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b318f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b318f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b318f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b318f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b318f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b318f-115">Not supported.</span></span>|
|<span data-ttu-id="b318f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b318f-116">Application</span></span>|<span data-ttu-id="b318f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b318f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b318f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b318f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="b318f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b318f-119">Request headers</span></span>
|<span data-ttu-id="b318f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b318f-120">Header</span></span>|<span data-ttu-id="b318f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b318f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b318f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b318f-122">Authorization</span></span>|<span data-ttu-id="b318f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b318f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b318f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b318f-124">Accept</span></span>|<span data-ttu-id="b318f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b318f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b318f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b318f-126">Request body</span></span>
<span data-ttu-id="b318f-127">В тексте запроса добавьте представление объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b318f-127">In the request body, supply a JSON representation for the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

<span data-ttu-id="b318f-128">В следующей таблице приведены свойства, необходимые при создании [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b318f-128">The following table shows the properties that are required when you create the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>

|<span data-ttu-id="b318f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b318f-129">Property</span></span>|<span data-ttu-id="b318f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b318f-130">Type</span></span>|<span data-ttu-id="b318f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b318f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b318f-132">id</span><span class="sxs-lookup"><span data-stu-id="b318f-132">id</span></span>|<span data-ttu-id="b318f-133">String</span><span class="sxs-lookup"><span data-stu-id="b318f-133">String</span></span>|<span data-ttu-id="b318f-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="b318f-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b318f-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b318f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b318f-136">createdDateTime</span></span>|<span data-ttu-id="b318f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b318f-137">DateTimeOffset</span></span>|<span data-ttu-id="b318f-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="b318f-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b318f-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b318f-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b318f-140">lastModifiedDateTime</span></span>|<span data-ttu-id="b318f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b318f-141">DateTimeOffset</span></span>|<span data-ttu-id="b318f-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="b318f-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b318f-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b318f-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="b318f-144">payloadId</span></span>|<span data-ttu-id="b318f-145">String.</span><span class="sxs-lookup"><span data-stu-id="b318f-145">String</span></span>|<span data-ttu-id="b318f-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="b318f-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b318f-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b318f-148">itemType</span><span class="sxs-lookup"><span data-stu-id="b318f-148">itemType</span></span>|<span data-ttu-id="b318f-149">String.</span><span class="sxs-lookup"><span data-stu-id="b318f-149">String</span></span>|<span data-ttu-id="b318f-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="b318f-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b318f-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b318f-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b318f-152">displayName</span></span>|<span data-ttu-id="b318f-153">Строка</span><span class="sxs-lookup"><span data-stu-id="b318f-153">String</span></span>|<span data-ttu-id="b318f-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="b318f-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b318f-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b318f-156">status</span><span class="sxs-lookup"><span data-stu-id="b318f-156">status</span></span>|[<span data-ttu-id="b318f-157">полицисетстатус</span><span class="sxs-lookup"><span data-stu-id="b318f-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b318f-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="b318f-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b318f-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b318f-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b318f-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b318f-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="b318f-161">errorCode</span></span>|[<span data-ttu-id="b318f-162">Коде</span><span class="sxs-lookup"><span data-stu-id="b318f-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b318f-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="b318f-163">Error code if any occured.</span></span> <span data-ttu-id="b318f-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="b318f-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="b318f-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b318f-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b318f-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="b318f-166">guidedDeploymentTags</span></span>|<span data-ttu-id="b318f-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b318f-167">String collection</span></span>|<span data-ttu-id="b318f-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b318f-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="b318f-169">таржетедаппманажементлевелс</span><span class="sxs-lookup"><span data-stu-id="b318f-169">targetedAppManagementLevels</span></span>|<span data-ttu-id="b318f-170">String.</span><span class="sxs-lookup"><span data-stu-id="b318f-170">String</span></span>|<span data-ttu-id="b318f-171">Таржетедаппманажементлевелс Манажедаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="b318f-171">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="b318f-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b318f-172">Response</span></span>
<span data-ttu-id="b318f-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b318f-173">If successful, this method returns a `200 OK` response code and an updated [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b318f-174">Пример</span><span class="sxs-lookup"><span data-stu-id="b318f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="b318f-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="b318f-175">Request</span></span>
<span data-ttu-id="b318f-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b318f-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```

### <a name="response"></a><span data-ttu-id="b318f-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="b318f-177">Response</span></span>
<span data-ttu-id="b318f-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b318f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 561

{
  "@odata.type": "#microsoft.graph.managedAppProtectionPolicySetItem",
  "id": "e10d79c9-79c9-e10d-c979-0de1c9790de1",
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
  "targetedAppManagementLevels": "Targeted App Management Levels value"
}
```




