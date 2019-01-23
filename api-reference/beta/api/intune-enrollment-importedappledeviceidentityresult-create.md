---
title: Создание importedAppleDeviceIdentityResult
description: Создание нового объекта importedAppleDeviceIdentityResult.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bd48716e7268997305a5b8840beacbab9106cf42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417730"
---
# <a name="create-importedappledeviceidentityresult"></a><span data-ttu-id="21597-103">Создание importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="21597-103">Create importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="21597-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21597-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21597-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21597-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21597-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21597-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21597-107">Создание нового объекта [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="21597-107">Create a new [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21597-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="21597-108">Prerequisites</span></span>
<span data-ttu-id="21597-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="21597-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21597-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21597-111">Permission type</span></span>|<span data-ttu-id="21597-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21597-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21597-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21597-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21597-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21597-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21597-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21597-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21597-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21597-116">Not supported.</span></span>|
|<span data-ttu-id="21597-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21597-117">Application</span></span>|<span data-ttu-id="21597-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21597-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21597-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21597-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="21597-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21597-120">Request headers</span></span>
|<span data-ttu-id="21597-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21597-121">Header</span></span>|<span data-ttu-id="21597-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21597-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21597-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21597-123">Authorization</span></span>|<span data-ttu-id="21597-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="21597-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21597-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21597-125">Accept</span></span>|<span data-ttu-id="21597-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21597-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21597-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21597-127">Request body</span></span>
<span data-ttu-id="21597-128">В тексте запроса укажите представление JSON для объекта importedAppleDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="21597-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.</span></span>

<span data-ttu-id="21597-129">В следующей таблице показаны свойства, которые необходимы для создания importedAppleDeviceIdentityResult.</span><span class="sxs-lookup"><span data-stu-id="21597-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.</span></span>

|<span data-ttu-id="21597-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="21597-130">Property</span></span>|<span data-ttu-id="21597-131">Тип</span><span class="sxs-lookup"><span data-stu-id="21597-131">Type</span></span>|<span data-ttu-id="21597-132">Описание</span><span class="sxs-lookup"><span data-stu-id="21597-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21597-133">id</span><span class="sxs-lookup"><span data-stu-id="21597-133">id</span></span>|<span data-ttu-id="21597-134">String</span><span class="sxs-lookup"><span data-stu-id="21597-134">String</span></span>|<span data-ttu-id="21597-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21597-135">Key of the entity.</span></span> <span data-ttu-id="21597-136">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="21597-137">serialNumber</span></span>|<span data-ttu-id="21597-138">String</span><span class="sxs-lookup"><span data-stu-id="21597-138">String</span></span>|<span data-ttu-id="21597-139">Серийный номер устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="21597-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="21597-141">String</span><span class="sxs-lookup"><span data-stu-id="21597-141">String</span></span>|<span data-ttu-id="21597-142">Идентификатор администрирования профилей регистрации предполагаются для применения к устройства во время следующего регистрации унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="21597-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="21597-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21597-144">DateTimeOffset</span></span>|<span data-ttu-id="21597-145">Профиль регистрации времени была назначена на устройство Inherited из [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="21597-146">isSupervised</span></span>|<span data-ttu-id="21597-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="21597-147">Boolean</span></span>|<span data-ttu-id="21597-148">Указывает, если управляет устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="21597-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="21597-149">Дополнительные сведения о был создан: https://support.apple.com/en-us/HT202837 наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-150">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="21597-150">discoverySource</span></span>|<span data-ttu-id="21597-151">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="21597-151">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="21597-152">Источник обнаружения устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="21597-152">Apple device discovery source.</span></span> <span data-ttu-id="21597-153">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="21597-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="21597-154">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="21597-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="21597-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21597-155">createdDateTime</span></span>|<span data-ttu-id="21597-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21597-156">DateTimeOffset</span></span>|<span data-ttu-id="21597-157">Созданные Дата и время устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-157">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-158">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="21597-158">lastContactedDateTime</span></span>|<span data-ttu-id="21597-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21597-159">DateTimeOffset</span></span>|<span data-ttu-id="21597-160">Связаться с даты последнего устройства, унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-160">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-161">description</span><span class="sxs-lookup"><span data-stu-id="21597-161">description</span></span>|<span data-ttu-id="21597-162">String</span><span class="sxs-lookup"><span data-stu-id="21597-162">String</span></span>|<span data-ttu-id="21597-163">Описание устройства унаследованные от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="21597-163">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="21597-164">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="21597-164">enrollmentState</span></span>|[<span data-ttu-id="21597-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="21597-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="21597-166">Состояние устройства в Intune наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="21597-166">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="21597-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="21597-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="21597-168">platform</span><span class="sxs-lookup"><span data-stu-id="21597-168">platform</span></span>|[<span data-ttu-id="21597-169">Платформа</span><span class="sxs-lookup"><span data-stu-id="21597-169">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="21597-170">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="21597-170">The platform of the Device.</span></span> <span data-ttu-id="21597-171">Наследуется от [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="21597-171">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="21597-172">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="21597-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="21597-173">status</span><span class="sxs-lookup"><span data-stu-id="21597-173">status</span></span>|<span data-ttu-id="21597-174">Логический</span><span class="sxs-lookup"><span data-stu-id="21597-174">Boolean</span></span>|<span data-ttu-id="21597-175">Состояние импортированных устройств удостоверений</span><span class="sxs-lookup"><span data-stu-id="21597-175">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="21597-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="21597-176">Response</span></span>
<span data-ttu-id="21597-177">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="21597-177">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21597-178">Пример</span><span class="sxs-lookup"><span data-stu-id="21597-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="21597-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="21597-179">Request</span></span>
<span data-ttu-id="21597-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21597-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="21597-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="21597-181">Response</span></span>
<span data-ttu-id="21597-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="21597-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




