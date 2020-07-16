---
title: Обновление Импортедаппледевицеидентитиресулт
description: Обновление свойств объекта Импортедаппледевицеидентитиресулт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 407c6e10a289d08a695c12562d7791d539c09056
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122611"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="5e080-103">Обновление Импортедаппледевицеидентитиресулт</span><span class="sxs-lookup"><span data-stu-id="5e080-103">Update importedAppleDeviceIdentityResult</span></span>

<span data-ttu-id="5e080-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e080-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e080-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e080-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e080-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e080-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e080-107">Обновление свойств объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="5e080-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e080-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e080-108">Prerequisites</span></span>
<span data-ttu-id="5e080-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e080-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e080-111">Permission type</span></span>|<span data-ttu-id="5e080-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e080-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e080-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e080-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e080-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e080-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5e080-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e080-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e080-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e080-116">Not supported.</span></span>|
|<span data-ttu-id="5e080-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e080-117">Application</span></span>|<span data-ttu-id="5e080-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e080-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e080-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e080-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="5e080-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5e080-120">Request headers</span></span>
|<span data-ttu-id="5e080-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e080-121">Header</span></span>|<span data-ttu-id="5e080-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e080-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e080-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e080-123">Authorization</span></span>|<span data-ttu-id="5e080-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e080-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e080-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e080-125">Accept</span></span>|<span data-ttu-id="5e080-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e080-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e080-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e080-127">Request body</span></span>
<span data-ttu-id="5e080-128">В тексте запроса добавьте представление объекта [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e080-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="5e080-129">В следующей таблице приведены свойства, необходимые при создании [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="5e080-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="5e080-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e080-130">Property</span></span>|<span data-ttu-id="5e080-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5e080-131">Type</span></span>|<span data-ttu-id="5e080-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5e080-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e080-133">id</span><span class="sxs-lookup"><span data-stu-id="5e080-133">id</span></span>|<span data-ttu-id="5e080-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5e080-134">String</span></span>|<span data-ttu-id="5e080-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e080-135">Key of the entity.</span></span> <span data-ttu-id="5e080-136">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5e080-137">serialNumber</span></span>|<span data-ttu-id="5e080-138">String</span><span class="sxs-lookup"><span data-stu-id="5e080-138">String</span></span>|<span data-ttu-id="5e080-139">Серийный номер устройства, наследуемый от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-140">рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="5e080-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="5e080-141">String</span><span class="sxs-lookup"><span data-stu-id="5e080-141">String</span></span>|<span data-ttu-id="5e080-142">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации, унаследованной от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-143">рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="5e080-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="5e080-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e080-144">DateTimeOffset</span></span>|<span data-ttu-id="5e080-145">Профиль регистрации времени назначен устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="5e080-146">isSupervised</span></span>|<span data-ttu-id="5e080-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e080-147">Boolean</span></span>|<span data-ttu-id="5e080-148">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="5e080-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="5e080-149">Дополнительные сведения: https://support.apple.com/HT202837 наследуются от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-149">More information is at: https://support.apple.com/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="5e080-150">discoverySource</span></span>|<span data-ttu-id="5e080-151">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="5e080-151">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="5e080-152">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="5e080-152">Apple device discovery source.</span></span> <span data-ttu-id="5e080-153">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5e080-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5e080-154">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="5e080-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="5e080-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5e080-155">isDeleted</span></span>|<span data-ttu-id="5e080-156">Логический</span><span class="sxs-lookup"><span data-stu-id="5e080-156">Boolean</span></span>|<span data-ttu-id="5e080-157">Указывает, будет ли устройство удалено из Apple Business Manager, унаследованное от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-157">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e080-158">createdDateTime</span></span>|<span data-ttu-id="5e080-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e080-159">DateTimeOffset</span></span>|<span data-ttu-id="5e080-160">Дата и время создания устройства, унаследованного от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-160">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-161">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="5e080-161">lastContactedDateTime</span></span>|<span data-ttu-id="5e080-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e080-162">DateTimeOffset</span></span>|<span data-ttu-id="5e080-163">Дата и время последнего обращения к устройству, унаследованному от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-163">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-164">description</span><span class="sxs-lookup"><span data-stu-id="5e080-164">description</span></span>|<span data-ttu-id="5e080-165">String</span><span class="sxs-lookup"><span data-stu-id="5e080-165">String</span></span>|<span data-ttu-id="5e080-166">Описание устройства, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5e080-166">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="5e080-167">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="5e080-167">enrollmentState</span></span>|[<span data-ttu-id="5e080-168">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="5e080-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="5e080-169">Состояние устройства в Intune, наследуемого из [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5e080-169">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5e080-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="5e080-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5e080-171">platform</span><span class="sxs-lookup"><span data-stu-id="5e080-171">platform</span></span>|[<span data-ttu-id="5e080-172">управляем</span><span class="sxs-lookup"><span data-stu-id="5e080-172">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="5e080-173">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="5e080-173">The platform of the Device.</span></span> <span data-ttu-id="5e080-174">Наследуется от [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5e080-174">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="5e080-175">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="5e080-175">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="5e080-176">status</span><span class="sxs-lookup"><span data-stu-id="5e080-176">status</span></span>|<span data-ttu-id="5e080-177">Логический</span><span class="sxs-lookup"><span data-stu-id="5e080-177">Boolean</span></span>|<span data-ttu-id="5e080-178">Состояние импортированного удостоверения устройства</span><span class="sxs-lookup"><span data-stu-id="5e080-178">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="5e080-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e080-179">Response</span></span>
<span data-ttu-id="5e080-180">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e080-180">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e080-181">Пример</span><span class="sxs-lookup"><span data-stu-id="5e080-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e080-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e080-182">Request</span></span>
<span data-ttu-id="5e080-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e080-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="5e080-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e080-184">Response</span></span>
<span data-ttu-id="5e080-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e080-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```



