---
title: Обновление Иосвппаппассигнеддевицелиценсе
description: Обновление свойств объекта Иосвппаппассигнеддевицелиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83fabd3202391f5e466c5b5bd9af895ed82af0aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445528"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="79602-103">Обновление Иосвппаппассигнеддевицелиценсе</span><span class="sxs-lookup"><span data-stu-id="79602-103">Update iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="79602-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="79602-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79602-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79602-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79602-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79602-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79602-107">Обновление свойств объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="79602-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79602-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="79602-108">Prerequisites</span></span>
<span data-ttu-id="79602-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79602-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79602-111">Permission type</span></span>|<span data-ttu-id="79602-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79602-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79602-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79602-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79602-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79602-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79602-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79602-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79602-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79602-116">Not supported.</span></span>|
|<span data-ttu-id="79602-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79602-117">Application</span></span>|<span data-ttu-id="79602-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79602-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79602-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79602-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="79602-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="79602-120">Request headers</span></span>
|<span data-ttu-id="79602-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79602-121">Header</span></span>|<span data-ttu-id="79602-122">Значение</span><span class="sxs-lookup"><span data-stu-id="79602-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79602-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79602-123">Authorization</span></span>|<span data-ttu-id="79602-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79602-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79602-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79602-125">Accept</span></span>|<span data-ttu-id="79602-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79602-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79602-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79602-127">Request body</span></span>
<span data-ttu-id="79602-128">В тексте запроса добавьте представление объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79602-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="79602-129">В следующей таблице приведены свойства, необходимые при создании [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="79602-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="79602-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="79602-130">Property</span></span>|<span data-ttu-id="79602-131">Тип</span><span class="sxs-lookup"><span data-stu-id="79602-131">Type</span></span>|<span data-ttu-id="79602-132">Описание</span><span class="sxs-lookup"><span data-stu-id="79602-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79602-133">id</span><span class="sxs-lookup"><span data-stu-id="79602-133">id</span></span>|<span data-ttu-id="79602-134">Строка</span><span class="sxs-lookup"><span data-stu-id="79602-134">String</span></span>|<span data-ttu-id="79602-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79602-135">Key of the entity.</span></span> <span data-ttu-id="79602-136">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79602-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79602-137">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="79602-137">userEmailAddress</span></span>|<span data-ttu-id="79602-138">String</span><span class="sxs-lookup"><span data-stu-id="79602-138">String</span></span>|<span data-ttu-id="79602-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="79602-139">The user email address.</span></span> <span data-ttu-id="79602-140">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79602-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79602-141">userId</span><span class="sxs-lookup"><span data-stu-id="79602-141">userId</span></span>|<span data-ttu-id="79602-142">String</span><span class="sxs-lookup"><span data-stu-id="79602-142">String</span></span>|<span data-ttu-id="79602-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="79602-143">The user ID.</span></span> <span data-ttu-id="79602-144">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79602-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79602-145">userName</span><span class="sxs-lookup"><span data-stu-id="79602-145">userName</span></span>|<span data-ttu-id="79602-146">String</span><span class="sxs-lookup"><span data-stu-id="79602-146">String</span></span>|<span data-ttu-id="79602-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="79602-147">The user name.</span></span> <span data-ttu-id="79602-148">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79602-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79602-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79602-149">userPrincipalName</span></span>|<span data-ttu-id="79602-150">Строка</span><span class="sxs-lookup"><span data-stu-id="79602-150">String</span></span>|<span data-ttu-id="79602-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="79602-151">The user principal name.</span></span> <span data-ttu-id="79602-152">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="79602-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="79602-153">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="79602-153">managedDeviceId</span></span>|<span data-ttu-id="79602-154">String</span><span class="sxs-lookup"><span data-stu-id="79602-154">String</span></span>|<span data-ttu-id="79602-155">Идентификатор управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="79602-155">The managed device ID.</span></span>|
|<span data-ttu-id="79602-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="79602-156">deviceName</span></span>|<span data-ttu-id="79602-157">String</span><span class="sxs-lookup"><span data-stu-id="79602-157">String</span></span>|<span data-ttu-id="79602-158">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="79602-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="79602-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="79602-159">Response</span></span>
<span data-ttu-id="79602-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79602-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79602-161">Пример</span><span class="sxs-lookup"><span data-stu-id="79602-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="79602-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="79602-162">Request</span></span>
<span data-ttu-id="79602-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79602-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="79602-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="79602-164">Response</span></span>
<span data-ttu-id="79602-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79602-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```





