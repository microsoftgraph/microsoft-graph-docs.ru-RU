---
title: Обновление importedAppleDeviceIdentity
description: Обновление свойства объекта importedAppleDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 53f80608d2236b1afe6d7f9f80c5e4816d76ec50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990987"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="a1ef0-103">Обновление importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a1ef0-103">Update importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="a1ef0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1ef0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1ef0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1ef0-107">Обновление свойства объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a1ef0-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1ef0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1ef0-108">Prerequisites</span></span>
<span data-ttu-id="a1ef0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1ef0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1ef0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1ef0-111">Permission type</span></span>|<span data-ttu-id="a1ef0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1ef0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1ef0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1ef0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1ef0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1ef0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1ef0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1ef0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1ef0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-116">Not supported.</span></span>|
|<span data-ttu-id="a1ef0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1ef0-117">Application</span></span>|<span data-ttu-id="a1ef0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1ef0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1ef0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a1ef0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1ef0-120">Request headers</span></span>
|<span data-ttu-id="a1ef0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1ef0-121">Header</span></span>|<span data-ttu-id="a1ef0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a1ef0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1ef0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1ef0-123">Authorization</span></span>|<span data-ttu-id="a1ef0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a1ef0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1ef0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1ef0-125">Accept</span></span>|<span data-ttu-id="a1ef0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1ef0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1ef0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1ef0-127">Request body</span></span>
<span data-ttu-id="a1ef0-128">В тексте запроса укажите представление JSON для объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a1ef0-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="a1ef0-129">В следующей таблице показаны свойства, которые необходимы для создания [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a1ef0-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="a1ef0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1ef0-130">Property</span></span>|<span data-ttu-id="a1ef0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a1ef0-131">Type</span></span>|<span data-ttu-id="a1ef0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a1ef0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ef0-133">id</span><span class="sxs-lookup"><span data-stu-id="a1ef0-133">id</span></span>|<span data-ttu-id="a1ef0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ef0-134">String</span></span>|<span data-ttu-id="a1ef0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-135">Key of the entity.</span></span>|
|<span data-ttu-id="a1ef0-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a1ef0-136">serialNumber</span></span>|<span data-ttu-id="a1ef0-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ef0-137">String</span></span>|<span data-ttu-id="a1ef0-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="a1ef0-138">Device serial number</span></span>|
|<span data-ttu-id="a1ef0-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="a1ef0-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="a1ef0-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ef0-140">String</span></span>|<span data-ttu-id="a1ef0-141">Admin идентификатор профиля регистрации планирует применять на устройство во время следующего регистрации</span><span class="sxs-lookup"><span data-stu-id="a1ef0-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="a1ef0-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="a1ef0-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="a1ef0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1ef0-143">DateTimeOffset</span></span>|<span data-ttu-id="a1ef0-144">Профиль регистрации времени была назначена на устройство</span><span class="sxs-lookup"><span data-stu-id="a1ef0-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="a1ef0-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a1ef0-145">isSupervised</span></span>|<span data-ttu-id="a1ef0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1ef0-146">Boolean</span></span>|<span data-ttu-id="a1ef0-147">Указывает, если управляет устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="a1ef0-148">Дополнительные сведения о был создан:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="a1ef0-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="a1ef0-149">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="a1ef0-149">discoverySource</span></span>|<span data-ttu-id="a1ef0-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="a1ef0-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="a1ef0-151">Источник обнаружения устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-151">Apple device discovery source.</span></span> <span data-ttu-id="a1ef0-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="a1ef0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1ef0-153">createdDateTime</span></span>|<span data-ttu-id="a1ef0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1ef0-154">DateTimeOffset</span></span>|<span data-ttu-id="a1ef0-155">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="a1ef0-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="a1ef0-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1ef0-156">lastContactedDateTime</span></span>|<span data-ttu-id="a1ef0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1ef0-157">DateTimeOffset</span></span>|<span data-ttu-id="a1ef0-158">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="a1ef0-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="a1ef0-159">описание</span><span class="sxs-lookup"><span data-stu-id="a1ef0-159">description</span></span>|<span data-ttu-id="a1ef0-160">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ef0-160">String</span></span>|<span data-ttu-id="a1ef0-161">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="a1ef0-161">The description of the device</span></span>|
|<span data-ttu-id="a1ef0-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a1ef0-162">enrollmentState</span></span>|[<span data-ttu-id="a1ef0-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="a1ef0-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="a1ef0-164">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-164">The state of the device in Intune.</span></span> <span data-ttu-id="a1ef0-165">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a1ef0-166">platform</span><span class="sxs-lookup"><span data-stu-id="a1ef0-166">platform</span></span>|[<span data-ttu-id="a1ef0-167">Платформа</span><span class="sxs-lookup"><span data-stu-id="a1ef0-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="a1ef0-168">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-168">The platform of the Device.</span></span> <span data-ttu-id="a1ef0-169">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1ef0-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1ef0-170">Response</span></span>
<span data-ttu-id="a1ef0-171">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-171">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1ef0-172">Пример</span><span class="sxs-lookup"><span data-stu-id="a1ef0-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1ef0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1ef0-173">Request</span></span>
<span data-ttu-id="a1ef0-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1ef0-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1ef0-175">Response</span></span>
<span data-ttu-id="a1ef0-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a1ef0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





