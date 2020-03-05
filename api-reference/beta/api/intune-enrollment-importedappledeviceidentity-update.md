---
title: Обновление Импортедаппледевицеидентити
description: Обновление свойств объекта Импортедаппледевицеидентити.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f184fa8b5b73c7ad0da1f48156f7e5dcbad03115
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466803"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="edf3a-103">Обновление Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="edf3a-103">Update importedAppleDeviceIdentity</span></span>

<span data-ttu-id="edf3a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="edf3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edf3a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edf3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edf3a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edf3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edf3a-107">Обновление свойств объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="edf3a-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edf3a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="edf3a-108">Prerequisites</span></span>
<span data-ttu-id="edf3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edf3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edf3a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edf3a-111">Permission type</span></span>|<span data-ttu-id="edf3a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="edf3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edf3a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edf3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edf3a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edf3a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="edf3a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edf3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edf3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edf3a-116">Not supported.</span></span>|
|<span data-ttu-id="edf3a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edf3a-117">Application</span></span>|<span data-ttu-id="edf3a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edf3a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edf3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edf3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="edf3a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="edf3a-120">Request headers</span></span>
|<span data-ttu-id="edf3a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edf3a-121">Header</span></span>|<span data-ttu-id="edf3a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="edf3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edf3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edf3a-123">Authorization</span></span>|<span data-ttu-id="edf3a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edf3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edf3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="edf3a-125">Accept</span></span>|<span data-ttu-id="edf3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edf3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edf3a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edf3a-127">Request body</span></span>
<span data-ttu-id="edf3a-128">В тексте запроса добавьте представление объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edf3a-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="edf3a-129">В следующей таблице приведены свойства, необходимые при создании [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="edf3a-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="edf3a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="edf3a-130">Property</span></span>|<span data-ttu-id="edf3a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="edf3a-131">Type</span></span>|<span data-ttu-id="edf3a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="edf3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edf3a-133">id</span><span class="sxs-lookup"><span data-stu-id="edf3a-133">id</span></span>|<span data-ttu-id="edf3a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="edf3a-134">String</span></span>|<span data-ttu-id="edf3a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="edf3a-135">Key of the entity.</span></span>|
|<span data-ttu-id="edf3a-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="edf3a-136">serialNumber</span></span>|<span data-ttu-id="edf3a-137">String</span><span class="sxs-lookup"><span data-stu-id="edf3a-137">String</span></span>|<span data-ttu-id="edf3a-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="edf3a-138">Device serial number</span></span>|
|<span data-ttu-id="edf3a-139">рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="edf3a-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="edf3a-140">String</span><span class="sxs-lookup"><span data-stu-id="edf3a-140">String</span></span>|<span data-ttu-id="edf3a-141">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="edf3a-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="edf3a-142">рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="edf3a-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="edf3a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edf3a-143">DateTimeOffset</span></span>|<span data-ttu-id="edf3a-144">Для устройства назначен профиль регистрации времени.</span><span class="sxs-lookup"><span data-stu-id="edf3a-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="edf3a-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="edf3a-145">isSupervised</span></span>|<span data-ttu-id="edf3a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="edf3a-146">Boolean</span></span>|<span data-ttu-id="edf3a-147">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="edf3a-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="edf3a-148">Дополнительные сведения:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="edf3a-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="edf3a-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="edf3a-149">discoverySource</span></span>|<span data-ttu-id="edf3a-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="edf3a-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="edf3a-151">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="edf3a-151">Apple device discovery source.</span></span> <span data-ttu-id="edf3a-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="edf3a-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="edf3a-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="edf3a-153">isDeleted</span></span>|<span data-ttu-id="edf3a-154">Логический</span><span class="sxs-lookup"><span data-stu-id="edf3a-154">Boolean</span></span>|<span data-ttu-id="edf3a-155">Указывает, было ли устройство удалено из Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="edf3a-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="edf3a-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edf3a-156">createdDateTime</span></span>|<span data-ttu-id="edf3a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edf3a-157">DateTimeOffset</span></span>|<span data-ttu-id="edf3a-158">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="edf3a-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="edf3a-159">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="edf3a-159">lastContactedDateTime</span></span>|<span data-ttu-id="edf3a-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edf3a-160">DateTimeOffset</span></span>|<span data-ttu-id="edf3a-161">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="edf3a-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="edf3a-162">description</span><span class="sxs-lookup"><span data-stu-id="edf3a-162">description</span></span>|<span data-ttu-id="edf3a-163">String</span><span class="sxs-lookup"><span data-stu-id="edf3a-163">String</span></span>|<span data-ttu-id="edf3a-164">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="edf3a-164">The description of the device</span></span>|
|<span data-ttu-id="edf3a-165">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="edf3a-165">enrollmentState</span></span>|[<span data-ttu-id="edf3a-166">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="edf3a-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="edf3a-167">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="edf3a-167">The state of the device in Intune.</span></span> <span data-ttu-id="edf3a-168">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="edf3a-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="edf3a-169">platform</span><span class="sxs-lookup"><span data-stu-id="edf3a-169">platform</span></span>|[<span data-ttu-id="edf3a-170">управляем</span><span class="sxs-lookup"><span data-stu-id="edf3a-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="edf3a-171">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="edf3a-171">The platform of the Device.</span></span> <span data-ttu-id="edf3a-172">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="edf3a-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="edf3a-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="edf3a-173">Response</span></span>
<span data-ttu-id="edf3a-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edf3a-174">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edf3a-175">Пример</span><span class="sxs-lookup"><span data-stu-id="edf3a-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="edf3a-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="edf3a-176">Request</span></span>
<span data-ttu-id="edf3a-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edf3a-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="edf3a-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="edf3a-178">Response</span></span>
<span data-ttu-id="edf3a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edf3a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





