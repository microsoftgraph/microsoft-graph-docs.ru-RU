---
title: Создание Импортедаппледевицеидентитиресулт
description: Создание нового объекта Импортедаппледевицеидентитиресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fb0493c1b693ddb72b648311a9e329e38420a75
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185030"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="2a37d-103">Создание Импортедаппледевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="2a37d-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="2a37d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a37d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a37d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a37d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a37d-106">Создание нового объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="2a37d-106">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a37d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2a37d-107">Prerequisites</span></span>
<span data-ttu-id="2a37d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a37d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a37d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a37d-110">Permission type</span></span>|<span data-ttu-id="2a37d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a37d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a37d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a37d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a37d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a37d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a37d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a37d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a37d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a37d-115">Not supported.</span></span>|
|<span data-ttu-id="2a37d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a37d-116">Application</span></span>|<span data-ttu-id="2a37d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a37d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a37d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a37d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="2a37d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a37d-119">Request headers</span></span>
|<span data-ttu-id="2a37d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a37d-120">Header</span></span>|<span data-ttu-id="2a37d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2a37d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a37d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a37d-122">Authorization</span></span>|<span data-ttu-id="2a37d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a37d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a37d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2a37d-124">Accept</span></span>|<span data-ttu-id="2a37d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a37d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a37d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a37d-126">Request body</span></span>
<span data-ttu-id="2a37d-127">В тексте запроса добавьте представление объекта Импортедаппледевицеидентитиресулт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a37d-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="2a37d-128">В следующей таблице приведены свойства, необходимые при создании Импортедаппледевицеидентитиресулт.</span><span class="sxs-lookup"><span data-stu-id="2a37d-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="2a37d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a37d-129">Property</span></span>|<span data-ttu-id="2a37d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a37d-130">Type</span></span>|<span data-ttu-id="2a37d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a37d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a37d-132">id</span><span class="sxs-lookup"><span data-stu-id="2a37d-132">id</span></span>|<span data-ttu-id="2a37d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2a37d-133">String</span></span>|<span data-ttu-id="2a37d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2a37d-134">Key of the entity.</span></span> <span data-ttu-id="2a37d-135">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="2a37d-136">serialNumber</span></span>|<span data-ttu-id="2a37d-137">String</span><span class="sxs-lookup"><span data-stu-id="2a37d-137">String</span></span>|<span data-ttu-id="2a37d-138">Серийный номер устройства, наследуемый от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-139">рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="2a37d-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="2a37d-140">String.</span><span class="sxs-lookup"><span data-stu-id="2a37d-140">String</span></span>|<span data-ttu-id="2a37d-141">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации, унаследованной от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-142">рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="2a37d-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="2a37d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a37d-143">DateTimeOffset</span></span>|<span data-ttu-id="2a37d-144">Профиль регистрации времени назначен устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="2a37d-145">isSupervised</span></span>|<span data-ttu-id="2a37d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a37d-146">Boolean</span></span>|<span data-ttu-id="2a37d-147">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="2a37d-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="2a37d-148">Дополнительные сведения: https://support.apple.com/en-us/HT202837 наследуются от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="2a37d-149">discoverySource</span></span>|<span data-ttu-id="2a37d-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="2a37d-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="2a37d-151">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="2a37d-151">Apple device discovery source.</span></span> <span data-ttu-id="2a37d-152">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2a37d-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="2a37d-153">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="2a37d-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="2a37d-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a37d-154">createdDateTime</span></span>|<span data-ttu-id="2a37d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a37d-155">DateTimeOffset</span></span>|<span data-ttu-id="2a37d-156">Дата и время создания устройства, унаследованного от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-157">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="2a37d-157">lastContactedDateTime</span></span>|<span data-ttu-id="2a37d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a37d-158">DateTimeOffset</span></span>|<span data-ttu-id="2a37d-159">Дата и время последнего обращения к устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-160">description</span><span class="sxs-lookup"><span data-stu-id="2a37d-160">description</span></span>|<span data-ttu-id="2a37d-161">String</span><span class="sxs-lookup"><span data-stu-id="2a37d-161">String</span></span>|<span data-ttu-id="2a37d-162">Описание устройства, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="2a37d-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="2a37d-163">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="2a37d-163">enrollmentState</span></span>|[<span data-ttu-id="2a37d-164">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="2a37d-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="2a37d-165">Состояние устройства в Intune, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2a37d-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="2a37d-166">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2a37d-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2a37d-167">platform</span><span class="sxs-lookup"><span data-stu-id="2a37d-167">platform</span></span>|[<span data-ttu-id="2a37d-168">управляем</span><span class="sxs-lookup"><span data-stu-id="2a37d-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="2a37d-169">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="2a37d-169">The platform of the Device.</span></span> <span data-ttu-id="2a37d-170">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2a37d-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="2a37d-171">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="2a37d-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="2a37d-172">status</span><span class="sxs-lookup"><span data-stu-id="2a37d-172">status</span></span>|<span data-ttu-id="2a37d-173">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2a37d-173">Boolean</span></span>|<span data-ttu-id="2a37d-174">Состояние импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="2a37d-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="2a37d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a37d-175">Response</span></span>
<span data-ttu-id="2a37d-176">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a37d-176">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a37d-177">Пример</span><span class="sxs-lookup"><span data-stu-id="2a37d-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a37d-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a37d-178">Request</span></span>
<span data-ttu-id="2a37d-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a37d-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="2a37d-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a37d-180">Response</span></span>
<span data-ttu-id="2a37d-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a37d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 630

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




