---
title: Создание windowsInformationProtectionDeviceRegistration
description: Создание нового объекта windowsInformationProtectionDeviceRegistration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a752cb3262d4ca8899660e0de50b637315680ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158887"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="b765b-103">Создание windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="b765b-103">Create windowsInformationProtectionDeviceRegistration</span></span>

<span data-ttu-id="b765b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b765b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b765b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b765b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b765b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b765b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b765b-107">Создание нового [объекта windowsInformationProtectionDeviceRegistration.](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)</span><span class="sxs-lookup"><span data-stu-id="b765b-107">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b765b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b765b-108">Prerequisites</span></span>
<span data-ttu-id="b765b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b765b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b765b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b765b-111">Permission type</span></span>|<span data-ttu-id="b765b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b765b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b765b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b765b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b765b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b765b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b765b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b765b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b765b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b765b-116">Not supported.</span></span>|
|<span data-ttu-id="b765b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b765b-117">Application</span></span>|<span data-ttu-id="b765b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b765b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b765b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b765b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="b765b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b765b-120">Request headers</span></span>
|<span data-ttu-id="b765b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b765b-121">Header</span></span>|<span data-ttu-id="b765b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b765b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b765b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b765b-123">Authorization</span></span>|<span data-ttu-id="b765b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b765b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b765b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b765b-125">Accept</span></span>|<span data-ttu-id="b765b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b765b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b765b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b765b-127">Request body</span></span>
<span data-ttu-id="b765b-128">В теле запроса поставляем представление JSON для объекта windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="b765b-128">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="b765b-129">В следующей таблице показаны свойства, необходимые при создании windowsInformationProtectionDeviceRegistration.</span><span class="sxs-lookup"><span data-stu-id="b765b-129">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="b765b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b765b-130">Property</span></span>|<span data-ttu-id="b765b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b765b-131">Type</span></span>|<span data-ttu-id="b765b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b765b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b765b-133">id</span><span class="sxs-lookup"><span data-stu-id="b765b-133">id</span></span>|<span data-ttu-id="b765b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b765b-134">String</span></span>|<span data-ttu-id="b765b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b765b-135">Key of the entity.</span></span>|
|<span data-ttu-id="b765b-136">userId</span><span class="sxs-lookup"><span data-stu-id="b765b-136">userId</span></span>|<span data-ttu-id="b765b-137">String</span><span class="sxs-lookup"><span data-stu-id="b765b-137">String</span></span>|<span data-ttu-id="b765b-138">UserId, связанный с этой записью регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b765b-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="b765b-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="b765b-139">deviceRegistrationId</span></span>|<span data-ttu-id="b765b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b765b-140">String</span></span>|<span data-ttu-id="b765b-141">Идентификатор устройства для записи регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="b765b-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="b765b-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="b765b-142">deviceName</span></span>|<span data-ttu-id="b765b-143">String</span><span class="sxs-lookup"><span data-stu-id="b765b-143">String</span></span>|<span data-ttu-id="b765b-144">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="b765b-144">Device name.</span></span>|
|<span data-ttu-id="b765b-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="b765b-145">deviceType</span></span>|<span data-ttu-id="b765b-146">String</span><span class="sxs-lookup"><span data-stu-id="b765b-146">String</span></span>|<span data-ttu-id="b765b-147">Тип устройства, например, windows laptop VS Windows phone.</span><span class="sxs-lookup"><span data-stu-id="b765b-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="b765b-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="b765b-148">deviceMacAddress</span></span>|<span data-ttu-id="b765b-149">Строка</span><span class="sxs-lookup"><span data-stu-id="b765b-149">String</span></span>|<span data-ttu-id="b765b-150">Адрес Mac устройства.</span><span class="sxs-lookup"><span data-stu-id="b765b-150">Device Mac address.</span></span>|
|<span data-ttu-id="b765b-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="b765b-151">lastCheckInDateTime</span></span>|<span data-ttu-id="b765b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b765b-152">DateTimeOffset</span></span>|<span data-ttu-id="b765b-153">Время последней проверки устройства.</span><span class="sxs-lookup"><span data-stu-id="b765b-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="b765b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b765b-154">Response</span></span>
<span data-ttu-id="b765b-155">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b765b-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b765b-156">Пример</span><span class="sxs-lookup"><span data-stu-id="b765b-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="b765b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b765b-157">Request</span></span>
<span data-ttu-id="b765b-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b765b-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
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

### <a name="response"></a><span data-ttu-id="b765b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b765b-159">Response</span></span>
<span data-ttu-id="b765b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b765b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




