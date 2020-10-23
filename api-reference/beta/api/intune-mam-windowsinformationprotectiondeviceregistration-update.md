---
title: Обновление Виндовсинформатионпротектиондевицерегистратион
description: Обновление свойств объекта Виндовсинформатионпротектиондевицерегистратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e73c9664b0946e2c02d8f60ec95ae9832a7e3b3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694363"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="fc8e3-103">Обновление Виндовсинформатионпротектиондевицерегистратион</span><span class="sxs-lookup"><span data-stu-id="fc8e3-103">Update windowsInformationProtectionDeviceRegistration</span></span>

<span data-ttu-id="fc8e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc8e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc8e3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc8e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc8e3-107">Обновление свойств объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="fc8e3-107">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc8e3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc8e3-108">Prerequisites</span></span>
<span data-ttu-id="fc8e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc8e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc8e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc8e3-111">Permission type</span></span>|<span data-ttu-id="fc8e3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc8e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc8e3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc8e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc8e3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc8e3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc8e3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc8e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc8e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-116">Not supported.</span></span>|
|<span data-ttu-id="fc8e3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc8e3-117">Application</span></span>|<span data-ttu-id="fc8e3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc8e3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc8e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc8e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="fc8e3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fc8e3-120">Request headers</span></span>
|<span data-ttu-id="fc8e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc8e3-121">Header</span></span>|<span data-ttu-id="fc8e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc8e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc8e3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc8e3-123">Authorization</span></span>|<span data-ttu-id="fc8e3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc8e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc8e3-125">Accept</span></span>|<span data-ttu-id="fc8e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc8e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc8e3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc8e3-127">Request body</span></span>
<span data-ttu-id="fc8e3-128">В тексте запроса добавьте представление объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-128">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="fc8e3-129">В следующей таблице приведены свойства, необходимые при создании [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span><span class="sxs-lookup"><span data-stu-id="fc8e3-129">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="fc8e3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc8e3-130">Property</span></span>|<span data-ttu-id="fc8e3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fc8e3-131">Type</span></span>|<span data-ttu-id="fc8e3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fc8e3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc8e3-133">id</span><span class="sxs-lookup"><span data-stu-id="fc8e3-133">id</span></span>|<span data-ttu-id="fc8e3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fc8e3-134">String</span></span>|<span data-ttu-id="fc8e3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-135">Key of the entity.</span></span>|
|<span data-ttu-id="fc8e3-136">userId</span><span class="sxs-lookup"><span data-stu-id="fc8e3-136">userId</span></span>|<span data-ttu-id="fc8e3-137">String</span><span class="sxs-lookup"><span data-stu-id="fc8e3-137">String</span></span>|<span data-ttu-id="fc8e3-138">UserId, связанный с этой записью регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="fc8e3-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="fc8e3-139">deviceRegistrationId</span></span>|<span data-ttu-id="fc8e3-140">Строка</span><span class="sxs-lookup"><span data-stu-id="fc8e3-140">String</span></span>|<span data-ttu-id="fc8e3-141">Идентификатор устройства для записи регистрации этого устройства.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="fc8e3-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="fc8e3-142">deviceName</span></span>|<span data-ttu-id="fc8e3-143">String</span><span class="sxs-lookup"><span data-stu-id="fc8e3-143">String</span></span>|<span data-ttu-id="fc8e3-144">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-144">Device name.</span></span>|
|<span data-ttu-id="fc8e3-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="fc8e3-145">deviceType</span></span>|<span data-ttu-id="fc8e3-146">String</span><span class="sxs-lookup"><span data-stu-id="fc8e3-146">String</span></span>|<span data-ttu-id="fc8e3-147">Тип устройства, например Windows для портативного компьютера Windows и Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="fc8e3-148">девицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="fc8e3-148">deviceMacAddress</span></span>|<span data-ttu-id="fc8e3-149">Строка</span><span class="sxs-lookup"><span data-stu-id="fc8e3-149">String</span></span>|<span data-ttu-id="fc8e3-150">Mac-адрес устройства.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-150">Device Mac address.</span></span>|
|<span data-ttu-id="fc8e3-151">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="fc8e3-151">lastCheckInDateTime</span></span>|<span data-ttu-id="fc8e3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc8e3-152">DateTimeOffset</span></span>|<span data-ttu-id="fc8e3-153">Время последнего возврата устройства.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="fc8e3-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc8e3-154">Response</span></span>
<span data-ttu-id="fc8e3-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc8e3-156">Пример</span><span class="sxs-lookup"><span data-stu-id="fc8e3-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc8e3-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc8e3-157">Request</span></span>
<span data-ttu-id="fc8e3-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc8e3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc8e3-159">Response</span></span>
<span data-ttu-id="fc8e3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc8e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





