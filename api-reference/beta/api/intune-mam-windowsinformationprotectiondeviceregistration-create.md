---
title: Создание Виндовсинформатионпротектиондевицерегистратион
description: Создание нового объекта Виндовсинформатионпротектиондевицерегистратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 089e9546665ced37ff75e95353bbee18342dbc60
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191500"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="55880-103">Создание Виндовсинформатионпротектиондевицерегистратион</span><span class="sxs-lookup"><span data-stu-id="55880-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="55880-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55880-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55880-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55880-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55880-106">Создание нового объекта [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="55880-106">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55880-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55880-107">Prerequisites</span></span>
<span data-ttu-id="55880-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55880-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55880-110">Permission type</span></span>|<span data-ttu-id="55880-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55880-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55880-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55880-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55880-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55880-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55880-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55880-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55880-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55880-115">Not supported.</span></span>|
|<span data-ttu-id="55880-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55880-116">Application</span></span>|<span data-ttu-id="55880-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55880-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55880-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55880-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="55880-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55880-119">Request headers</span></span>
|<span data-ttu-id="55880-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55880-120">Header</span></span>|<span data-ttu-id="55880-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55880-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55880-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55880-122">Authorization</span></span>|<span data-ttu-id="55880-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55880-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55880-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55880-124">Accept</span></span>|<span data-ttu-id="55880-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55880-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55880-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55880-126">Request body</span></span>
<span data-ttu-id="55880-127">В тексте запроса добавьте представление объекта Виндовсинформатионпротектиондевицерегистратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55880-127">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="55880-128">В следующей таблице приведены свойства, необходимые при создании Виндовсинформатионпротектиондевицерегистратион.</span><span class="sxs-lookup"><span data-stu-id="55880-128">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="55880-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="55880-129">Property</span></span>|<span data-ttu-id="55880-130">Тип</span><span class="sxs-lookup"><span data-stu-id="55880-130">Type</span></span>|<span data-ttu-id="55880-131">Описание</span><span class="sxs-lookup"><span data-stu-id="55880-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55880-132">id</span><span class="sxs-lookup"><span data-stu-id="55880-132">id</span></span>|<span data-ttu-id="55880-133">Строка</span><span class="sxs-lookup"><span data-stu-id="55880-133">String</span></span>|<span data-ttu-id="55880-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55880-134">Key of the entity.</span></span>|
|<span data-ttu-id="55880-135">userId</span><span class="sxs-lookup"><span data-stu-id="55880-135">userId</span></span>|<span data-ttu-id="55880-136">String</span><span class="sxs-lookup"><span data-stu-id="55880-136">String</span></span>|<span data-ttu-id="55880-137">UserId, связанный с этой записью регистрации устройства.</span><span class="sxs-lookup"><span data-stu-id="55880-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="55880-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="55880-138">deviceRegistrationId</span></span>|<span data-ttu-id="55880-139">Строка</span><span class="sxs-lookup"><span data-stu-id="55880-139">String</span></span>|<span data-ttu-id="55880-140">Идентификатор устройства для записи регистрации этого устройства.</span><span class="sxs-lookup"><span data-stu-id="55880-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="55880-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="55880-141">deviceName</span></span>|<span data-ttu-id="55880-142">String</span><span class="sxs-lookup"><span data-stu-id="55880-142">String</span></span>|<span data-ttu-id="55880-143">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="55880-143">Device name.</span></span>|
|<span data-ttu-id="55880-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="55880-144">deviceType</span></span>|<span data-ttu-id="55880-145">String</span><span class="sxs-lookup"><span data-stu-id="55880-145">String</span></span>|<span data-ttu-id="55880-146">Тип устройства, например Windows для портативного компьютера Windows и Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="55880-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="55880-147">девицемакаддресс</span><span class="sxs-lookup"><span data-stu-id="55880-147">deviceMacAddress</span></span>|<span data-ttu-id="55880-148">String.</span><span class="sxs-lookup"><span data-stu-id="55880-148">String</span></span>|<span data-ttu-id="55880-149">Mac-адрес устройства.</span><span class="sxs-lookup"><span data-stu-id="55880-149">Device Mac address.</span></span>|
|<span data-ttu-id="55880-150">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="55880-150">lastCheckInDateTime</span></span>|<span data-ttu-id="55880-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55880-151">DateTimeOffset</span></span>|<span data-ttu-id="55880-152">Время последнего возврата устройства.</span><span class="sxs-lookup"><span data-stu-id="55880-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="55880-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="55880-153">Response</span></span>
<span data-ttu-id="55880-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсинформатионпротектиондевицерегистратион](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55880-154">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55880-155">Пример</span><span class="sxs-lookup"><span data-stu-id="55880-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="55880-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="55880-156">Request</span></span>
<span data-ttu-id="55880-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55880-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55880-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="55880-158">Response</span></span>
<span data-ttu-id="55880-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55880-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




