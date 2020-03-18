---
title: Создание Импортедаппледевицеидентити
description: Создание нового объекта Импортедаппледевицеидентити.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfbf2311bf1e5482de093d5d84987147503edba5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813136"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="7fc00-103">Создание Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="7fc00-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="7fc00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fc00-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fc00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fc00-106">Создание нового объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="7fc00-106">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fc00-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7fc00-107">Prerequisites</span></span>
<span data-ttu-id="7fc00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fc00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fc00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc00-110">Permission type</span></span>|<span data-ttu-id="7fc00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fc00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fc00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fc00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fc00-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc00-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7fc00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fc00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fc00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc00-115">Not supported.</span></span>|
|<span data-ttu-id="7fc00-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7fc00-116">Application</span></span>|<span data-ttu-id="7fc00-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc00-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fc00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fc00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="7fc00-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7fc00-119">Request headers</span></span>
|<span data-ttu-id="7fc00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fc00-120">Header</span></span>|<span data-ttu-id="7fc00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7fc00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fc00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fc00-122">Authorization</span></span>|<span data-ttu-id="7fc00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fc00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fc00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7fc00-124">Accept</span></span>|<span data-ttu-id="7fc00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fc00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fc00-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fc00-126">Request body</span></span>
<span data-ttu-id="7fc00-127">В тексте запроса добавьте представление объекта Импортедаппледевицеидентити в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fc00-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="7fc00-128">В следующей таблице приведены свойства, необходимые при создании Импортедаппледевицеидентити.</span><span class="sxs-lookup"><span data-stu-id="7fc00-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="7fc00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fc00-129">Property</span></span>|<span data-ttu-id="7fc00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7fc00-130">Type</span></span>|<span data-ttu-id="7fc00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7fc00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fc00-132">id</span><span class="sxs-lookup"><span data-stu-id="7fc00-132">id</span></span>|<span data-ttu-id="7fc00-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc00-133">String</span></span>|<span data-ttu-id="7fc00-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7fc00-134">Key of the entity.</span></span>|
|<span data-ttu-id="7fc00-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7fc00-135">serialNumber</span></span>|<span data-ttu-id="7fc00-136">String</span><span class="sxs-lookup"><span data-stu-id="7fc00-136">String</span></span>|<span data-ttu-id="7fc00-137">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="7fc00-137">Device serial number</span></span>|
|<span data-ttu-id="7fc00-138">рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="7fc00-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="7fc00-139">String</span><span class="sxs-lookup"><span data-stu-id="7fc00-139">String</span></span>|<span data-ttu-id="7fc00-140">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="7fc00-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="7fc00-141">рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="7fc00-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="7fc00-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fc00-142">DateTimeOffset</span></span>|<span data-ttu-id="7fc00-143">Для устройства назначен профиль регистрации времени.</span><span class="sxs-lookup"><span data-stu-id="7fc00-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="7fc00-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="7fc00-144">isSupervised</span></span>|<span data-ttu-id="7fc00-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fc00-145">Boolean</span></span>|<span data-ttu-id="7fc00-146">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="7fc00-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="7fc00-147">Дополнительные сведения:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="7fc00-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="7fc00-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="7fc00-148">discoverySource</span></span>|<span data-ttu-id="7fc00-149">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="7fc00-149">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="7fc00-150">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="7fc00-150">Apple device discovery source.</span></span> <span data-ttu-id="7fc00-151">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="7fc00-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="7fc00-152">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7fc00-152">isDeleted</span></span>|<span data-ttu-id="7fc00-153">Логический</span><span class="sxs-lookup"><span data-stu-id="7fc00-153">Boolean</span></span>|<span data-ttu-id="7fc00-154">Указывает, было ли устройство удалено из Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="7fc00-154">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="7fc00-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7fc00-155">createdDateTime</span></span>|<span data-ttu-id="7fc00-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fc00-156">DateTimeOffset</span></span>|<span data-ttu-id="7fc00-157">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="7fc00-157">Created Date Time of the device</span></span>|
|<span data-ttu-id="7fc00-158">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="7fc00-158">lastContactedDateTime</span></span>|<span data-ttu-id="7fc00-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fc00-159">DateTimeOffset</span></span>|<span data-ttu-id="7fc00-160">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="7fc00-160">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="7fc00-161">description</span><span class="sxs-lookup"><span data-stu-id="7fc00-161">description</span></span>|<span data-ttu-id="7fc00-162">String</span><span class="sxs-lookup"><span data-stu-id="7fc00-162">String</span></span>|<span data-ttu-id="7fc00-163">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="7fc00-163">The description of the device</span></span>|
|<span data-ttu-id="7fc00-164">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="7fc00-164">enrollmentState</span></span>|[<span data-ttu-id="7fc00-165">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="7fc00-165">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="7fc00-166">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="7fc00-166">The state of the device in Intune.</span></span> <span data-ttu-id="7fc00-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="7fc00-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7fc00-168">platform</span><span class="sxs-lookup"><span data-stu-id="7fc00-168">platform</span></span>|[<span data-ttu-id="7fc00-169">управляем</span><span class="sxs-lookup"><span data-stu-id="7fc00-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="7fc00-170">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="7fc00-170">The platform of the Device.</span></span> <span data-ttu-id="7fc00-171">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="7fc00-171">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="7fc00-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc00-172">Response</span></span>
<span data-ttu-id="7fc00-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fc00-173">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fc00-174">Пример</span><span class="sxs-lookup"><span data-stu-id="7fc00-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fc00-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fc00-175">Request</span></span>
<span data-ttu-id="7fc00-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fc00-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="7fc00-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc00-177">Response</span></span>
<span data-ttu-id="7fc00-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fc00-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




