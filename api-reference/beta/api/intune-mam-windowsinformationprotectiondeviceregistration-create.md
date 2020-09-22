---
title: Создание Виндовсинформатионпротектиондевицерегистратион
description: Создание нового объекта Виндовсинформатионпротектиондевицерегистратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63f9d63b9e84d4f67100df7cff35d791e729c151
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078684"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="f93a7-103">Создание Виндовсинформатионпротектиондевицерегистратион</span><span class="sxs-lookup"><span data-stu-id="f93a7-103">Create windowsInformationProtectionDeviceRegistration</span></span>

<span data-ttu-id="f93a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f93a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f93a7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f93a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f93a7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f93a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f93a7-107">Создание нового объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="f93a7-107">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f93a7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f93a7-108">Prerequisites</span></span>
<span data-ttu-id="f93a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f93a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f93a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f93a7-111">Permission type</span></span>|<span data-ttu-id="f93a7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f93a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f93a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f93a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f93a7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f93a7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f93a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f93a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f93a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f93a7-116">Not supported.</span></span>|
|<span data-ttu-id="f93a7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f93a7-117">Application</span></span>|<span data-ttu-id="f93a7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f93a7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f93a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f93a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="f93a7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f93a7-120">Request headers</span></span>
|<span data-ttu-id="f93a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f93a7-121">Header</span></span>|<span data-ttu-id="f93a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f93a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f93a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f93a7-123">Authorization</span></span>|<span data-ttu-id="f93a7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f93a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f93a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f93a7-125">Accept</span></span>|<span data-ttu-id="f93a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f93a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f93a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f93a7-127">Request body</span></span>
<span data-ttu-id="f93a7-128">В тексте запроса добавьте представление объекта Виндовсинформатионпротектиондевицерегистратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f93a7-128">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="f93a7-129">В следующей таблице приведены свойства, необходимые при создании Виндовсинформатионпротектиондевицерегистратион.</span><span class="sxs-lookup"><span data-stu-id="f93a7-129">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="f93a7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f93a7-130">Property</span></span>|<span data-ttu-id="f93a7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f93a7-131">Type</span></span>|<span data-ttu-id="f93a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f93a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f93a7-133">id</span><span class="sxs-lookup"><span data-stu-id="f93a7-133">id</span></span>|<span data-ttu-id="f93a7-134">String</span><span class="sxs-lookup"><span data-stu-id="f93a7-134">String</span></span>|<span data-ttu-id="f93a7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f93a7-135">Key of the entity.</span></span>|
|<span data-ttu-id="f93a7-136">userId</span><span class="sxs-lookup"><span data-stu-id="f93a7-136">userId</span></span>|<span data-ttu-id="f93a7-137">String</span><span class="sxs-lookup"><span data-stu-id="f93a7-137">String</span></span>|<span data-ttu-id="f93a7-138">UserId, связанный с этой записью регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="f93a7-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="f93a7-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f93a7-139">deviceRegistrationId</span></span>|<span data-ttu-id="f93a7-140">Строка</span><span class="sxs-lookup"><span data-stu-id="f93a7-140">String</span></span>|<span data-ttu-id="f93a7-141">Идентификатор устройства для записи регистрации этого устройства.</span><span class="sxs-lookup"><span data-stu-id="f93a7-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="f93a7-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="f93a7-142">deviceName</span></span>|<span data-ttu-id="f93a7-143">String</span><span class="sxs-lookup"><span data-stu-id="f93a7-143">String</span></span>|<span data-ttu-id="f93a7-144">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="f93a7-144">Device name.</span></span>|
|<span data-ttu-id="f93a7-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="f93a7-145">deviceType</span></span>|<span data-ttu-id="f93a7-146">String</span><span class="sxs-lookup"><span data-stu-id="f93a7-146">String</span></span>|<span data-ttu-id="f93a7-147">Тип устройства, например Windows для портативного компьютера Windows и Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f93a7-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="f93a7-148">девицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="f93a7-148">deviceMacAddress</span></span>|<span data-ttu-id="f93a7-149">String</span><span class="sxs-lookup"><span data-stu-id="f93a7-149">String</span></span>|<span data-ttu-id="f93a7-150">Mac-адрес устройства.</span><span class="sxs-lookup"><span data-stu-id="f93a7-150">Device Mac address.</span></span>|
|<span data-ttu-id="f93a7-151">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="f93a7-151">lastCheckInDateTime</span></span>|<span data-ttu-id="f93a7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f93a7-152">DateTimeOffset</span></span>|<span data-ttu-id="f93a7-153">Время последнего возврата устройства.</span><span class="sxs-lookup"><span data-stu-id="f93a7-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="f93a7-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f93a7-154">Response</span></span>
<span data-ttu-id="f93a7-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f93a7-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f93a7-156">Пример</span><span class="sxs-lookup"><span data-stu-id="f93a7-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f93a7-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="f93a7-157">Request</span></span>
<span data-ttu-id="f93a7-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f93a7-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f93a7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="f93a7-159">Response</span></span>
<span data-ttu-id="f93a7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f93a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






