---
title: Обновление Манажедапппротектионполицисетитем
description: Обновление свойств объекта Манажедапппротектионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6e4bc9cc9164d9c0d3751f5e8ac43bfc2e23cf6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449953"
---
# <a name="update-managedappprotectionpolicysetitem"></a><span data-ttu-id="6c6e5-103">Обновление Манажедапппротектионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="6c6e5-103">Update managedAppProtectionPolicySetItem</span></span>

<span data-ttu-id="6c6e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c6e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c6e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c6e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c6e5-107">Обновление свойств объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="6c6e5-107">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c6e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c6e5-108">Prerequisites</span></span>
<span data-ttu-id="6c6e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c6e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c6e5-111">Permission type</span></span>|<span data-ttu-id="6c6e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c6e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c6e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c6e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c6e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-116">Not supported.</span></span>|
|<span data-ttu-id="6c6e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c6e5-117">Application</span></span>|<span data-ttu-id="6c6e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c6e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c6e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="6c6e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c6e5-120">Request headers</span></span>
|<span data-ttu-id="6c6e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c6e5-121">Header</span></span>|<span data-ttu-id="6c6e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6c6e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c6e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c6e5-123">Authorization</span></span>|<span data-ttu-id="6c6e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c6e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6c6e5-125">Accept</span></span>|<span data-ttu-id="6c6e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c6e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c6e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c6e5-127">Request body</span></span>
<span data-ttu-id="6c6e5-128">В тексте запроса добавьте представление объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-128">In the request body, supply a JSON representation for the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

<span data-ttu-id="6c6e5-129">В следующей таблице приведены свойства, необходимые при создании [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="6c6e5-129">The following table shows the properties that are required when you create the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>

|<span data-ttu-id="6c6e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c6e5-130">Property</span></span>|<span data-ttu-id="6c6e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6c6e5-131">Type</span></span>|<span data-ttu-id="6c6e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6c6e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c6e5-133">id</span><span class="sxs-lookup"><span data-stu-id="6c6e5-133">id</span></span>|<span data-ttu-id="6c6e5-134">String</span><span class="sxs-lookup"><span data-stu-id="6c6e5-134">String</span></span>|<span data-ttu-id="6c6e5-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="6c6e5-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="6c6e5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c6e5-137">createdDateTime</span></span>|<span data-ttu-id="6c6e5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c6e5-138">DateTimeOffset</span></span>|<span data-ttu-id="6c6e5-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="6c6e5-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="6c6e5-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c6e5-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6c6e5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c6e5-142">DateTimeOffset</span></span>|<span data-ttu-id="6c6e5-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="6c6e5-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="6c6e5-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="6c6e5-145">payloadId</span></span>|<span data-ttu-id="6c6e5-146">String</span><span class="sxs-lookup"><span data-stu-id="6c6e5-146">String</span></span>|<span data-ttu-id="6c6e5-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="6c6e5-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="6c6e5-149">itemType</span><span class="sxs-lookup"><span data-stu-id="6c6e5-149">itemType</span></span>|<span data-ttu-id="6c6e5-150">String</span><span class="sxs-lookup"><span data-stu-id="6c6e5-150">String</span></span>|<span data-ttu-id="6c6e5-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="6c6e5-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="6c6e5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6c6e5-153">displayName</span></span>|<span data-ttu-id="6c6e5-154">Строка</span><span class="sxs-lookup"><span data-stu-id="6c6e5-154">String</span></span>|<span data-ttu-id="6c6e5-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="6c6e5-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="6c6e5-157">status</span><span class="sxs-lookup"><span data-stu-id="6c6e5-157">status</span></span>|[<span data-ttu-id="6c6e5-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="6c6e5-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="6c6e5-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="6c6e5-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="6c6e5-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="6c6e5-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="6c6e5-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="6c6e5-162">errorCode</span></span>|[<span data-ttu-id="6c6e5-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="6c6e5-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="6c6e5-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="6c6e5-164">Error code if any occured.</span></span> <span data-ttu-id="6c6e5-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="6c6e5-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="6c6e5-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="6c6e5-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="6c6e5-167">guidedDeploymentTags</span></span>|<span data-ttu-id="6c6e5-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6c6e5-168">String collection</span></span>|<span data-ttu-id="6c6e5-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c6e5-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="6c6e5-170">таржетедаппманажементлевелс</span><span class="sxs-lookup"><span data-stu-id="6c6e5-170">targetedAppManagementLevels</span></span>|<span data-ttu-id="6c6e5-171">String</span><span class="sxs-lookup"><span data-stu-id="6c6e5-171">String</span></span>|<span data-ttu-id="6c6e5-172">Таржетедаппманажементлевелс Манажедаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-172">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="6c6e5-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c6e5-173">Response</span></span>
<span data-ttu-id="6c6e5-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-174">If successful, this method returns a `200 OK` response code and an updated [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c6e5-175">Пример</span><span class="sxs-lookup"><span data-stu-id="6c6e5-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c6e5-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c6e5-176">Request</span></span>
<span data-ttu-id="6c6e5-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c6e5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c6e5-178">Response</span></span>
<span data-ttu-id="6c6e5-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c6e5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



