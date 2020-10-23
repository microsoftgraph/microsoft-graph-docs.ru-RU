---
title: Создание Мобилеаппполицисетитем
description: Создание нового объекта Мобилеаппполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e202df2354ee5857c75541925c3f16b775d5aa2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731570"
---
# <a name="create-mobileapppolicysetitem"></a><span data-ttu-id="ccd28-103">Создание Мобилеаппполицисетитем</span><span class="sxs-lookup"><span data-stu-id="ccd28-103">Create mobileAppPolicySetItem</span></span>

<span data-ttu-id="ccd28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccd28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccd28-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccd28-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccd28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd28-107">Создание нового объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ccd28-107">Create a new [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccd28-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ccd28-108">Prerequisites</span></span>
<span data-ttu-id="ccd28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd28-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd28-111">Permission type</span></span>|<span data-ttu-id="ccd28-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccd28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd28-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccd28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd28-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd28-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccd28-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccd28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd28-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd28-116">Not supported.</span></span>|
|<span data-ttu-id="ccd28-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccd28-117">Application</span></span>|<span data-ttu-id="ccd28-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd28-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd28-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccd28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/items
```

## <a name="request-headers"></a><span data-ttu-id="ccd28-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ccd28-120">Request headers</span></span>
|<span data-ttu-id="ccd28-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccd28-121">Header</span></span>|<span data-ttu-id="ccd28-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ccd28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccd28-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccd28-123">Authorization</span></span>|<span data-ttu-id="ccd28-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccd28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccd28-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ccd28-125">Accept</span></span>|<span data-ttu-id="ccd28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccd28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd28-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccd28-127">Request body</span></span>
<span data-ttu-id="ccd28-128">В тексте запроса добавьте представление объекта Мобилеаппполицисетитем в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccd28-128">In the request body, supply a JSON representation for the mobileAppPolicySetItem object.</span></span>

<span data-ttu-id="ccd28-129">В следующей таблице приведены свойства, необходимые при создании Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-129">The following table shows the properties that are required when you create the mobileAppPolicySetItem.</span></span>

|<span data-ttu-id="ccd28-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccd28-130">Property</span></span>|<span data-ttu-id="ccd28-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ccd28-131">Type</span></span>|<span data-ttu-id="ccd28-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd28-133">id</span><span class="sxs-lookup"><span data-stu-id="ccd28-133">id</span></span>|<span data-ttu-id="ccd28-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ccd28-134">String</span></span>|<span data-ttu-id="ccd28-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="ccd28-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccd28-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccd28-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccd28-137">createdDateTime</span></span>|<span data-ttu-id="ccd28-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccd28-138">DateTimeOffset</span></span>|<span data-ttu-id="ccd28-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="ccd28-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccd28-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccd28-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccd28-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ccd28-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccd28-142">DateTimeOffset</span></span>|<span data-ttu-id="ccd28-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="ccd28-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccd28-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccd28-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="ccd28-145">payloadId</span></span>|<span data-ttu-id="ccd28-146">Строка</span><span class="sxs-lookup"><span data-stu-id="ccd28-146">String</span></span>|<span data-ttu-id="ccd28-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="ccd28-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccd28-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccd28-149">itemType</span><span class="sxs-lookup"><span data-stu-id="ccd28-149">itemType</span></span>|<span data-ttu-id="ccd28-150">Строка</span><span class="sxs-lookup"><span data-stu-id="ccd28-150">String</span></span>|<span data-ttu-id="ccd28-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="ccd28-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccd28-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccd28-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ccd28-153">displayName</span></span>|<span data-ttu-id="ccd28-154">Строка</span><span class="sxs-lookup"><span data-stu-id="ccd28-154">String</span></span>|<span data-ttu-id="ccd28-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="ccd28-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccd28-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccd28-157">status</span><span class="sxs-lookup"><span data-stu-id="ccd28-157">status</span></span>|[<span data-ttu-id="ccd28-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="ccd28-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="ccd28-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="ccd28-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="ccd28-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="ccd28-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ccd28-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="ccd28-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="ccd28-162">errorCode</span></span>|[<span data-ttu-id="ccd28-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="ccd28-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="ccd28-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="ccd28-164">Error code if any occured.</span></span> <span data-ttu-id="ccd28-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="ccd28-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="ccd28-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="ccd28-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="ccd28-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="ccd28-167">guidedDeploymentTags</span></span>|<span data-ttu-id="ccd28-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ccd28-168">String collection</span></span>|<span data-ttu-id="ccd28-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="ccd28-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="ccd28-170">intent</span><span class="sxs-lookup"><span data-stu-id="ccd28-170">intent</span></span>|[<span data-ttu-id="ccd28-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="ccd28-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ccd28-172">Установка цели Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="ccd28-173">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ccd28-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ccd28-174">settings</span><span class="sxs-lookup"><span data-stu-id="ccd28-174">settings</span></span>|[<span data-ttu-id="ccd28-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ccd28-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="ccd28-176">Параметры Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="ccd28-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="ccd28-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccd28-177">Response</span></span>
<span data-ttu-id="ccd28-178">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccd28-178">If successful, this method returns a `201 Created` response code and a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd28-179">Пример</span><span class="sxs-lookup"><span data-stu-id="ccd28-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccd28-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccd28-180">Request</span></span>
<span data-ttu-id="ccd28-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccd28-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-type: application/json
Content-length: 514

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
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true
  }
}
```

### <a name="response"></a><span data-ttu-id="ccd28-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd28-182">Response</span></span>
<span data-ttu-id="ccd28-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccd28-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 686

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
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true
  }
}
```





