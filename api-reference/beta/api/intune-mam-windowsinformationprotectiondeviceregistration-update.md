---
title: Обновление Виндовсинформатионпротектиондевицерегистратион
description: Обновление свойств объекта Виндовсинформатионпротектиондевицерегистратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54d8dc2e1c2c62d956502e48791ad55e0787de03
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786079"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="42a78-103">Обновление Виндовсинформатионпротектиондевицерегистратион</span><span class="sxs-lookup"><span data-stu-id="42a78-103">Update windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="42a78-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42a78-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42a78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42a78-106">Обновление свойств объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="42a78-106">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42a78-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42a78-107">Prerequisites</span></span>
<span data-ttu-id="42a78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42a78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42a78-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42a78-110">Permission type</span></span>|<span data-ttu-id="42a78-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42a78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42a78-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42a78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42a78-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a78-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42a78-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42a78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42a78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a78-115">Not supported.</span></span>|
|<span data-ttu-id="42a78-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42a78-116">Application</span></span>|<span data-ttu-id="42a78-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42a78-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42a78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="42a78-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42a78-119">Request headers</span></span>
|<span data-ttu-id="42a78-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42a78-120">Header</span></span>|<span data-ttu-id="42a78-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42a78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42a78-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42a78-122">Authorization</span></span>|<span data-ttu-id="42a78-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42a78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42a78-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42a78-124">Accept</span></span>|<span data-ttu-id="42a78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42a78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42a78-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42a78-126">Request body</span></span>
<span data-ttu-id="42a78-127">В тексте запроса добавьте представление объекта [Виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42a78-127">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="42a78-128">В следующей таблице приведены свойства, необходимые при создании [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span><span class="sxs-lookup"><span data-stu-id="42a78-128">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="42a78-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="42a78-129">Property</span></span>|<span data-ttu-id="42a78-130">Тип</span><span class="sxs-lookup"><span data-stu-id="42a78-130">Type</span></span>|<span data-ttu-id="42a78-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42a78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42a78-132">id</span><span class="sxs-lookup"><span data-stu-id="42a78-132">id</span></span>|<span data-ttu-id="42a78-133">String</span><span class="sxs-lookup"><span data-stu-id="42a78-133">String</span></span>|<span data-ttu-id="42a78-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42a78-134">Key of the entity.</span></span>|
|<span data-ttu-id="42a78-135">userId</span><span class="sxs-lookup"><span data-stu-id="42a78-135">userId</span></span>|<span data-ttu-id="42a78-136">String</span><span class="sxs-lookup"><span data-stu-id="42a78-136">String</span></span>|<span data-ttu-id="42a78-137">UserId, связанный с этой записью регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="42a78-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="42a78-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="42a78-138">deviceRegistrationId</span></span>|<span data-ttu-id="42a78-139">Строка</span><span class="sxs-lookup"><span data-stu-id="42a78-139">String</span></span>|<span data-ttu-id="42a78-140">Идентификатор устройства для записи регистрации этого устройства.</span><span class="sxs-lookup"><span data-stu-id="42a78-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="42a78-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="42a78-141">deviceName</span></span>|<span data-ttu-id="42a78-142">String</span><span class="sxs-lookup"><span data-stu-id="42a78-142">String</span></span>|<span data-ttu-id="42a78-143">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="42a78-143">Device name.</span></span>|
|<span data-ttu-id="42a78-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="42a78-144">deviceType</span></span>|<span data-ttu-id="42a78-145">String</span><span class="sxs-lookup"><span data-stu-id="42a78-145">String</span></span>|<span data-ttu-id="42a78-146">Тип устройства, например Windows для портативного компьютера Windows и Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="42a78-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="42a78-147">Девицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="42a78-147">deviceMacAddress</span></span>|<span data-ttu-id="42a78-148">String</span><span class="sxs-lookup"><span data-stu-id="42a78-148">String</span></span>|<span data-ttu-id="42a78-149">Mac-адрес устройства.</span><span class="sxs-lookup"><span data-stu-id="42a78-149">Device Mac address.</span></span>|
|<span data-ttu-id="42a78-150">Ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="42a78-150">lastCheckInDateTime</span></span>|<span data-ttu-id="42a78-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42a78-151">DateTimeOffset</span></span>|<span data-ttu-id="42a78-152">Время последнего возврата устройства.</span><span class="sxs-lookup"><span data-stu-id="42a78-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="42a78-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a78-153">Response</span></span>
<span data-ttu-id="42a78-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42a78-154">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42a78-155">Пример</span><span class="sxs-lookup"><span data-stu-id="42a78-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="42a78-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="42a78-156">Request</span></span>
<span data-ttu-id="42a78-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42a78-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42a78-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a78-158">Response</span></span>
<span data-ttu-id="42a78-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42a78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





