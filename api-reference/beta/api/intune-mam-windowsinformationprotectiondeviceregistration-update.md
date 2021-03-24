---
title: Обновление windowsInformationProtectionDeviceRegistration
description: Обновление свойств объекта windowsInformationProtectionDeviceRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0652b9dbd0d81d8d4f02a418d36ff0555809c20e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135231"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="7ebbc-103">Обновление windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="7ebbc-103">Update windowsInformationProtectionDeviceRegistration</span></span>

<span data-ttu-id="7ebbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ebbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ebbc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ebbc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ebbc-107">Обновление свойств объекта [windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)</span><span class="sxs-lookup"><span data-stu-id="7ebbc-107">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ebbc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7ebbc-108">Prerequisites</span></span>
<span data-ttu-id="7ebbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ebbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ebbc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ebbc-111">Permission type</span></span>|<span data-ttu-id="7ebbc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ebbc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ebbc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ebbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ebbc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ebbc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ebbc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ebbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ebbc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-116">Not supported.</span></span>|
|<span data-ttu-id="7ebbc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7ebbc-117">Application</span></span>|<span data-ttu-id="7ebbc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ebbc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ebbc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ebbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="7ebbc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ebbc-120">Request headers</span></span>
|<span data-ttu-id="7ebbc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ebbc-121">Header</span></span>|<span data-ttu-id="7ebbc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7ebbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ebbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ebbc-123">Authorization</span></span>|<span data-ttu-id="7ebbc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ebbc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ebbc-125">Accept</span></span>|<span data-ttu-id="7ebbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ebbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ebbc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ebbc-127">Request body</span></span>
<span data-ttu-id="7ebbc-128">В теле запроса поставляем представление JSON для [объекта windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)</span><span class="sxs-lookup"><span data-stu-id="7ebbc-128">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="7ebbc-129">В следующей таблице показаны свойства, необходимые при создании [windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)</span><span class="sxs-lookup"><span data-stu-id="7ebbc-129">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="7ebbc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ebbc-130">Property</span></span>|<span data-ttu-id="7ebbc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ebbc-131">Type</span></span>|<span data-ttu-id="7ebbc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ebbc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ebbc-133">id</span><span class="sxs-lookup"><span data-stu-id="7ebbc-133">id</span></span>|<span data-ttu-id="7ebbc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7ebbc-134">String</span></span>|<span data-ttu-id="7ebbc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-135">Key of the entity.</span></span>|
|<span data-ttu-id="7ebbc-136">userId</span><span class="sxs-lookup"><span data-stu-id="7ebbc-136">userId</span></span>|<span data-ttu-id="7ebbc-137">String</span><span class="sxs-lookup"><span data-stu-id="7ebbc-137">String</span></span>|<span data-ttu-id="7ebbc-138">UserId, связанный с этой записью регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="7ebbc-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="7ebbc-139">deviceRegistrationId</span></span>|<span data-ttu-id="7ebbc-140">Строка</span><span class="sxs-lookup"><span data-stu-id="7ebbc-140">String</span></span>|<span data-ttu-id="7ebbc-141">Идентификатор устройства для записи регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="7ebbc-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="7ebbc-142">deviceName</span></span>|<span data-ttu-id="7ebbc-143">String</span><span class="sxs-lookup"><span data-stu-id="7ebbc-143">String</span></span>|<span data-ttu-id="7ebbc-144">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-144">Device name.</span></span>|
|<span data-ttu-id="7ebbc-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="7ebbc-145">deviceType</span></span>|<span data-ttu-id="7ebbc-146">String</span><span class="sxs-lookup"><span data-stu-id="7ebbc-146">String</span></span>|<span data-ttu-id="7ebbc-147">Тип устройства, например, windows laptop VS Windows phone.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="7ebbc-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="7ebbc-148">deviceMacAddress</span></span>|<span data-ttu-id="7ebbc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="7ebbc-149">String</span></span>|<span data-ttu-id="7ebbc-150">Адрес Mac устройства.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-150">Device Mac address.</span></span>|
|<span data-ttu-id="7ebbc-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="7ebbc-151">lastCheckInDateTime</span></span>|<span data-ttu-id="7ebbc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ebbc-152">DateTimeOffset</span></span>|<span data-ttu-id="7ebbc-153">Время последней проверки устройства.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="7ebbc-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ebbc-154">Response</span></span>
<span data-ttu-id="7ebbc-155">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ebbc-156">Пример</span><span class="sxs-lookup"><span data-stu-id="7ebbc-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ebbc-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ebbc-157">Request</span></span>
<span data-ttu-id="7ebbc-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
Content-type: application/json
Content-length: 366

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="7ebbc-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ebbc-159">Response</span></span>
<span data-ttu-id="7ebbc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ebbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 415

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




