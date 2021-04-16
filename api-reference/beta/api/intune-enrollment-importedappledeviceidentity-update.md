---
title: Обновление импортируемогоAppleDeviceIdentity
description: Обновление свойств объекта importedAppleDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5c280965a3624bd86fc91290b9a517c89986c0aa
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867569"
---
# <a name="update-importedappledeviceidentity"></a><span data-ttu-id="b3a01-103">Обновление импортируемогоAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b3a01-103">Update importedAppleDeviceIdentity</span></span>

<span data-ttu-id="b3a01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3a01-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3a01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3a01-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3a01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3a01-107">Обновление свойств объекта [importedAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b3a01-107">Update the properties of a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3a01-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b3a01-108">Prerequisites</span></span>
<span data-ttu-id="b3a01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3a01-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3a01-111">Permission type</span></span>|<span data-ttu-id="b3a01-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3a01-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3a01-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3a01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3a01-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3a01-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3a01-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3a01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3a01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3a01-116">Not supported.</span></span>|
|<span data-ttu-id="b3a01-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b3a01-117">Application</span></span>|<span data-ttu-id="b3a01-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3a01-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3a01-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3a01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="b3a01-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b3a01-120">Request headers</span></span>
|<span data-ttu-id="b3a01-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3a01-121">Header</span></span>|<span data-ttu-id="b3a01-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3a01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3a01-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3a01-123">Authorization</span></span>|<span data-ttu-id="b3a01-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3a01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3a01-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3a01-125">Accept</span></span>|<span data-ttu-id="b3a01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3a01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3a01-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3a01-127">Request body</span></span>
<span data-ttu-id="b3a01-128">В теле запроса поставляем представление JSON для объекта [importedAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b3a01-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

<span data-ttu-id="b3a01-129">В следующей таблице показаны свойства, необходимые при создании объекта [importedAppleDeviceId.](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b3a01-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span>

|<span data-ttu-id="b3a01-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3a01-130">Property</span></span>|<span data-ttu-id="b3a01-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b3a01-131">Type</span></span>|<span data-ttu-id="b3a01-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b3a01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3a01-133">id</span><span class="sxs-lookup"><span data-stu-id="b3a01-133">id</span></span>|<span data-ttu-id="b3a01-134">String</span><span class="sxs-lookup"><span data-stu-id="b3a01-134">String</span></span>|<span data-ttu-id="b3a01-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b3a01-135">Key of the entity.</span></span>|
|<span data-ttu-id="b3a01-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b3a01-136">serialNumber</span></span>|<span data-ttu-id="b3a01-137">String</span><span class="sxs-lookup"><span data-stu-id="b3a01-137">String</span></span>|<span data-ttu-id="b3a01-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="b3a01-138">Device serial number</span></span>|
|<span data-ttu-id="b3a01-139">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="b3a01-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="b3a01-140">String</span><span class="sxs-lookup"><span data-stu-id="b3a01-140">String</span></span>|<span data-ttu-id="b3a01-141">Администратор ID профиля регистрации намерен примениться к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="b3a01-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="b3a01-142">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="b3a01-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="b3a01-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3a01-143">DateTimeOffset</span></span>|<span data-ttu-id="b3a01-144">Профиль времени регистрации был назначен устройству</span><span class="sxs-lookup"><span data-stu-id="b3a01-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="b3a01-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="b3a01-145">isSupervised</span></span>|<span data-ttu-id="b3a01-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3a01-146">Boolean</span></span>|<span data-ttu-id="b3a01-147">Указывает, контролируется ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="b3a01-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="b3a01-148">Дополнительные сведения можно получить по: https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="b3a01-148">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="b3a01-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="b3a01-149">discoverySource</span></span>|<span data-ttu-id="b3a01-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="b3a01-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="b3a01-151">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="b3a01-151">Apple device discovery source.</span></span> <span data-ttu-id="b3a01-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="b3a01-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="b3a01-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b3a01-153">isDeleted</span></span>|<span data-ttu-id="b3a01-154">Логический</span><span class="sxs-lookup"><span data-stu-id="b3a01-154">Boolean</span></span>|<span data-ttu-id="b3a01-155">Указывает, удалено ли устройство из Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="b3a01-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="b3a01-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3a01-156">createdDateTime</span></span>|<span data-ttu-id="b3a01-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3a01-157">DateTimeOffset</span></span>|<span data-ttu-id="b3a01-158">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="b3a01-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="b3a01-159">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3a01-159">lastContactedDateTime</span></span>|<span data-ttu-id="b3a01-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3a01-160">DateTimeOffset</span></span>|<span data-ttu-id="b3a01-161">Время последней контактной даты устройства</span><span class="sxs-lookup"><span data-stu-id="b3a01-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="b3a01-162">description</span><span class="sxs-lookup"><span data-stu-id="b3a01-162">description</span></span>|<span data-ttu-id="b3a01-163">String</span><span class="sxs-lookup"><span data-stu-id="b3a01-163">String</span></span>|<span data-ttu-id="b3a01-164">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="b3a01-164">The description of the device</span></span>|
|<span data-ttu-id="b3a01-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="b3a01-165">enrollmentState</span></span>|[<span data-ttu-id="b3a01-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="b3a01-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="b3a01-167">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="b3a01-167">The state of the device in Intune.</span></span> <span data-ttu-id="b3a01-168">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="b3a01-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="b3a01-169">платформа</span><span class="sxs-lookup"><span data-stu-id="b3a01-169">platform</span></span>|[<span data-ttu-id="b3a01-170">платформа</span><span class="sxs-lookup"><span data-stu-id="b3a01-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="b3a01-171">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="b3a01-171">The platform of the Device.</span></span> <span data-ttu-id="b3a01-172">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="b3a01-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="b3a01-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3a01-173">Response</span></span>
<span data-ttu-id="b3a01-174">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b3a01-174">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3a01-175">Пример</span><span class="sxs-lookup"><span data-stu-id="b3a01-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3a01-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3a01-176">Request</span></span>
<span data-ttu-id="b3a01-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3a01-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3a01-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3a01-178">Response</span></span>
<span data-ttu-id="b3a01-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3a01-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




