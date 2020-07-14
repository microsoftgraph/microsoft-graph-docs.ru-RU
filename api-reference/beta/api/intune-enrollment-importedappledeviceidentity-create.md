---
title: Создание Импортедаппледевицеидентити
description: Создание нового объекта Импортедаппледевицеидентити.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67299d70e50052f104388a5aae046122c0d63299
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122688"
---
# <a name="create-importedappledeviceidentity"></a><span data-ttu-id="1da12-103">Создание Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="1da12-103">Create importedAppleDeviceIdentity</span></span>

<span data-ttu-id="1da12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1da12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1da12-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1da12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1da12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1da12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1da12-107">Создание нового объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="1da12-107">Create a new [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1da12-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1da12-108">Prerequisites</span></span>
<span data-ttu-id="1da12-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1da12-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1da12-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1da12-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1da12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1da12-111">Permission type</span></span>|<span data-ttu-id="1da12-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1da12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1da12-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1da12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1da12-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da12-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1da12-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1da12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1da12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1da12-116">Not supported.</span></span>|
|<span data-ttu-id="1da12-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1da12-117">Application</span></span>|<span data-ttu-id="1da12-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da12-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1da12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1da12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="1da12-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1da12-120">Request headers</span></span>
|<span data-ttu-id="1da12-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1da12-121">Header</span></span>|<span data-ttu-id="1da12-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1da12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1da12-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1da12-123">Authorization</span></span>|<span data-ttu-id="1da12-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1da12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1da12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1da12-125">Accept</span></span>|<span data-ttu-id="1da12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1da12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1da12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1da12-127">Request body</span></span>
<span data-ttu-id="1da12-128">В тексте запроса добавьте представление объекта Импортедаппледевицеидентити в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1da12-128">In the request body, supply a JSON representation for the importedAppleDeviceIdentity object.</span></span>

<span data-ttu-id="1da12-129">В следующей таблице приведены свойства, необходимые при создании Импортедаппледевицеидентити.</span><span class="sxs-lookup"><span data-stu-id="1da12-129">The following table shows the properties that are required when you create the importedAppleDeviceIdentity.</span></span>

|<span data-ttu-id="1da12-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1da12-130">Property</span></span>|<span data-ttu-id="1da12-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1da12-131">Type</span></span>|<span data-ttu-id="1da12-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1da12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1da12-133">id</span><span class="sxs-lookup"><span data-stu-id="1da12-133">id</span></span>|<span data-ttu-id="1da12-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1da12-134">String</span></span>|<span data-ttu-id="1da12-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1da12-135">Key of the entity.</span></span>|
|<span data-ttu-id="1da12-136">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1da12-136">serialNumber</span></span>|<span data-ttu-id="1da12-137">String</span><span class="sxs-lookup"><span data-stu-id="1da12-137">String</span></span>|<span data-ttu-id="1da12-138">Серийный номер устройства</span><span class="sxs-lookup"><span data-stu-id="1da12-138">Device serial number</span></span>|
|<span data-ttu-id="1da12-139">рекуестеденроллментпрофилеид</span><span class="sxs-lookup"><span data-stu-id="1da12-139">requestedEnrollmentProfileId</span></span>|<span data-ttu-id="1da12-140">String</span><span class="sxs-lookup"><span data-stu-id="1da12-140">String</span></span>|<span data-ttu-id="1da12-141">Идентификатор профиля регистрации администратор планирует применить к устройству во время следующей регистрации</span><span class="sxs-lookup"><span data-stu-id="1da12-141">Enrollment profile Id admin intends to apply to the device during next enrollment</span></span>|
|<span data-ttu-id="1da12-142">рекуестеденроллментпрофилеассигнментдатетиме</span><span class="sxs-lookup"><span data-stu-id="1da12-142">requestedEnrollmentProfileAssignmentDateTime</span></span>|<span data-ttu-id="1da12-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1da12-143">DateTimeOffset</span></span>|<span data-ttu-id="1da12-144">Для устройства назначен профиль регистрации времени.</span><span class="sxs-lookup"><span data-stu-id="1da12-144">The time enrollment profile was assigned to the device</span></span>|
|<span data-ttu-id="1da12-145">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1da12-145">isSupervised</span></span>|<span data-ttu-id="1da12-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1da12-146">Boolean</span></span>|<span data-ttu-id="1da12-147">Указывает, защищено ли устройство Apple.</span><span class="sxs-lookup"><span data-stu-id="1da12-147">Indicates if the Apple device is supervised.</span></span> <span data-ttu-id="1da12-148">Дополнительные сведения:https://support.apple.com/HT202837</span><span class="sxs-lookup"><span data-stu-id="1da12-148">More information is at: https://support.apple.com/HT202837</span></span>|
|<span data-ttu-id="1da12-149">discoverySource</span><span class="sxs-lookup"><span data-stu-id="1da12-149">discoverySource</span></span>|<span data-ttu-id="1da12-150">[discoverySource](../resources/intune-enrollment-discoverysource.md);</span><span class="sxs-lookup"><span data-stu-id="1da12-150">[discoverySource](../resources/intune-enrollment-discoverysource.md)</span></span>|<span data-ttu-id="1da12-151">Источник обнаружения устройств Apple.</span><span class="sxs-lookup"><span data-stu-id="1da12-151">Apple device discovery source.</span></span> <span data-ttu-id="1da12-152">Возможные значения: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span><span class="sxs-lookup"><span data-stu-id="1da12-152">Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.</span></span>|
|<span data-ttu-id="1da12-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1da12-153">isDeleted</span></span>|<span data-ttu-id="1da12-154">Логический</span><span class="sxs-lookup"><span data-stu-id="1da12-154">Boolean</span></span>|<span data-ttu-id="1da12-155">Указывает, было ли устройство удалено из Apple Business Manager</span><span class="sxs-lookup"><span data-stu-id="1da12-155">Indicates if the device is deleted from Apple Business Manager</span></span>|
|<span data-ttu-id="1da12-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1da12-156">createdDateTime</span></span>|<span data-ttu-id="1da12-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1da12-157">DateTimeOffset</span></span>|<span data-ttu-id="1da12-158">Дата и время создания устройства</span><span class="sxs-lookup"><span data-stu-id="1da12-158">Created Date Time of the device</span></span>|
|<span data-ttu-id="1da12-159">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="1da12-159">lastContactedDateTime</span></span>|<span data-ttu-id="1da12-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1da12-160">DateTimeOffset</span></span>|<span data-ttu-id="1da12-161">Дата и время последнего обращения к устройству</span><span class="sxs-lookup"><span data-stu-id="1da12-161">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="1da12-162">description</span><span class="sxs-lookup"><span data-stu-id="1da12-162">description</span></span>|<span data-ttu-id="1da12-163">String</span><span class="sxs-lookup"><span data-stu-id="1da12-163">String</span></span>|<span data-ttu-id="1da12-164">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="1da12-164">The description of the device</span></span>|
|<span data-ttu-id="1da12-165">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="1da12-165">enrollmentState</span></span>|[<span data-ttu-id="1da12-166">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="1da12-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="1da12-167">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="1da12-167">The state of the device in Intune.</span></span> <span data-ttu-id="1da12-168">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="1da12-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1da12-169">platform</span><span class="sxs-lookup"><span data-stu-id="1da12-169">platform</span></span>|[<span data-ttu-id="1da12-170">управляем</span><span class="sxs-lookup"><span data-stu-id="1da12-170">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="1da12-171">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="1da12-171">The platform of the Device.</span></span> <span data-ttu-id="1da12-172">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="1da12-172">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="1da12-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="1da12-173">Response</span></span>
<span data-ttu-id="1da12-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1da12-174">If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1da12-175">Пример</span><span class="sxs-lookup"><span data-stu-id="1da12-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="1da12-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="1da12-176">Request</span></span>
<span data-ttu-id="1da12-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1da12-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="1da12-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="1da12-178">Response</span></span>
<span data-ttu-id="1da12-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1da12-179">Here is an example of the response.</span></span> <span data-ttu-id="1da12-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1da12-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1da12-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1da12-181">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



