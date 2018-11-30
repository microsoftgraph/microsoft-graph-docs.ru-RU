---
title: Обновление importedAppleDeviceIdentityResult
description: Обновление свойства объекта importedAppleDeviceIdentityResult.
ms.openlocfilehash: 1c631a37a4f4df7a82093402ce323ad272c04f11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079132"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="72d99-103">Обновление importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="72d99-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="72d99-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72d99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72d99-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72d99-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="72d99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72d99-107">Обновление свойства объекта [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="72d99-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72d99-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72d99-108">Prerequisites</span></span>
<span data-ttu-id="72d99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72d99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72d99-111">Permission type</span></span>|<span data-ttu-id="72d99-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72d99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72d99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72d99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72d99-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d99-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="72d99-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72d99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72d99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d99-116">Not supported.</span></span>|
|<span data-ttu-id="72d99-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72d99-117">Application</span></span>|<span data-ttu-id="72d99-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d99-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72d99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72d99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="72d99-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72d99-120">Request headers</span></span>
|<span data-ttu-id="72d99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72d99-121">Header</span></span>|<span data-ttu-id="72d99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72d99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72d99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72d99-123">Authorization</span></span>|<span data-ttu-id="72d99-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="72d99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72d99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72d99-125">Accept</span></span>|<span data-ttu-id="72d99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72d99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72d99-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72d99-127">Request body</span></span>
<span data-ttu-id="72d99-128">В тексте запроса укажите представление JSON для объекта [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="72d99-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="72d99-129">В следующей таблице показаны свойства, которые необходимы для создания [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="72d99-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="72d99-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72d99-130">Property</span></span>|<span data-ttu-id="72d99-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72d99-131">Type</span></span>|<span data-ttu-id="72d99-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72d99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72d99-133">id</span><span class="sxs-lookup"><span data-stu-id="72d99-133">id</span></span>|<span data-ttu-id="72d99-134">String</span><span class="sxs-lookup"><span data-stu-id="72d99-134">String</span></span>|<span data-ttu-id="72d99-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72d99-135">Key of the entity.</span></span> <span data-ttu-id="72d99-136">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="72d99-137">serialNumber</span></span>|<span data-ttu-id="72d99-138">String</span><span class="sxs-lookup"><span data-stu-id="72d99-138">String</span></span>|<span data-ttu-id="72d99-139">Серийный номер устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="72d99-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="72d99-141">String</span><span class="sxs-lookup"><span data-stu-id="72d99-141">String</span></span>|<span data-ttu-id="72d99-142">Идентификатор администрирования профилей регистрации предполагаются для применения к устройства во время следующего регистрации унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="72d99-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="72d99-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72d99-144">DateTimeOffset</span></span>|<span data-ttu-id="72d99-145">Профиль регистрации времени была назначена на устройство Inherited из [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="72d99-146">isSupervised</span></span>|<span data-ttu-id="72d99-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="72d99-147">Boolean</span></span>|<span data-ttu-id="72d99-148">Указывает, если управляет устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="72d99-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="72d99-149">Дополнительные сведения о был создан: https://support.apple.com/en-us/HT202837 наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-150">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="72d99-150">discoverySource</span></span>|<span data-ttu-id="72d99-151">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="72d99-151">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="72d99-152">Источник обнаружения устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="72d99-152">Apple device discovery source.</span></span> <span data-ttu-id="72d99-153">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="72d99-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="72d99-154">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="72d99-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="72d99-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72d99-155">createdDateTime</span></span>|<span data-ttu-id="72d99-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72d99-156">DateTimeOffset</span></span>|<span data-ttu-id="72d99-157">Созданные Дата и время устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="72d99-158">lastContactedDateTime</span></span>|<span data-ttu-id="72d99-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72d99-159">DateTimeOffset</span></span>|<span data-ttu-id="72d99-160">Связаться с даты последнего устройства, унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-161">описание</span><span class="sxs-lookup"><span data-stu-id="72d99-161">description</span></span>|<span data-ttu-id="72d99-162">String</span><span class="sxs-lookup"><span data-stu-id="72d99-162">String</span></span>|<span data-ttu-id="72d99-163">Описание устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="72d99-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="72d99-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="72d99-164">enrollmentState</span></span>|[<span data-ttu-id="72d99-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="72d99-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="72d99-166">Состояние устройства в Intune наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="72d99-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="72d99-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="72d99-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="72d99-168">platform</span><span class="sxs-lookup"><span data-stu-id="72d99-168">platform</span></span>|[<span data-ttu-id="72d99-169">Платформа</span><span class="sxs-lookup"><span data-stu-id="72d99-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="72d99-170">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="72d99-170">The platform of the Device.</span></span> <span data-ttu-id="72d99-171">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="72d99-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="72d99-172">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="72d99-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="72d99-173">status</span><span class="sxs-lookup"><span data-stu-id="72d99-173">status</span></span>|<span data-ttu-id="72d99-174">Логический</span><span class="sxs-lookup"><span data-stu-id="72d99-174">Boolean</span></span>|<span data-ttu-id="72d99-175">Состояние импортированных устройств удостоверений</span><span class="sxs-lookup"><span data-stu-id="72d99-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="72d99-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="72d99-176">Response</span></span>
<span data-ttu-id="72d99-177">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="72d99-177">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72d99-178">Пример</span><span class="sxs-lookup"><span data-stu-id="72d99-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="72d99-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="72d99-179">Request</span></span>
<span data-ttu-id="72d99-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72d99-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 450

{
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

### <a name="response"></a><span data-ttu-id="72d99-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="72d99-181">Response</span></span>
<span data-ttu-id="72d99-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="72d99-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





