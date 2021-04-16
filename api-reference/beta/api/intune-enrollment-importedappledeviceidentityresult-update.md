---
title: Обновление importedAppleDeviceIdentityResult
description: Обновление свойств импортируемого объектаAppleDeviceIdentityResult.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f0db5a3ed08c54e7036e82a22f9e5658aa04ace
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868206"
---
# <a name="update-importedappledeviceidentityresult"></a><span data-ttu-id="57d24-103">Обновление importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="57d24-103">Update importedAppleDeviceIdentityResult</span></span>

<span data-ttu-id="57d24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57d24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57d24-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57d24-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57d24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57d24-107">Обновление свойств импортируемого [объектаAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-107">Update the properties of a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57d24-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="57d24-108">Prerequisites</span></span>
<span data-ttu-id="57d24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57d24-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57d24-111">Permission type</span></span>|<span data-ttu-id="57d24-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57d24-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57d24-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57d24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57d24-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d24-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="57d24-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57d24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57d24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d24-116">Not supported.</span></span>|
|<span data-ttu-id="57d24-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="57d24-117">Application</span></span>|<span data-ttu-id="57d24-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d24-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57d24-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57d24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="57d24-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57d24-120">Request headers</span></span>
|<span data-ttu-id="57d24-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57d24-121">Header</span></span>|<span data-ttu-id="57d24-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57d24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57d24-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57d24-123">Authorization</span></span>|<span data-ttu-id="57d24-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57d24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57d24-125">Accept</span></span>|<span data-ttu-id="57d24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57d24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57d24-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57d24-127">Request body</span></span>
<span data-ttu-id="57d24-128">В теле запроса поставляем представление JSON для объекта [importedAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-128">In the request body, supply a JSON representation for the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>

<span data-ttu-id="57d24-129">В следующей таблице показаны свойства, необходимые при создании [импортируемогоAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-129">The following table shows the properties that are required when you create the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>

|<span data-ttu-id="57d24-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="57d24-130">Property</span></span>|<span data-ttu-id="57d24-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57d24-131">Type</span></span>|<span data-ttu-id="57d24-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57d24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57d24-133">id</span><span class="sxs-lookup"><span data-stu-id="57d24-133">id</span></span>|<span data-ttu-id="57d24-134">String</span><span class="sxs-lookup"><span data-stu-id="57d24-134">String</span></span>|<span data-ttu-id="57d24-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57d24-135">Key of the entity.</span></span> <span data-ttu-id="57d24-136">Унаследованный от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-136">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="57d24-137">serialNumber</span></span>|<span data-ttu-id="57d24-138">String</span><span class="sxs-lookup"><span data-stu-id="57d24-138">String</span></span>|<span data-ttu-id="57d24-139">Серийный номер устройства, унаследованный от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-139">Device serial number Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-140">requestedEnrollmentProfileId</span><span class="sxs-lookup"><span data-stu-id="57d24-140">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="57d24-141">String</span><span class="sxs-lookup"><span data-stu-id="57d24-141">String</span></span>|<span data-ttu-id="57d24-142">Администратор ID профиля регистрации намерен применить к устройству во время следующей регистрации, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-142">Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-143">requestedEnrollmentProfileAssignmentDateTime</span><span class="sxs-lookup"><span data-stu-id="57d24-143">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="57d24-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57d24-144">DateTimeOffset</span></span>|<span data-ttu-id="57d24-145">Профиль времени регистрации назначен устройству, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-145">The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-146">isSupervised</span><span class="sxs-lookup"><span data-stu-id="57d24-146">isSupervised</span></span>|<span data-ttu-id="57d24-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="57d24-147">Boolean</span></span>|<span data-ttu-id="57d24-148">Указывает, контролируется ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="57d24-148">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="57d24-149">Дополнительные сведения: https://support.apple.com/en-us/HT202837 Унаследованные от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-149">More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-150">discoverySource</span><span class="sxs-lookup"><span data-stu-id="57d24-150">discoverySource</span></span>|<span data-ttu-id="57d24-151">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="57d24-151">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="57d24-152">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="57d24-152">Apple device discovery source.</span></span> <span data-ttu-id="57d24-153">Наследуется [от импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="57d24-153">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="57d24-154">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="57d24-154">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="57d24-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="57d24-155">isDeleted</span></span>|<span data-ttu-id="57d24-156">Логический</span><span class="sxs-lookup"><span data-stu-id="57d24-156">Boolean</span></span>|<span data-ttu-id="57d24-157">Указывает, удалено ли устройство из подразделения Apple Business Manager, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-157">Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57d24-158">createdDateTime</span></span>|<span data-ttu-id="57d24-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57d24-159">DateTimeOffset</span></span>|<span data-ttu-id="57d24-160">Создано время даты устройства, унаследованной от [импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-160">Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-161">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="57d24-161">lastContactedDateTime</span></span>|<span data-ttu-id="57d24-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57d24-162">DateTimeOffset</span></span>|<span data-ttu-id="57d24-163">Время последней контактируемой даты устройства, унаследованной от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-163">Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-164">description</span><span class="sxs-lookup"><span data-stu-id="57d24-164">description</span></span>|<span data-ttu-id="57d24-165">String</span><span class="sxs-lookup"><span data-stu-id="57d24-165">String</span></span>|<span data-ttu-id="57d24-166">Описание устройства, унаследованной от [импортируемого ОбъектаAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-166">The description of the device Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)</span></span>|
|<span data-ttu-id="57d24-167">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="57d24-167">enrollmentState</span></span>|[<span data-ttu-id="57d24-168">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="57d24-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="57d24-169">Состояние устройства в Intune Наследуется от [импортируемогоAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="57d24-169">The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="57d24-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="57d24-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="57d24-171">платформа</span><span class="sxs-lookup"><span data-stu-id="57d24-171">platform</span></span>|[<span data-ttu-id="57d24-172">платформа</span><span class="sxs-lookup"><span data-stu-id="57d24-172">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="57d24-173">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="57d24-173">The platform of the Device.</span></span> <span data-ttu-id="57d24-174">Наследуется [от импортируемогоAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="57d24-174">Inherited from [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).</span></span> <span data-ttu-id="57d24-175">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="57d24-175">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="57d24-176">status</span><span class="sxs-lookup"><span data-stu-id="57d24-176">status</span></span>|<span data-ttu-id="57d24-177">Логический</span><span class="sxs-lookup"><span data-stu-id="57d24-177">Boolean</span></span>|<span data-ttu-id="57d24-178">Состояние удостоверения импортируемого устройства</span><span class="sxs-lookup"><span data-stu-id="57d24-178">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="57d24-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d24-179">Response</span></span>
<span data-ttu-id="57d24-180">В случае успешной работы этот метод возвращает код ответа и обновленный импортируемый `200 OK` [объектAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="57d24-180">If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57d24-181">Пример</span><span class="sxs-lookup"><span data-stu-id="57d24-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="57d24-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d24-182">Request</span></span>
<span data-ttu-id="57d24-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57d24-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="57d24-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d24-184">Response</span></span>
<span data-ttu-id="57d24-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57d24-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
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
  "platform": "ios",
  "status": true
}
```




