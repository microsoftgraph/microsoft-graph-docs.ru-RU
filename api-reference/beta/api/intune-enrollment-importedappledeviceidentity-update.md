---
title: Обновление Импортедаппледевицеидентити
description: Обновление свойств объекта Импортедаппледевицеидентити.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4de33b356d23acacef13936259ce35304bb903d3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797454"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="1f47f-103">Обновление Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="1f47f-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="1f47f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f47f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f47f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f47f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f47f-106">Обновление свойств объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="1f47f-106">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f47f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f47f-107">Prerequisites</span></span>
<span data-ttu-id="1f47f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f47f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f47f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f47f-110">Permission type</span></span>|<span data-ttu-id="1f47f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f47f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f47f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f47f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f47f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f47f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f47f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f47f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f47f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f47f-115">Not supported.</span></span>|
|<span data-ttu-id="1f47f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f47f-116">Application</span></span>|<span data-ttu-id="1f47f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f47f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f47f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f47f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="1f47f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f47f-119">Request headers</span></span>
|<span data-ttu-id="1f47f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f47f-120">Header</span></span>|<span data-ttu-id="1f47f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1f47f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f47f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f47f-122">Authorization</span></span>|<span data-ttu-id="1f47f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f47f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f47f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1f47f-124">Accept</span></span>|<span data-ttu-id="1f47f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f47f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f47f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f47f-126">Request body</span></span>
<span data-ttu-id="1f47f-127">В тексте запроса добавьте представление объекта [Импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f47f-127">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="1f47f-128">В следующей таблице приведены свойства, необходимые при создании [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="1f47f-128">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="1f47f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f47f-129">Property</span></span>|<span data-ttu-id="1f47f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1f47f-130">Type</span></span>|<span data-ttu-id="1f47f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1f47f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f47f-132">id</span><span class="sxs-lookup"><span data-stu-id="1f47f-132">id</span></span>|<span data-ttu-id="1f47f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1f47f-133">String</span></span>|<span data-ttu-id="1f47f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1f47f-134">Key of the entity.</span></span>|
|<span data-ttu-id="1f47f-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1f47f-135">serialNumber</span></span>|<span data-ttu-id="1f47f-136">String</span><span class="sxs-lookup"><span data-stu-id="1f47f-136">String</span></span>|<span data-ttu-id="1f47f-137">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="1f47f-137">Device serial number</span></span>|
|<span data-ttu-id="1f47f-138">Рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="1f47f-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="1f47f-139">String</span><span class="sxs-lookup"><span data-stu-id="1f47f-139">String</span></span>|<span data-ttu-id="1f47f-140">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="1f47f-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="1f47f-141">Рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="1f47f-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="1f47f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f47f-142">DateTimeOffset</span></span>|<span data-ttu-id="1f47f-143">Для устройства назначен профиль регистрации времени.</span><span class="sxs-lookup"><span data-stu-id="1f47f-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="1f47f-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1f47f-144">isSupervised</span></span>|<span data-ttu-id="1f47f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f47f-145">Boolean</span></span>|<span data-ttu-id="1f47f-146">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="1f47f-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="1f47f-147">Дополнительные сведения:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="1f47f-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="1f47f-148">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1f47f-148">discoverySource</span></span>|[<span data-ttu-id="1f47f-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1f47f-149">discoverySource</span></span>](../resources/intune-enrollment-discoverysource.md)|<span data-ttu-id="1f47f-150">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="1f47f-150">Apple device discovery source.</span></span> <span data-ttu-id="1f47f-151">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="1f47f-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="1f47f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f47f-152">createdDateTime</span></span>|<span data-ttu-id="1f47f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f47f-153">DateTimeOffset</span></span>|<span data-ttu-id="1f47f-154">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="1f47f-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="1f47f-155">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="1f47f-155">lastContactedDateTime</span></span>|<span data-ttu-id="1f47f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f47f-156">DateTimeOffset</span></span>|<span data-ttu-id="1f47f-157">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="1f47f-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="1f47f-158">description</span><span class="sxs-lookup"><span data-stu-id="1f47f-158">description</span></span>|<span data-ttu-id="1f47f-159">String</span><span class="sxs-lookup"><span data-stu-id="1f47f-159">String</span></span>|<span data-ttu-id="1f47f-160">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="1f47f-160">The description of the device</span></span>|
|<span data-ttu-id="1f47f-161">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="1f47f-161">enrollmentState</span></span>|[<span data-ttu-id="1f47f-162">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="1f47f-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="1f47f-163">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="1f47f-163">The state of the device in Intune.</span></span> <span data-ttu-id="1f47f-164">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="1f47f-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1f47f-165">platform</span><span class="sxs-lookup"><span data-stu-id="1f47f-165">platform</span></span>|[<span data-ttu-id="1f47f-166">platform</span><span class="sxs-lookup"><span data-stu-id="1f47f-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1f47f-167">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="1f47f-167">The platform of the Device.</span></span> <span data-ttu-id="1f47f-168">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="1f47f-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="1f47f-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f47f-169">Response</span></span>
<span data-ttu-id="1f47f-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f47f-170">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f47f-171">Пример</span><span class="sxs-lookup"><span data-stu-id="1f47f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f47f-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f47f-172">Request</span></span>
<span data-ttu-id="1f47f-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f47f-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f47f-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f47f-174">Response</span></span>
<span data-ttu-id="1f47f-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f47f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





