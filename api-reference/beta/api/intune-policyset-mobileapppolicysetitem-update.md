---
title: Обновление Мобилеаппполицисетитем
description: Обновление свойств объекта Мобилеаппполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a855e37a9cf5b66aedb69cbbaeda3a280ac06728
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44174253"
---
# <a name="update-mobileapppolicysetitem"></a><span data-ttu-id="1c409-103">Обновление Мобилеаппполицисетитем</span><span class="sxs-lookup"><span data-stu-id="1c409-103">Update mobileAppPolicySetItem</span></span>

<span data-ttu-id="1c409-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c409-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c409-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c409-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c409-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c409-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c409-107">Обновление свойств объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="1c409-107">Update the properties of a [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c409-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c409-108">Prerequisites</span></span>
<span data-ttu-id="1c409-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c409-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c409-111">Permission type</span></span>|<span data-ttu-id="1c409-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c409-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c409-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c409-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c409-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c409-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c409-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c409-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c409-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c409-116">Not supported.</span></span>|
|<span data-ttu-id="1c409-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c409-117">Application</span></span>|<span data-ttu-id="1c409-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c409-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c409-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c409-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="1c409-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c409-120">Request headers</span></span>
|<span data-ttu-id="1c409-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c409-121">Header</span></span>|<span data-ttu-id="1c409-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c409-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c409-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c409-123">Authorization</span></span>|<span data-ttu-id="1c409-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c409-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c409-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c409-125">Accept</span></span>|<span data-ttu-id="1c409-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c409-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c409-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c409-127">Request body</span></span>
<span data-ttu-id="1c409-128">В тексте запроса добавьте представление объекта [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c409-128">In the request body, supply a JSON representation for the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

<span data-ttu-id="1c409-129">В следующей таблице приведены свойства, необходимые при создании [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1c409-129">The following table shows the properties that are required when you create the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md).</span></span>

|<span data-ttu-id="1c409-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c409-130">Property</span></span>|<span data-ttu-id="1c409-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c409-131">Type</span></span>|<span data-ttu-id="1c409-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c409-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c409-133">id</span><span class="sxs-lookup"><span data-stu-id="1c409-133">id</span></span>|<span data-ttu-id="1c409-134">String</span><span class="sxs-lookup"><span data-stu-id="1c409-134">String</span></span>|<span data-ttu-id="1c409-135">Ключ Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-135">Key of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1c409-136">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c409-136">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c409-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c409-137">createdDateTime</span></span>|<span data-ttu-id="1c409-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c409-138">DateTimeOffset</span></span>|<span data-ttu-id="1c409-139">Время создания Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-139">Creation time of the PolicySetItem.</span></span> <span data-ttu-id="1c409-140">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c409-140">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c409-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c409-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1c409-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c409-142">DateTimeOffset</span></span>|<span data-ttu-id="1c409-143">Время последнего изменения Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-143">Last modified time of the PolicySetItem.</span></span> <span data-ttu-id="1c409-144">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c409-144">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c409-145">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="1c409-145">payloadId</span></span>|<span data-ttu-id="1c409-146">Строка</span><span class="sxs-lookup"><span data-stu-id="1c409-146">String</span></span>|<span data-ttu-id="1c409-147">Пайлоадид Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-147">PayloadId of the PolicySetItem.</span></span> <span data-ttu-id="1c409-148">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c409-148">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c409-149">itemType</span><span class="sxs-lookup"><span data-stu-id="1c409-149">itemType</span></span>|<span data-ttu-id="1c409-150">Строка</span><span class="sxs-lookup"><span data-stu-id="1c409-150">String</span></span>|<span data-ttu-id="1c409-151">Полицисеттипе Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-151">policySetType of the PolicySetItem.</span></span> <span data-ttu-id="1c409-152">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c409-152">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c409-153">displayName</span><span class="sxs-lookup"><span data-stu-id="1c409-153">displayName</span></span>|<span data-ttu-id="1c409-154">Строка</span><span class="sxs-lookup"><span data-stu-id="1c409-154">String</span></span>|<span data-ttu-id="1c409-155">DisplayName объекта Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-155">DisplayName of the PolicySetItem.</span></span> <span data-ttu-id="1c409-156">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c409-156">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c409-157">status</span><span class="sxs-lookup"><span data-stu-id="1c409-157">status</span></span>|[<span data-ttu-id="1c409-158">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="1c409-158">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="1c409-159">Состояние Полицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-159">Status of the PolicySetItem.</span></span> <span data-ttu-id="1c409-160">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1c409-160">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1c409-161">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1c409-161">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="1c409-162">errorCode</span><span class="sxs-lookup"><span data-stu-id="1c409-162">errorCode</span></span>|[<span data-ttu-id="1c409-163">errorCode</span><span class="sxs-lookup"><span data-stu-id="1c409-163">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="1c409-164">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="1c409-164">Error code if any occured.</span></span> <span data-ttu-id="1c409-165">Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md).</span><span class="sxs-lookup"><span data-stu-id="1c409-165">Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md).</span></span> <span data-ttu-id="1c409-166">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="1c409-166">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="1c409-167">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="1c409-167">guidedDeploymentTags</span></span>|<span data-ttu-id="1c409-168">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="1c409-168">String collection</span></span>|<span data-ttu-id="1c409-169">Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c409-169">Tags of the guided deployment Inherited from [policySetItem](../resources/intune-policyset-policysetitem.md)</span></span>|
|<span data-ttu-id="1c409-170">intent</span><span class="sxs-lookup"><span data-stu-id="1c409-170">intent</span></span>|[<span data-ttu-id="1c409-171">installIntent</span><span class="sxs-lookup"><span data-stu-id="1c409-171">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1c409-172">Установка цели Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-172">Install intent of the MobileAppPolicySetItem.</span></span> <span data-ttu-id="1c409-173">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1c409-173">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="1c409-174">settings</span><span class="sxs-lookup"><span data-stu-id="1c409-174">settings</span></span>|[<span data-ttu-id="1c409-175">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1c409-175">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="1c409-176">Параметры Мобилеаппполицисетитем.</span><span class="sxs-lookup"><span data-stu-id="1c409-176">Settings of the MobileAppPolicySetItem.</span></span>|



## <a name="response"></a><span data-ttu-id="1c409-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c409-177">Response</span></span>
<span data-ttu-id="1c409-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппполицисетитем](../resources/intune-policyset-mobileapppolicysetitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c409-178">If successful, this method returns a `200 OK` response code and an updated [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c409-179">Пример</span><span class="sxs-lookup"><span data-stu-id="1c409-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c409-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c409-180">Request</span></span>
<span data-ttu-id="1c409-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c409-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
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

### <a name="response"></a><span data-ttu-id="1c409-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c409-182">Response</span></span>
<span data-ttu-id="1c409-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c409-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



