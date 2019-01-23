---
title: Создание importedAppleDeviceIdentity
description: Создание нового объекта importedAppleDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 839e604fc52c22ff08a963d5601b987780ee241c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422378"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="ec71d-103">Создание importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ec71d-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="ec71d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ec71d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec71d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec71d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec71d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec71d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec71d-107">Создание нового объекта [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="ec71d-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec71d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ec71d-108">Prerequisites</span></span>
<span data-ttu-id="ec71d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec71d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ec71d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec71d-111">Permission type</span></span>|<span data-ttu-id="ec71d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec71d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec71d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec71d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec71d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec71d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ec71d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec71d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec71d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec71d-116">Not supported.</span></span>|
|<span data-ttu-id="ec71d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec71d-117">Application</span></span>|<span data-ttu-id="ec71d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec71d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec71d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec71d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="ec71d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec71d-120">Request headers</span></span>
|<span data-ttu-id="ec71d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec71d-121">Header</span></span>|<span data-ttu-id="ec71d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ec71d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec71d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec71d-123">Authorization</span></span>|<span data-ttu-id="ec71d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ec71d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec71d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ec71d-125">Accept</span></span>|<span data-ttu-id="ec71d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec71d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec71d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec71d-127">Request body</span></span>
<span data-ttu-id="ec71d-128">В тексте запроса укажите представление JSON для объекта importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="ec71d-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="ec71d-129">В следующей таблице показаны свойства, которые необходимы для создания importedAppleDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="ec71d-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="ec71d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec71d-130">Property</span></span>|<span data-ttu-id="ec71d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ec71d-131">Type</span></span>|<span data-ttu-id="ec71d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ec71d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec71d-133">id</span><span class="sxs-lookup"><span data-stu-id="ec71d-133">id</span></span>|<span data-ttu-id="ec71d-134">String</span><span class="sxs-lookup"><span data-stu-id="ec71d-134">String</span></span>|<span data-ttu-id="ec71d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ec71d-135">Key of the entity.</span></span>|
|<span data-ttu-id="ec71d-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ec71d-136">serialNumber</span></span>|<span data-ttu-id="ec71d-137">String</span><span class="sxs-lookup"><span data-stu-id="ec71d-137">String</span></span>|<span data-ttu-id="ec71d-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="ec71d-138">Device serial number</span></span>|
|<span data-ttu-id="ec71d-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="ec71d-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="ec71d-140">String</span><span class="sxs-lookup"><span data-stu-id="ec71d-140">String</span></span>|<span data-ttu-id="ec71d-141">Admin идентификатор профиля регистрации планирует применять на устройство во время следующего регистрации</span><span class="sxs-lookup"><span data-stu-id="ec71d-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="ec71d-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="ec71d-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="ec71d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec71d-143">DateTimeOffset</span></span>|<span data-ttu-id="ec71d-144">Профиль регистрации времени была назначена на устройство</span><span class="sxs-lookup"><span data-stu-id="ec71d-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="ec71d-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ec71d-145">isSupervised</span></span>|<span data-ttu-id="ec71d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec71d-146">Boolean</span></span>|<span data-ttu-id="ec71d-147">Указывает, если управляет устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="ec71d-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="ec71d-148">Дополнительные сведения о был создан:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="ec71d-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="ec71d-149">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="ec71d-149">discoverySource</span></span>|<span data-ttu-id="ec71d-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="ec71d-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="ec71d-151">Источник обнаружения устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="ec71d-151">Apple device discovery source.</span></span> <span data-ttu-id="ec71d-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="ec71d-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="ec71d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec71d-153">createdDateTime</span></span>|<span data-ttu-id="ec71d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec71d-154">DateTimeOffset</span></span>|<span data-ttu-id="ec71d-155">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="ec71d-155">Created Date Time of the device</span></span>|
|<span data-ttu-id="ec71d-156">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec71d-156">lastContactedDateTime</span></span>|<span data-ttu-id="ec71d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec71d-157">DateTimeOffset</span></span>|<span data-ttu-id="ec71d-158">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="ec71d-158">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="ec71d-159">description</span><span class="sxs-lookup"><span data-stu-id="ec71d-159">description</span></span>|<span data-ttu-id="ec71d-160">String</span><span class="sxs-lookup"><span data-stu-id="ec71d-160">String</span></span>|<span data-ttu-id="ec71d-161">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="ec71d-161">The description of the device</span></span>|
|<span data-ttu-id="ec71d-162">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ec71d-162">enrollmentState</span></span>|[<span data-ttu-id="ec71d-163">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="ec71d-163">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="ec71d-164">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="ec71d-164">The state of the device in Intune.</span></span> <span data-ttu-id="ec71d-165">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="ec71d-165">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ec71d-166">platform</span><span class="sxs-lookup"><span data-stu-id="ec71d-166">platform</span></span>|[<span data-ttu-id="ec71d-167">Платформа</span><span class="sxs-lookup"><span data-stu-id="ec71d-167">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="ec71d-168">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="ec71d-168">The platform of the Device.</span></span> <span data-ttu-id="ec71d-169">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="ec71d-169">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="ec71d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec71d-170">Response</span></span>
<span data-ttu-id="ec71d-171">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ec71d-171">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec71d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="ec71d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec71d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec71d-173">Request</span></span>
<span data-ttu-id="ec71d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec71d-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="ec71d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec71d-175">Response</span></span>
<span data-ttu-id="ec71d-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ec71d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




