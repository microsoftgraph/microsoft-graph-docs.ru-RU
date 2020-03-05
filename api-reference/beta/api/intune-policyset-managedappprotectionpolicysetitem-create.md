---
title: Создание Манажедапппротектионполицисетитем
description: Создание нового объекта Манажедапппротектионполицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05e2f903a79b7e51047650b5de603fa925b271a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460915"
---
# <a name="create-managedappprotectionpolicysetitem"></a><span data-ttu-id="fb49a-103">Создание Манажедапппротектионполицисетитем</span><span class="sxs-lookup"><span data-stu-id="fb49a-103">Create managedAppProtectionPolicySetItem</span></span>

<span data-ttu-id="fb49a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fb49a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb49a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb49a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb49a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb49a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb49a-107">Создание нового объекта [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="fb49a-107">Create a new [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb49a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb49a-108">Prerequisites</span></span>
<span data-ttu-id="fb49a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb49a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb49a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb49a-111">Permission type</span></span>|<span data-ttu-id="fb49a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb49a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb49a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb49a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb49a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb49a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb49a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb49a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb49a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb49a-116">Not supported.</span></span>|
|<span data-ttu-id="fb49a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb49a-117">Application</span></span>|<span data-ttu-id="fb49a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb49a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb49a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb49a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="fb49a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb49a-120">Request headers</span></span>
|<span data-ttu-id="fb49a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb49a-121">Header</span></span>|<span data-ttu-id="fb49a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb49a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb49a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb49a-123">Authorization</span></span>|<span data-ttu-id="fb49a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb49a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb49a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb49a-125">Accept</span></span>|<span data-ttu-id="fb49a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb49a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb49a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb49a-127">Request body</span></span>
<span data-ttu-id="fb49a-128">В тексте запроса добавьте представление объекта Манажедапппротектионполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb49a-128">In the request body, supply a JSON representation for the managedAppProtectionPolicySetItem object.</span></span>

<span data-ttu-id="fb49a-129">В следующей таблице приведены свойства, необходимые при создании Манажедапппротектионполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-129">The following table shows the properties that are required when you create the managedAppProtectionPolicySetItem.</span></span>

|<span data-ttu-id="fb49a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb49a-130">Property</span></span>|<span data-ttu-id="fb49a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb49a-131">Type</span></span>|<span data-ttu-id="fb49a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb49a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb49a-133">id</span><span class="sxs-lookup"><span data-stu-id="fb49a-133">id</span></span>|<span data-ttu-id="fb49a-134">String</span><span class="sxs-lookup"><span data-stu-id="fb49a-134">String</span></span>|<span data-ttu-id="fb49a-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="fb49a-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb49a-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fb49a-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb49a-137">createdDateTime</span></span>|<span data-ttu-id="fb49a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb49a-138">DateTimeOffset</span></span>|<span data-ttu-id="fb49a-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="fb49a-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb49a-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fb49a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb49a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="fb49a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb49a-142">DateTimeOffset</span></span>|<span data-ttu-id="fb49a-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="fb49a-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb49a-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fb49a-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="fb49a-145">payloadId</span></span>|<span data-ttu-id="fb49a-146">String</span><span class="sxs-lookup"><span data-stu-id="fb49a-146">String</span></span>|<span data-ttu-id="fb49a-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="fb49a-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb49a-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fb49a-149">itemType</span><span class="sxs-lookup"><span data-stu-id="fb49a-149">itemType</span></span>|<span data-ttu-id="fb49a-150">String</span><span class="sxs-lookup"><span data-stu-id="fb49a-150">String</span></span>|<span data-ttu-id="fb49a-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="fb49a-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb49a-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fb49a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="fb49a-153">displayName</span></span>|<span data-ttu-id="fb49a-154">Строка</span><span class="sxs-lookup"><span data-stu-id="fb49a-154">String</span></span>|<span data-ttu-id="fb49a-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="fb49a-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb49a-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fb49a-157">status</span><span class="sxs-lookup"><span data-stu-id="fb49a-157">status</span></span>|[<span data-ttu-id="fb49a-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="fb49a-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="fb49a-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="fb49a-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="fb49a-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="fb49a-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fb49a-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="fb49a-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="fb49a-162">errorCode</span></span>|[<span data-ttu-id="fb49a-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="fb49a-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="fb49a-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="fb49a-164">Error code if any occured.</span></span> <span data-ttu-id="fb49a-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="fb49a-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="fb49a-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="fb49a-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="fb49a-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="fb49a-167">guidedDeploymentTags</span></span>|<span data-ttu-id="fb49a-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb49a-168">String collection</span></span>|<span data-ttu-id="fb49a-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb49a-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="fb49a-170">таржетедаппманажементлевелс</span><span class="sxs-lookup"><span data-stu-id="fb49a-170">targetedAppManagementLevels</span></span>|<span data-ttu-id="fb49a-171">String</span><span class="sxs-lookup"><span data-stu-id="fb49a-171">String</span></span>|<span data-ttu-id="fb49a-172">Таржетедаппманажементлевелс Манажедаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="fb49a-172">TargetedAppManagementLevels of the ManagedAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="fb49a-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb49a-173">Response</span></span>
<span data-ttu-id="fb49a-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедапппротектионполицисетитем](../resources/intune-policyset-managedappprotectionpolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb49a-174">If successful, this method returns a `201 Created` response code and a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb49a-175">Пример</span><span class="sxs-lookup"><span data-stu-id="fb49a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb49a-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb49a-176">Request</span></span>
<span data-ttu-id="fb49a-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb49a-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
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

### <a name="response"></a><span data-ttu-id="fb49a-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb49a-178">Response</span></span>
<span data-ttu-id="fb49a-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb49a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





