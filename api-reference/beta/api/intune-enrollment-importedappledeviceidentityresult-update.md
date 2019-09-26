---
title: Обновление Импортедаппледевицеидентитиресулт
description: Обновление свойств объекта Импортедаппледевицеидентитиресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b71a471c5391e67e6119abfeab56146a9afa84d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37184960"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="eb5e7-103">Обновление Импортедаппледевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="eb5e7-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="eb5e7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb5e7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb5e7-106">Обновление свойств объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="eb5e7-106">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb5e7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eb5e7-107">Prerequisites</span></span>
<span data-ttu-id="eb5e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb5e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb5e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb5e7-110">Permission type</span></span>|<span data-ttu-id="eb5e7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb5e7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb5e7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb5e7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb5e7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb5e7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-115">Not supported.</span></span>|
|<span data-ttu-id="eb5e7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb5e7-116">Application</span></span>|<span data-ttu-id="eb5e7-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb5e7-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb5e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb5e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="eb5e7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb5e7-119">Request headers</span></span>
|<span data-ttu-id="eb5e7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb5e7-120">Header</span></span>|<span data-ttu-id="eb5e7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eb5e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb5e7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb5e7-122">Authorization</span></span>|<span data-ttu-id="eb5e7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb5e7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eb5e7-124">Accept</span></span>|<span data-ttu-id="eb5e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb5e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb5e7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb5e7-126">Request body</span></span>
<span data-ttu-id="eb5e7-127">В тексте запроса добавьте представление объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="eb5e7-128">В следующей таблице приведены свойства, необходимые при создании [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="eb5e7-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="eb5e7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb5e7-129">Property</span></span>|<span data-ttu-id="eb5e7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eb5e7-130">Type</span></span>|<span data-ttu-id="eb5e7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eb5e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb5e7-132">id</span><span class="sxs-lookup"><span data-stu-id="eb5e7-132">id</span></span>|<span data-ttu-id="eb5e7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="eb5e7-133">String</span></span>|<span data-ttu-id="eb5e7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-134">Key of the entity.</span></span> <span data-ttu-id="eb5e7-135">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-135">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="eb5e7-136">serialNumber</span></span>|<span data-ttu-id="eb5e7-137">String</span><span class="sxs-lookup"><span data-stu-id="eb5e7-137">String</span></span>|<span data-ttu-id="eb5e7-138">Серийный номер устройства, наследуемый от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-138">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-139">рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="eb5e7-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="eb5e7-140">String.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-140">String</span></span>|<span data-ttu-id="eb5e7-141">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации, унаследованной от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-141">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-142">рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="eb5e7-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="eb5e7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb5e7-143">DateTimeOffset</span></span>|<span data-ttu-id="eb5e7-144">Профиль регистрации времени назначен устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-144">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="eb5e7-145">isSupervised</span></span>|<span data-ttu-id="eb5e7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb5e7-146">Boolean</span></span>|<span data-ttu-id="eb5e7-147">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="eb5e7-148">Дополнительные сведения: https://support.apple.com/en-us/HT202837 наследуются от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-148">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="eb5e7-149">discoverySource</span></span>|<span data-ttu-id="eb5e7-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="eb5e7-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="eb5e7-151">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-151">Apple device discovery source.</span></span> <span data-ttu-id="eb5e7-152">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="eb5e7-152">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="eb5e7-153">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-153">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="eb5e7-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb5e7-154">createdDateTime</span></span>|<span data-ttu-id="eb5e7-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb5e7-155">DateTimeOffset</span></span>|<span data-ttu-id="eb5e7-156">Дата и время создания устройства, унаследованного от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-156">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-157">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="eb5e7-157">lastContactedDateTime</span></span>|<span data-ttu-id="eb5e7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb5e7-158">DateTimeOffset</span></span>|<span data-ttu-id="eb5e7-159">Дата и время последнего обращения к устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-159">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-160">description</span><span class="sxs-lookup"><span data-stu-id="eb5e7-160">description</span></span>|<span data-ttu-id="eb5e7-161">String</span><span class="sxs-lookup"><span data-stu-id="eb5e7-161">String</span></span>|<span data-ttu-id="eb5e7-162">Описание устройства, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="eb5e7-162">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="eb5e7-163">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="eb5e7-163">enrollmentState</span></span>|[<span data-ttu-id="eb5e7-164">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="eb5e7-164">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="eb5e7-165">Состояние устройства в Intune, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="eb5e7-165">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="eb5e7-166">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-166">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="eb5e7-167">platform</span><span class="sxs-lookup"><span data-stu-id="eb5e7-167">platform</span></span>|[<span data-ttu-id="eb5e7-168">управляем</span><span class="sxs-lookup"><span data-stu-id="eb5e7-168">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="eb5e7-169">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-169">The platform of the Device.</span></span> <span data-ttu-id="eb5e7-170">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="eb5e7-170">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="eb5e7-171">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="eb5e7-172">status</span><span class="sxs-lookup"><span data-stu-id="eb5e7-172">status</span></span>|<span data-ttu-id="eb5e7-173">Boolean.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-173">Boolean</span></span>|<span data-ttu-id="eb5e7-174">Состояние импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="eb5e7-174">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="eb5e7-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb5e7-175">Response</span></span>
<span data-ttu-id="eb5e7-176">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-176">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb5e7-177">Пример</span><span class="sxs-lookup"><span data-stu-id="eb5e7-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb5e7-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb5e7-178">Request</span></span>
<span data-ttu-id="eb5e7-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="eb5e7-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb5e7-180">Response</span></span>
<span data-ttu-id="eb5e7-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb5e7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




