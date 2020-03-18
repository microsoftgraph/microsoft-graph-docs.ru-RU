---
title: Обновление Мобилеаппполицисетитем
description: Обновление свойств объекта Мобилеаппполицисетитем.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ac03bc2949b08a70b0413c372a8a522bda3975a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802155"
---
# <a name="update-mobileapppolicysetitem"></a><span data-ttu-id="1fa65-103">Обновление Мобилеаппполицисетитем</span><span class="sxs-lookup"><span data-stu-id="1fa65-103">Update mobileAppPolicySetItem</span></span>

> <span data-ttu-id="1fa65-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fa65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fa65-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fa65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fa65-106">Обновление свойств объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="1fa65-106">Update the properties of a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fa65-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1fa65-107">Prerequisites</span></span>
<span data-ttu-id="1fa65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fa65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fa65-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fa65-110">Permission type</span></span>|<span data-ttu-id="1fa65-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fa65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fa65-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fa65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fa65-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa65-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fa65-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fa65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fa65-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fa65-115">Not supported.</span></span>|
|<span data-ttu-id="1fa65-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1fa65-116">Application</span></span>|<span data-ttu-id="1fa65-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa65-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fa65-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fa65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="1fa65-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fa65-119">Request headers</span></span>
|<span data-ttu-id="1fa65-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fa65-120">Header</span></span>|<span data-ttu-id="1fa65-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1fa65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fa65-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fa65-122">Authorization</span></span>|<span data-ttu-id="1fa65-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fa65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fa65-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1fa65-124">Accept</span></span>|<span data-ttu-id="1fa65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1fa65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fa65-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fa65-126">Request body</span></span>
<span data-ttu-id="1fa65-127">В тексте запроса добавьте представление объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fa65-127">In the request body, supply a JSON representation for the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

<span data-ttu-id="1fa65-128">В следующей таблице приведены свойства, необходимые при создании [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1fa65-128">The following table shows the properties that are required when you create the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).</span></span>

|<span data-ttu-id="1fa65-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fa65-129">Property</span></span>|<span data-ttu-id="1fa65-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1fa65-130">Type</span></span>|<span data-ttu-id="1fa65-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa65-132">id</span><span class="sxs-lookup"><span data-stu-id="1fa65-132">id</span></span>|<span data-ttu-id="1fa65-133">String</span><span class="sxs-lookup"><span data-stu-id="1fa65-133">String</span></span>|<span data-ttu-id="1fa65-134">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-134">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1fa65-135">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1fa65-135">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1fa65-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1fa65-136">createdDateTime</span></span>|<span data-ttu-id="1fa65-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fa65-137">DateTimeOffset</span></span>|<span data-ttu-id="1fa65-138">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-138">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="1fa65-139">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1fa65-139">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1fa65-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1fa65-140">lastModifiedDateTime</span></span>|<span data-ttu-id="1fa65-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fa65-141">DateTimeOffset</span></span>|<span data-ttu-id="1fa65-142">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-142">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="1fa65-143">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1fa65-143">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1fa65-144">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="1fa65-144">payloadId</span></span>|<span data-ttu-id="1fa65-145">String</span><span class="sxs-lookup"><span data-stu-id="1fa65-145">String</span></span>|<span data-ttu-id="1fa65-146">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-146">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="1fa65-147">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1fa65-147">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1fa65-148">itemType</span><span class="sxs-lookup"><span data-stu-id="1fa65-148">itemType</span></span>|<span data-ttu-id="1fa65-149">String</span><span class="sxs-lookup"><span data-stu-id="1fa65-149">String</span></span>|<span data-ttu-id="1fa65-150">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-150">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="1fa65-151">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1fa65-151">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1fa65-152">displayName</span><span class="sxs-lookup"><span data-stu-id="1fa65-152">displayName</span></span>|<span data-ttu-id="1fa65-153">Строка</span><span class="sxs-lookup"><span data-stu-id="1fa65-153">String</span></span>|<span data-ttu-id="1fa65-154">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-154">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="1fa65-155">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1fa65-155">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1fa65-156">status</span><span class="sxs-lookup"><span data-stu-id="1fa65-156">status</span></span>|[<span data-ttu-id="1fa65-157">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="1fa65-157">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="1fa65-158">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-158">Status of the PolicySetItem.</span></span> <span data-ttu-id="1fa65-159">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1fa65-159">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1fa65-160">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1fa65-160">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="1fa65-161">errorCode</span><span class="sxs-lookup"><span data-stu-id="1fa65-161">errorCode</span></span>|[<span data-ttu-id="1fa65-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="1fa65-162">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="1fa65-163">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="1fa65-163">Error code if any occured.</span></span> <span data-ttu-id="1fa65-164">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1fa65-164">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1fa65-165">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1fa65-165">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="1fa65-166">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="1fa65-166">guidedDeploymentTags</span></span>|<span data-ttu-id="1fa65-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1fa65-167">String collection</span></span>|<span data-ttu-id="1fa65-168">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1fa65-168">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1fa65-169">intent</span><span class="sxs-lookup"><span data-stu-id="1fa65-169">intent</span></span>|[<span data-ttu-id="1fa65-170">installIntent</span><span class="sxs-lookup"><span data-stu-id="1fa65-170">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1fa65-171">Установка цели Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-171">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1fa65-172">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1fa65-172">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="1fa65-173">settings</span><span class="sxs-lookup"><span data-stu-id="1fa65-173">settings</span></span>|[<span data-ttu-id="1fa65-174">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1fa65-174">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="1fa65-175">Параметры Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1fa65-175">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="1fa65-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa65-176">Response</span></span>
<span data-ttu-id="1fa65-177">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fa65-177">If successful, this method returns a `200 OK` response code and an updated [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fa65-178">Пример</span><span class="sxs-lookup"><span data-stu-id="1fa65-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fa65-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fa65-179">Request</span></span>
<span data-ttu-id="1fa65-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fa65-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="1fa65-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa65-181">Response</span></span>
<span data-ttu-id="1fa65-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fa65-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
  "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
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
  "intent": "required",
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```




