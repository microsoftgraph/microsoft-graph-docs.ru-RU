---
title: Обновление importedAppleDeviceIdentity
description: Обновление свойства объекта importedAppleDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7970c0c74c7200d6a991a48f986125747589195c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412172"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="c3881-103">Обновление importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="c3881-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="c3881-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3881-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c3881-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3881-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3881-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3881-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3881-107">Обновление свойства объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="c3881-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3881-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c3881-108">Prerequisites</span></span>
<span data-ttu-id="c3881-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3881-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c3881-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3881-111">Permission type</span></span>|<span data-ttu-id="c3881-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3881-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3881-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3881-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3881-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3881-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c3881-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3881-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3881-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3881-116">Not supported.</span></span>|
|<span data-ttu-id="c3881-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3881-117">Application</span></span>|<span data-ttu-id="c3881-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3881-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3881-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3881-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="c3881-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3881-120">Request headers</span></span>
|<span data-ttu-id="c3881-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3881-121">Header</span></span>|<span data-ttu-id="c3881-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3881-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3881-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3881-123">Authorization</span></span>|<span data-ttu-id="c3881-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c3881-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3881-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3881-125">Accept</span></span>|<span data-ttu-id="c3881-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3881-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3881-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3881-127">Request body</span></span>
<span data-ttu-id="c3881-128">В тексте запроса укажите представление JSON для объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="c3881-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="c3881-129">В следующей таблице показаны свойства, которые необходимы для создания [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="c3881-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="c3881-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3881-130">Property</span></span>|<span data-ttu-id="c3881-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3881-131">Type</span></span>|<span data-ttu-id="c3881-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3881-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3881-133">id</span><span class="sxs-lookup"><span data-stu-id="c3881-133">id</span></span>|<span data-ttu-id="c3881-134">String</span><span class="sxs-lookup"><span data-stu-id="c3881-134">String</span></span>|<span data-ttu-id="c3881-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3881-135">Key of the entity.</span></span>|
|<span data-ttu-id="c3881-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c3881-136">serialNumber</span></span>|<span data-ttu-id="c3881-137">String</span><span class="sxs-lookup"><span data-stu-id="c3881-137">String</span></span>|<span data-ttu-id="c3881-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="c3881-138">Device serial number</span></span>|
|<span data-ttu-id="c3881-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="c3881-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="c3881-140">String</span><span class="sxs-lookup"><span data-stu-id="c3881-140">String</span></span>|<span data-ttu-id="c3881-141">Admin идентификатор профиля регистрации планирует применять на устройство во время следующего регистрации</span><span class="sxs-lookup"><span data-stu-id="c3881-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="c3881-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="c3881-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="c3881-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3881-143">DateTimeOffset</span></span>|<span data-ttu-id="c3881-144">Профиль регистрации времени была назначена на устройство</span><span class="sxs-lookup"><span data-stu-id="c3881-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="c3881-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="c3881-145">isSupervised</span></span>|<span data-ttu-id="c3881-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3881-146">Boolean</span></span>|<span data-ttu-id="c3881-147">Указывает, если управляет устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="c3881-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="c3881-148">Дополнительные сведения о был создан:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="c3881-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="c3881-149">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="c3881-149">discoverySource</span></span>|<span data-ttu-id="c3881-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="c3881-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="c3881-151">Источник обнаружения устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="c3881-151">Apple device discovery source.</span></span> <span data-ttu-id="c3881-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="c3881-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="c3881-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3881-153">createdDateTime</span></span>|<span data-ttu-id="c3881-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3881-154">DateTimeOffset</span></span>|<span data-ttu-id="c3881-155">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="c3881-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="c3881-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3881-156">lastContactedDateTime</span></span>|<span data-ttu-id="c3881-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3881-157">DateTimeOffset</span></span>|<span data-ttu-id="c3881-158">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="c3881-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="c3881-159">description</span><span class="sxs-lookup"><span data-stu-id="c3881-159">description</span></span>|<span data-ttu-id="c3881-160">String</span><span class="sxs-lookup"><span data-stu-id="c3881-160">String</span></span>|<span data-ttu-id="c3881-161">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="c3881-161">The description of the device</span></span>|
|<span data-ttu-id="c3881-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c3881-162">enrollmentState</span></span>|[<span data-ttu-id="c3881-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="c3881-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="c3881-164">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="c3881-164">The state of the device in Intune.</span></span> <span data-ttu-id="c3881-165">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="c3881-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="c3881-166">platform</span><span class="sxs-lookup"><span data-stu-id="c3881-166">platform</span></span>|[<span data-ttu-id="c3881-167">Платформа</span><span class="sxs-lookup"><span data-stu-id="c3881-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="c3881-168">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="c3881-168">The platform of the Device.</span></span> <span data-ttu-id="c3881-169">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="c3881-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="c3881-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3881-170">Response</span></span>
<span data-ttu-id="c3881-171">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3881-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3881-172">Пример</span><span class="sxs-lookup"><span data-stu-id="c3881-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3881-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3881-173">Request</span></span>
<span data-ttu-id="c3881-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3881-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3881-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3881-175">Response</span></span>
<span data-ttu-id="c3881-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c3881-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




