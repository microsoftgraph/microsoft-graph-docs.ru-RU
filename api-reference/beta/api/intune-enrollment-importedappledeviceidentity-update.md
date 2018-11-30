---
title: Обновление importedAppleDeviceIdentity
description: Обновление свойства объекта importedAppleDeviceIdentity.
ms.openlocfilehash: 48fbcd38e7e74734b069b9a0b8db6d675fe26a96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081092"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="6f003-103">Обновление importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6f003-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="6f003-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f003-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f003-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f003-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f003-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f003-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f003-107">Обновление свойства объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="6f003-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f003-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f003-108">Prerequisites</span></span>
<span data-ttu-id="6f003-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f003-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f003-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f003-111">Permission type</span></span>|<span data-ttu-id="6f003-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f003-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f003-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f003-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f003-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f003-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f003-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f003-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f003-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f003-116">Not supported.</span></span>|
|<span data-ttu-id="6f003-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f003-117">Application</span></span>|<span data-ttu-id="6f003-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f003-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f003-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f003-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="6f003-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f003-120">Request headers</span></span>
|<span data-ttu-id="6f003-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f003-121">Header</span></span>|<span data-ttu-id="6f003-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f003-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f003-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f003-123">Authorization</span></span>|<span data-ttu-id="6f003-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f003-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f003-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f003-125">Accept</span></span>|<span data-ttu-id="6f003-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f003-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f003-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f003-127">Request body</span></span>
<span data-ttu-id="6f003-128">В тексте запроса укажите представление JSON для объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="6f003-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="6f003-129">В следующей таблице показаны свойства, которые необходимы для создания [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="6f003-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="6f003-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f003-130">Property</span></span>|<span data-ttu-id="6f003-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f003-131">Type</span></span>|<span data-ttu-id="6f003-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f003-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f003-133">id</span><span class="sxs-lookup"><span data-stu-id="6f003-133">id</span></span>|<span data-ttu-id="6f003-134">String</span><span class="sxs-lookup"><span data-stu-id="6f003-134">String</span></span>|<span data-ttu-id="6f003-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f003-135">Key of the entity.</span></span>|
|<span data-ttu-id="6f003-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="6f003-136">serialNumber</span></span>|<span data-ttu-id="6f003-137">String</span><span class="sxs-lookup"><span data-stu-id="6f003-137">String</span></span>|<span data-ttu-id="6f003-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="6f003-138">Device serial number</span></span>|
|<span data-ttu-id="6f003-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="6f003-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="6f003-140">String</span><span class="sxs-lookup"><span data-stu-id="6f003-140">String</span></span>|<span data-ttu-id="6f003-141">Admin идентификатор профиля регистрации планирует применять на устройство во время следующего регистрации</span><span class="sxs-lookup"><span data-stu-id="6f003-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="6f003-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="6f003-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="6f003-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f003-143">DateTimeOffset</span></span>|<span data-ttu-id="6f003-144">Профиль регистрации времени была назначена на устройство</span><span class="sxs-lookup"><span data-stu-id="6f003-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="6f003-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="6f003-145">isSupervised</span></span>|<span data-ttu-id="6f003-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f003-146">Boolean</span></span>|<span data-ttu-id="6f003-147">Указывает, если управляет устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="6f003-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="6f003-148">Дополнительные сведения о был создан:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="6f003-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="6f003-149">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="6f003-149">discoverySource</span></span>|<span data-ttu-id="6f003-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="6f003-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="6f003-151">Источник обнаружения устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="6f003-151">Apple device discovery source.</span></span> <span data-ttu-id="6f003-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="6f003-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="6f003-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f003-153">createdDateTime</span></span>|<span data-ttu-id="6f003-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f003-154">DateTimeOffset</span></span>|<span data-ttu-id="6f003-155">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="6f003-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="6f003-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f003-156">lastContactedDateTime</span></span>|<span data-ttu-id="6f003-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f003-157">DateTimeOffset</span></span>|<span data-ttu-id="6f003-158">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="6f003-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="6f003-159">описание</span><span class="sxs-lookup"><span data-stu-id="6f003-159">description</span></span>|<span data-ttu-id="6f003-160">String</span><span class="sxs-lookup"><span data-stu-id="6f003-160">String</span></span>|<span data-ttu-id="6f003-161">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="6f003-161">The description of the device</span></span>|
|<span data-ttu-id="6f003-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6f003-162">enrollmentState</span></span>|[<span data-ttu-id="6f003-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="6f003-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="6f003-164">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="6f003-164">The state of the device in Intune.</span></span> <span data-ttu-id="6f003-165">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="6f003-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="6f003-166">platform</span><span class="sxs-lookup"><span data-stu-id="6f003-166">platform</span></span>|[<span data-ttu-id="6f003-167">Платформа</span><span class="sxs-lookup"><span data-stu-id="6f003-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="6f003-168">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="6f003-168">The platform of the Device.</span></span> <span data-ttu-id="6f003-169">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="6f003-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="6f003-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f003-170">Response</span></span>
<span data-ttu-id="6f003-171">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6f003-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f003-172">Пример</span><span class="sxs-lookup"><span data-stu-id="6f003-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f003-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f003-173">Request</span></span>
<span data-ttu-id="6f003-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f003-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 431

{
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

### <a name="response"></a><span data-ttu-id="6f003-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f003-175">Response</span></span>
<span data-ttu-id="6f003-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6f003-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





