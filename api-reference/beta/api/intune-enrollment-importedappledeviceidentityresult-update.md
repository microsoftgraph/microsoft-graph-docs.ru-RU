---
title: Обновление importedAppleDeviceIdentityResult
description: Обновление свойства объекта importedAppleDeviceIdentityResult.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d721da146e86e05b1e99a53c6570a8681adf7a06
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396457"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="d7154-103">Обновление importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="d7154-103">Update importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="d7154-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7154-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d7154-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7154-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7154-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7154-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7154-107">Обновление свойства объекта [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="d7154-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7154-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="d7154-108">Prerequisites</span></span>
<span data-ttu-id="d7154-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7154-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7154-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7154-111">Permission type</span></span>|<span data-ttu-id="d7154-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7154-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7154-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7154-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7154-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7154-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d7154-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7154-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7154-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7154-116">Not supported.</span></span>|
|<span data-ttu-id="d7154-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7154-117">Application</span></span>|<span data-ttu-id="d7154-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7154-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7154-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7154-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="d7154-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7154-120">Request headers</span></span>
|<span data-ttu-id="d7154-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7154-121">Header</span></span>|<span data-ttu-id="d7154-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7154-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7154-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7154-123">Authorization</span></span>|<span data-ttu-id="d7154-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d7154-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7154-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7154-125">Accept</span></span>|<span data-ttu-id="d7154-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7154-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7154-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7154-127">Request body</span></span>
<span data-ttu-id="d7154-128">В тексте запроса укажите представление JSON для объекта [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="d7154-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="d7154-129">В следующей таблице показаны свойства, которые необходимы для создания [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="d7154-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="d7154-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7154-130">Property</span></span>|<span data-ttu-id="d7154-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7154-131">Type</span></span>|<span data-ttu-id="d7154-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7154-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7154-133">id</span><span class="sxs-lookup"><span data-stu-id="d7154-133">id</span></span>|<span data-ttu-id="d7154-134">String</span><span class="sxs-lookup"><span data-stu-id="d7154-134">String</span></span>|<span data-ttu-id="d7154-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7154-135">Key of the entity.</span></span> <span data-ttu-id="d7154-136">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d7154-137">serialNumber</span></span>|<span data-ttu-id="d7154-138">String</span><span class="sxs-lookup"><span data-stu-id="d7154-138">String</span></span>|<span data-ttu-id="d7154-139">Серийный номер устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="d7154-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="d7154-141">String</span><span class="sxs-lookup"><span data-stu-id="d7154-141">String</span></span>|<span data-ttu-id="d7154-142">Идентификатор администрирования профилей регистрации предполагаются для применения к устройства во время следующего регистрации унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="d7154-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="d7154-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7154-144">DateTimeOffset</span></span>|<span data-ttu-id="d7154-145">Профиль регистрации времени была назначена на устройство Inherited из [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d7154-146">isSupervised</span></span>|<span data-ttu-id="d7154-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7154-147">Boolean</span></span>|<span data-ttu-id="d7154-148">Указывает, если управляет устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="d7154-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="d7154-149">Дополнительные сведения о был создан: https://support.apple.com/en-us/HT202837 наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-150">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="d7154-150">discoverySource</span></span>|<span data-ttu-id="d7154-151">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="d7154-151">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="d7154-152">Источник обнаружения устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="d7154-152">Apple device discovery source.</span></span> <span data-ttu-id="d7154-153">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d7154-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="d7154-154">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="d7154-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="d7154-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7154-155">createdDateTime</span></span>|<span data-ttu-id="d7154-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7154-156">DateTimeOffset</span></span>|<span data-ttu-id="d7154-157">Созданные Дата и время устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7154-158">lastContactedDateTime</span></span>|<span data-ttu-id="d7154-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7154-159">DateTimeOffset</span></span>|<span data-ttu-id="d7154-160">Связаться с даты последнего устройства, унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-161">description</span><span class="sxs-lookup"><span data-stu-id="d7154-161">description</span></span>|<span data-ttu-id="d7154-162">String</span><span class="sxs-lookup"><span data-stu-id="d7154-162">String</span></span>|<span data-ttu-id="d7154-163">Описание устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d7154-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="d7154-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d7154-164">enrollmentState</span></span>|[<span data-ttu-id="d7154-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="d7154-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d7154-166">Состояние устройства в Intune наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d7154-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="d7154-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="d7154-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d7154-168">platform</span><span class="sxs-lookup"><span data-stu-id="d7154-168">platform</span></span>|[<span data-ttu-id="d7154-169">Платформа</span><span class="sxs-lookup"><span data-stu-id="d7154-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d7154-170">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="d7154-170">The platform of the Device.</span></span> <span data-ttu-id="d7154-171">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d7154-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="d7154-172">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="d7154-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="d7154-173">status</span><span class="sxs-lookup"><span data-stu-id="d7154-173">status</span></span>|<span data-ttu-id="d7154-174">Логический</span><span class="sxs-lookup"><span data-stu-id="d7154-174">Boolean</span></span>|<span data-ttu-id="d7154-175">Состояние импортированных устройств удостоверений</span><span class="sxs-lookup"><span data-stu-id="d7154-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="d7154-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7154-176">Response</span></span>
<span data-ttu-id="d7154-177">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d7154-177">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7154-178">Пример</span><span class="sxs-lookup"><span data-stu-id="d7154-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7154-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7154-179">Request</span></span>
<span data-ttu-id="d7154-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7154-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7154-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7154-181">Response</span></span>
<span data-ttu-id="d7154-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7154-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




