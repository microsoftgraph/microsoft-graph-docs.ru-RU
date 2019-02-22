---
title: Создание Импортедаппледевицеидентити
description: Создание нового объекта Импортедаппледевицеидентити.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7eb92900e7dfaad30cf23b1d89d3851fe4d1be4e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151620"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="479fb-103">Создание Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="479fb-103">Create importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="479fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="479fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="479fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="479fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="479fb-106">Создание нового объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="479fb-106">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="479fb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="479fb-107">Prerequisites</span></span>
<span data-ttu-id="479fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="479fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="479fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="479fb-110">Permission type</span></span>|<span data-ttu-id="479fb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="479fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="479fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="479fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="479fb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479fb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="479fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="479fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="479fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="479fb-115">Not supported.</span></span>|
|<span data-ttu-id="479fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="479fb-116">Application</span></span>|<span data-ttu-id="479fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="479fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="479fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="479fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="479fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="479fb-119">Request headers</span></span>
|<span data-ttu-id="479fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="479fb-120">Header</span></span>|<span data-ttu-id="479fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="479fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="479fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="479fb-122">Authorization</span></span>|<span data-ttu-id="479fb-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="479fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="479fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="479fb-124">Accept</span></span>|<span data-ttu-id="479fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="479fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="479fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="479fb-126">Request body</span></span>
<span data-ttu-id="479fb-127">В тексте запроса добавьте представление объекта Импортедаппледевицеидентити в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="479fb-127">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="479fb-128">В следующей таблице приведены свойства, необходимые при создании Импортедаппледевицеидентити.</span><span class="sxs-lookup"><span data-stu-id="479fb-128">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="479fb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="479fb-129">Property</span></span>|<span data-ttu-id="479fb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="479fb-130">Type</span></span>|<span data-ttu-id="479fb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="479fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="479fb-132">id</span><span class="sxs-lookup"><span data-stu-id="479fb-132">id</span></span>|<span data-ttu-id="479fb-133">String</span><span class="sxs-lookup"><span data-stu-id="479fb-133">String</span></span>|<span data-ttu-id="479fb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="479fb-134">Key of the entity.</span></span>|
|<span data-ttu-id="479fb-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="479fb-135">serialNumber</span></span>|<span data-ttu-id="479fb-136">String</span><span class="sxs-lookup"><span data-stu-id="479fb-136">String</span></span>|<span data-ttu-id="479fb-137">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="479fb-137">Device serial number</span></span>|
|<span data-ttu-id="479fb-138">Рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="479fb-138">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="479fb-139">String</span><span class="sxs-lookup"><span data-stu-id="479fb-139">String</span></span>|<span data-ttu-id="479fb-140">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="479fb-140">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="479fb-141">Рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="479fb-141">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="479fb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="479fb-142">DateTimeOffset</span></span>|<span data-ttu-id="479fb-143">Для устройства назначен профиль регистрации времени.</span><span class="sxs-lookup"><span data-stu-id="479fb-143">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="479fb-144">isSupervised</span><span class="sxs-lookup"><span data-stu-id="479fb-144">isSupervised</span></span>|<span data-ttu-id="479fb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="479fb-145">Boolean</span></span>|<span data-ttu-id="479fb-146">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="479fb-146">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="479fb-147">Дополнительные сведения:https://support.apple.com/en-us/HT202837</span><span class="sxs-lookup"><span data-stu-id="479fb-147">More information is at: https://support.apple.com/en-us/HT202837</span></span>|
|<span data-ttu-id="479fb-148">discoverySource;</span><span class="sxs-lookup"><span data-stu-id="479fb-148">discoverySource</span></span>|<span data-ttu-id="479fb-149">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="479fb-149">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="479fb-150">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="479fb-150">Apple device discovery source.</span></span> <span data-ttu-id="479fb-151">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="479fb-151">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="479fb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="479fb-152">createdDateTime</span></span>|<span data-ttu-id="479fb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="479fb-153">DateTimeOffset</span></span>|<span data-ttu-id="479fb-154">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="479fb-154">Created Date Time of the device</span></span>|
|<span data-ttu-id="479fb-155">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="479fb-155">lastContactedDateTime</span></span>|<span data-ttu-id="479fb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="479fb-156">DateTimeOffset</span></span>|<span data-ttu-id="479fb-157">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="479fb-157">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="479fb-158">description</span><span class="sxs-lookup"><span data-stu-id="479fb-158">description</span></span>|<span data-ttu-id="479fb-159">Строка</span><span class="sxs-lookup"><span data-stu-id="479fb-159">String</span></span>|<span data-ttu-id="479fb-160">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="479fb-160">The description of the device</span></span>|
|<span data-ttu-id="479fb-161">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="479fb-161">enrollmentState</span></span>|[<span data-ttu-id="479fb-162">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="479fb-162">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="479fb-163">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="479fb-163">The state of the device in Intune.</span></span> <span data-ttu-id="479fb-164">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="479fb-164">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="479fb-165">platform</span><span class="sxs-lookup"><span data-stu-id="479fb-165">platform</span></span>|[<span data-ttu-id="479fb-166">управляем</span><span class="sxs-lookup"><span data-stu-id="479fb-166">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="479fb-167">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="479fb-167">The platform of the Device.</span></span> <span data-ttu-id="479fb-168">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="479fb-168">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="479fb-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="479fb-169">Response</span></span>
<span data-ttu-id="479fb-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="479fb-170">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="479fb-171">Пример</span><span class="sxs-lookup"><span data-stu-id="479fb-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="479fb-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="479fb-172">Request</span></span>
<span data-ttu-id="479fb-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="479fb-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="479fb-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="479fb-174">Response</span></span>
<span data-ttu-id="479fb-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="479fb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




