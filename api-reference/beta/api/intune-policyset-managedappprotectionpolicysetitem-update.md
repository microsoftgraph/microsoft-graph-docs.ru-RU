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
# <a name="update-managedappprotectionpolicysetitem"></a><span data-ttu-id="cdefb-103">Обновление Манажедапппротектионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="cdefb-103">Update managedAppProtectionPolicySetItem</span></span>

<span data-ttu-id="cdefb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdefb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdefb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdefb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdefb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdefb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdefb-107">Обновление свойств объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="cdefb-107">Update the properties of a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdefb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cdefb-108">Prerequisites</span></span>
<span data-ttu-id="cdefb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdefb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdefb-111">Permission type</span></span>|<span data-ttu-id="cdefb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdefb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdefb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdefb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cdefb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdefb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdefb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdefb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdefb-116">Not supported.</span></span>|
|<span data-ttu-id="cdefb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdefb-117">Application</span></span>|<span data-ttu-id="cdefb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdefb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdefb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdefb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="cdefb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cdefb-120">Request headers</span></span>
|<span data-ttu-id="cdefb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdefb-121">Header</span></span>|<span data-ttu-id="cdefb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cdefb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdefb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdefb-123">Authorization</span></span>|<span data-ttu-id="cdefb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdefb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdefb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cdefb-125">Accept</span></span>|<span data-ttu-id="cdefb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdefb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdefb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cdefb-127">Request body</span></span>
<span data-ttu-id="cdefb-128">В тексте запроса добавьте представление объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdefb-128">In the request body, supply a JSON representation for the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

<span data-ttu-id="cdefb-129">В следующей таблице приведены свойства, необходимые при создании [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="cdefb-129">The following table shows the properties that are required when you create the [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>

|<span data-ttu-id="cdefb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdefb-130">Property</span></span>|<span data-ttu-id="cdefb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cdefb-131">Type</span></span>|<span data-ttu-id="cdefb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cdefb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdefb-133">id</span><span class="sxs-lookup"><span data-stu-id="cdefb-133">id</span></span>|<span data-ttu-id="cdefb-134">String</span><span class="sxs-lookup"><span data-stu-id="cdefb-134">String</span></span>|<span data-ttu-id="cdefb-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="cdefb-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdefb-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="cdefb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdefb-137">createdDateTime</span></span>|<span data-ttu-id="cdefb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdefb-138">DateTimeOffset</span></span>|<span data-ttu-id="cdefb-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="cdefb-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdefb-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="cdefb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdefb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="cdefb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdefb-142">DateTimeOffset</span></span>|<span data-ttu-id="cdefb-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="cdefb-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdefb-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="cdefb-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="cdefb-145">payloadId</span></span>|<span data-ttu-id="cdefb-146">String</span><span class="sxs-lookup"><span data-stu-id="cdefb-146">String</span></span>|<span data-ttu-id="cdefb-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="cdefb-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdefb-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="cdefb-149">itemType</span><span class="sxs-lookup"><span data-stu-id="cdefb-149">itemType</span></span>|<span data-ttu-id="cdefb-150">String</span><span class="sxs-lookup"><span data-stu-id="cdefb-150">String</span></span>|<span data-ttu-id="cdefb-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="cdefb-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdefb-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="cdefb-153">displayName</span><span class="sxs-lookup"><span data-stu-id="cdefb-153">displayName</span></span>|<span data-ttu-id="cdefb-154">Строка</span><span class="sxs-lookup"><span data-stu-id="cdefb-154">String</span></span>|<span data-ttu-id="cdefb-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="cdefb-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdefb-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="cdefb-157">status</span><span class="sxs-lookup"><span data-stu-id="cdefb-157">status</span></span>|[<span data-ttu-id="cdefb-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="cdefb-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="cdefb-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="cdefb-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="cdefb-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="cdefb-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="cdefb-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="cdefb-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="cdefb-162">errorCode</span></span>|[<span data-ttu-id="cdefb-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="cdefb-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="cdefb-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="cdefb-164">Error code if any occured.</span></span> <span data-ttu-id="cdefb-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="cdefb-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="cdefb-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="cdefb-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="cdefb-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="cdefb-167">guidedDeploymentTags</span></span>|<span data-ttu-id="cdefb-168">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="cdefb-168">String collection</span></span>|<span data-ttu-id="cdefb-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="cdefb-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="cdefb-170">таржетедаппманажементлевелс</span><span class="sxs-lookup"><span data-stu-id="cdefb-170">targetedAppManagementLevels</span></span>|<span data-ttu-id="cdefb-171">String</span><span class="sxs-lookup"><span data-stu-id="cdefb-171">String</span></span>|<span data-ttu-id="cdefb-172">Таржетедаппманажементлевелс Манажедаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="cdefb-172">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="cdefb-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdefb-173">Response</span></span>
<span data-ttu-id="cdefb-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdefb-174">If successful, this method returns a `200 OK` response code and an updated [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdefb-175">Пример</span><span class="sxs-lookup"><span data-stu-id="cdefb-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdefb-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdefb-176">Request</span></span>
<span data-ttu-id="cdefb-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdefb-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cdefb-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdefb-178">Response</span></span>
<span data-ttu-id="cdefb-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdefb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



