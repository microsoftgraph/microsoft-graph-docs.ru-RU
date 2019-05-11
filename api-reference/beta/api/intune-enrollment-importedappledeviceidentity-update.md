---
title: Обновление Импортедаппледевицеидентити
description: Обновление свойств объекта Импортедаппледевицеидентити.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7881e153261ad71b2468f5555386c9c17f3d3983
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908479"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="35a5a-103">Обновление Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="35a5a-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="35a5a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35a5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35a5a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35a5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35a5a-106">Обновление свойств объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="35a5a-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35a5a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35a5a-107">Prerequisites</span></span>
<span data-ttu-id="35a5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35a5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35a5a-110">Permission type</span></span>|<span data-ttu-id="35a5a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35a5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35a5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35a5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35a5a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35a5a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="35a5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35a5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35a5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35a5a-115">Not supported.</span></span>|
|<span data-ttu-id="35a5a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35a5a-116">Application</span></span>|<span data-ttu-id="35a5a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35a5a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35a5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35a5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="35a5a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35a5a-119">Request headers</span></span>
|<span data-ttu-id="35a5a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35a5a-120">Header</span></span>|<span data-ttu-id="35a5a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="35a5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35a5a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35a5a-122">Authorization</span></span>|<span data-ttu-id="35a5a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35a5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35a5a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="35a5a-124">Accept</span></span>|<span data-ttu-id="35a5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35a5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35a5a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35a5a-126">Request body</span></span>
<span data-ttu-id="35a5a-127">В тексте запроса добавьте представление объекта [Импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35a5a-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="35a5a-128">В следующей таблице приведены свойства, необходимые при создании [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="35a5a-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="35a5a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="35a5a-129">Property</span></span>|<span data-ttu-id="35a5a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="35a5a-130">Type</span></span>|<span data-ttu-id="35a5a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="35a5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35a5a-132">id</span><span class="sxs-lookup"><span data-stu-id="35a5a-132">id</span></span>|<span data-ttu-id="35a5a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="35a5a-133">String</span></span>|<span data-ttu-id="35a5a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="35a5a-134">Key of the entity.</span></span>|
|<span data-ttu-id="35a5a-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="35a5a-135">serialNumber</span></span>|<span data-ttu-id="35a5a-136">String</span><span class="sxs-lookup"><span data-stu-id="35a5a-136">String</span></span>|<span data-ttu-id="35a5a-137">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="35a5a-137">Device serial number</span></span>|
|<span data-ttu-id="35a5a-138">Рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="35a5a-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="35a5a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="35a5a-139">String</span></span>|<span data-ttu-id="35a5a-140">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="35a5a-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="35a5a-141">Рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="35a5a-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="35a5a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35a5a-142">DateTimeOffset</span></span>|<span data-ttu-id="35a5a-143">Для устройства назначен профиль регистрации времени.</span><span class="sxs-lookup"><span data-stu-id="35a5a-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="35a5a-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="35a5a-144">isSupervised</span></span>|<span data-ttu-id="35a5a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="35a5a-145">Boolean</span></span>|<span data-ttu-id="35a5a-146">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="35a5a-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="35a5a-147">Дополнительные сведения:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="35a5a-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="35a5a-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="35a5a-148">discoverySource</span></span>|<span data-ttu-id="35a5a-149">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="35a5a-149">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="35a5a-150">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="35a5a-150">Apple device discovery source.</span></span> <span data-ttu-id="35a5a-151">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="35a5a-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="35a5a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35a5a-152">createdDateTime</span></span>|<span data-ttu-id="35a5a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35a5a-153">DateTimeOffset</span></span>|<span data-ttu-id="35a5a-154">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="35a5a-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="35a5a-155">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="35a5a-155">lastContactedDateTime</span></span>|<span data-ttu-id="35a5a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35a5a-156">DateTimeOffset</span></span>|<span data-ttu-id="35a5a-157">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="35a5a-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="35a5a-158">description</span><span class="sxs-lookup"><span data-stu-id="35a5a-158">description</span></span>|<span data-ttu-id="35a5a-159">String</span><span class="sxs-lookup"><span data-stu-id="35a5a-159">String</span></span>|<span data-ttu-id="35a5a-160">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="35a5a-160">The description of the device</span></span>|
|<span data-ttu-id="35a5a-161">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="35a5a-161">enrollmentState</span></span>|[<span data-ttu-id="35a5a-162">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="35a5a-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="35a5a-163">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="35a5a-163">The state of the device in Intune.</span></span> <span data-ttu-id="35a5a-164">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="35a5a-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="35a5a-165">platform</span><span class="sxs-lookup"><span data-stu-id="35a5a-165">platform</span></span>|[<span data-ttu-id="35a5a-166">управляем</span><span class="sxs-lookup"><span data-stu-id="35a5a-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="35a5a-167">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="35a5a-167">The platform of the Device.</span></span> <span data-ttu-id="35a5a-168">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="35a5a-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="35a5a-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="35a5a-169">Response</span></span>
<span data-ttu-id="35a5a-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35a5a-170">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35a5a-171">Пример</span><span class="sxs-lookup"><span data-stu-id="35a5a-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="35a5a-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="35a5a-172">Request</span></span>
<span data-ttu-id="35a5a-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35a5a-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="35a5a-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="35a5a-174">Response</span></span>
<span data-ttu-id="35a5a-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35a5a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```




