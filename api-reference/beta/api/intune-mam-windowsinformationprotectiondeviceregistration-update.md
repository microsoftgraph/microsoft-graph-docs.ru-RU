---
title: Обновление windowsInformationProtectionDeviceRegistration
description: Обновление свойства объекта windowsInformationProtectionDeviceRegistration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c84f81dd8d9df54c6f05b1435ee4644a1a75342
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430720"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="040ed-103">Обновление windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="040ed-103">Update windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="040ed-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="040ed-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="040ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="040ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="040ed-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="040ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="040ed-107">Обновление свойства объекта [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="040ed-107">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="040ed-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="040ed-108">Prerequisites</span></span>
<span data-ttu-id="040ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="040ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="040ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="040ed-111">Permission type</span></span>|<span data-ttu-id="040ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="040ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="040ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="040ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="040ed-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="040ed-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="040ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="040ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="040ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="040ed-116">Not supported.</span></span>|
|<span data-ttu-id="040ed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="040ed-117">Application</span></span>|<span data-ttu-id="040ed-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="040ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="040ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="040ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="040ed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="040ed-120">Request headers</span></span>
|<span data-ttu-id="040ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="040ed-121">Header</span></span>|<span data-ttu-id="040ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="040ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="040ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="040ed-123">Authorization</span></span>|<span data-ttu-id="040ed-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="040ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="040ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="040ed-125">Accept</span></span>|<span data-ttu-id="040ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="040ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="040ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="040ed-127">Request body</span></span>
<span data-ttu-id="040ed-128">В тексте запроса укажите представление JSON для объекта [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="040ed-128">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="040ed-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span><span class="sxs-lookup"><span data-stu-id="040ed-129">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="040ed-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="040ed-130">Property</span></span>|<span data-ttu-id="040ed-131">Тип</span><span class="sxs-lookup"><span data-stu-id="040ed-131">Type</span></span>|<span data-ttu-id="040ed-132">Описание</span><span class="sxs-lookup"><span data-stu-id="040ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="040ed-133">id</span><span class="sxs-lookup"><span data-stu-id="040ed-133">id</span></span>|<span data-ttu-id="040ed-134">String</span><span class="sxs-lookup"><span data-stu-id="040ed-134">String</span></span>|<span data-ttu-id="040ed-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="040ed-135">Key of the entity.</span></span>|
|<span data-ttu-id="040ed-136">userId</span><span class="sxs-lookup"><span data-stu-id="040ed-136">userId</span></span>|<span data-ttu-id="040ed-137">String</span><span class="sxs-lookup"><span data-stu-id="040ed-137">String</span></span>|<span data-ttu-id="040ed-138">Идентификатор пользователя, связанного с этой записи регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="040ed-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="040ed-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="040ed-139">deviceRegistrationId</span></span>|<span data-ttu-id="040ed-140">Строка</span><span class="sxs-lookup"><span data-stu-id="040ed-140">String</span></span>|<span data-ttu-id="040ed-141">Идентификатор устройства для этой записи регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="040ed-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="040ed-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="040ed-142">deviceName</span></span>|<span data-ttu-id="040ed-143">String</span><span class="sxs-lookup"><span data-stu-id="040ed-143">String</span></span>|<span data-ttu-id="040ed-144">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="040ed-144">Device name.</span></span>|
|<span data-ttu-id="040ed-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="040ed-145">deviceType</span></span>|<span data-ttu-id="040ed-146">String</span><span class="sxs-lookup"><span data-stu-id="040ed-146">String</span></span>|<span data-ttu-id="040ed-147">Тип устройства, например, Windows ноутбуков — и Windows phone.</span><span class="sxs-lookup"><span data-stu-id="040ed-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="040ed-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="040ed-148">deviceMacAddress</span></span>|<span data-ttu-id="040ed-149">String</span><span class="sxs-lookup"><span data-stu-id="040ed-149">String</span></span>|<span data-ttu-id="040ed-150">Mac-адрес устройства.</span><span class="sxs-lookup"><span data-stu-id="040ed-150">Device Mac address.</span></span>|
|<span data-ttu-id="040ed-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="040ed-151">lastCheckInDateTime</span></span>|<span data-ttu-id="040ed-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="040ed-152">DateTimeOffset</span></span>|<span data-ttu-id="040ed-153">Время последнего checkin устройства.</span><span class="sxs-lookup"><span data-stu-id="040ed-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="040ed-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="040ed-154">Response</span></span>
<span data-ttu-id="040ed-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="040ed-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="040ed-156">Пример</span><span class="sxs-lookup"><span data-stu-id="040ed-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="040ed-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="040ed-157">Request</span></span>
<span data-ttu-id="040ed-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="040ed-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="040ed-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="040ed-159">Response</span></span>
<span data-ttu-id="040ed-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="040ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




