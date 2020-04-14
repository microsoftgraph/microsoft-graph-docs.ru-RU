---
title: Обновление Импортедаппледевицеидентити
description: Обновление свойств объекта Импортедаппледевицеидентити.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10248fcb46a4d20667afd61cd41759dcc7da842c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451178"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="49ac9-103">Обновление Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="49ac9-103">Update importedAppleDeviceIdentity</span></span>

<span data-ttu-id="49ac9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49ac9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49ac9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49ac9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49ac9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49ac9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49ac9-107">Обновление свойств объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="49ac9-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49ac9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49ac9-108">Prerequisites</span></span>
<span data-ttu-id="49ac9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49ac9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49ac9-111">Permission type</span></span>|<span data-ttu-id="49ac9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49ac9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49ac9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49ac9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49ac9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ac9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49ac9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49ac9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49ac9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49ac9-116">Not supported.</span></span>|
|<span data-ttu-id="49ac9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49ac9-117">Application</span></span>|<span data-ttu-id="49ac9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ac9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49ac9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49ac9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="49ac9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49ac9-120">Request headers</span></span>
|<span data-ttu-id="49ac9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49ac9-121">Header</span></span>|<span data-ttu-id="49ac9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49ac9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49ac9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49ac9-123">Authorization</span></span>|<span data-ttu-id="49ac9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49ac9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49ac9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49ac9-125">Accept</span></span>|<span data-ttu-id="49ac9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49ac9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49ac9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49ac9-127">Request body</span></span>
<span data-ttu-id="49ac9-128">В тексте запроса добавьте представление объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49ac9-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="49ac9-129">В следующей таблице приведены свойства, необходимые при создании [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="49ac9-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="49ac9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49ac9-130">Property</span></span>|<span data-ttu-id="49ac9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49ac9-131">Type</span></span>|<span data-ttu-id="49ac9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49ac9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49ac9-133">id</span><span class="sxs-lookup"><span data-stu-id="49ac9-133">id</span></span>|<span data-ttu-id="49ac9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="49ac9-134">String</span></span>|<span data-ttu-id="49ac9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49ac9-135">Key of the entity.</span></span>|
|<span data-ttu-id="49ac9-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="49ac9-136">serialNumber</span></span>|<span data-ttu-id="49ac9-137">String</span><span class="sxs-lookup"><span data-stu-id="49ac9-137">String</span></span>|<span data-ttu-id="49ac9-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="49ac9-138">Device serial number</span></span>|
|<span data-ttu-id="49ac9-139">рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="49ac9-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="49ac9-140">String</span><span class="sxs-lookup"><span data-stu-id="49ac9-140">String</span></span>|<span data-ttu-id="49ac9-141">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="49ac9-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="49ac9-142">рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="49ac9-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="49ac9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ac9-143">DateTimeOffset</span></span>|<span data-ttu-id="49ac9-144">Для устройства назначен профиль регистрации времени.</span><span class="sxs-lookup"><span data-stu-id="49ac9-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="49ac9-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="49ac9-145">isSupervised</span></span>|<span data-ttu-id="49ac9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="49ac9-146">Boolean</span></span>|<span data-ttu-id="49ac9-147">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="49ac9-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="49ac9-148">Дополнительные сведения:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="49ac9-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="49ac9-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="49ac9-149">discoverySource</span></span>|<span data-ttu-id="49ac9-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="49ac9-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="49ac9-151">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="49ac9-151">Apple device discovery source.</span></span> <span data-ttu-id="49ac9-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="49ac9-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="49ac9-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="49ac9-153">isDeleted</span></span>|<span data-ttu-id="49ac9-154">Логическое</span><span class="sxs-lookup"><span data-stu-id="49ac9-154">Boolean</span></span>|<span data-ttu-id="49ac9-155">Указывает, было ли устройство удалено из Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="49ac9-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="49ac9-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49ac9-156">createdDateTime</span></span>|<span data-ttu-id="49ac9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ac9-157">DateTimeOffset</span></span>|<span data-ttu-id="49ac9-158">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="49ac9-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="49ac9-159">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="49ac9-159">lastContactedDateTime</span></span>|<span data-ttu-id="49ac9-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ac9-160">DateTimeOffset</span></span>|<span data-ttu-id="49ac9-161">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="49ac9-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="49ac9-162">description</span><span class="sxs-lookup"><span data-stu-id="49ac9-162">description</span></span>|<span data-ttu-id="49ac9-163">String</span><span class="sxs-lookup"><span data-stu-id="49ac9-163">String</span></span>|<span data-ttu-id="49ac9-164">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="49ac9-164">The description of the device</span></span>|
|<span data-ttu-id="49ac9-165">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="49ac9-165">enrollmentState</span></span>|[<span data-ttu-id="49ac9-166">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="49ac9-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="49ac9-167">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="49ac9-167">The state of the device in Intune.</span></span> <span data-ttu-id="49ac9-168">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="49ac9-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="49ac9-169">platform</span><span class="sxs-lookup"><span data-stu-id="49ac9-169">platform</span></span>|[<span data-ttu-id="49ac9-170">управляем</span><span class="sxs-lookup"><span data-stu-id="49ac9-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="49ac9-171">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="49ac9-171">The platform of the Device.</span></span> <span data-ttu-id="49ac9-172">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="49ac9-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="49ac9-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="49ac9-173">Response</span></span>
<span data-ttu-id="49ac9-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49ac9-174">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49ac9-175">Пример</span><span class="sxs-lookup"><span data-stu-id="49ac9-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="49ac9-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="49ac9-176">Request</span></span>
<span data-ttu-id="49ac9-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49ac9-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 519

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="49ac9-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="49ac9-178">Response</span></span>
<span data-ttu-id="49ac9-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49ac9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
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
  "platform": "ios"
}
```



