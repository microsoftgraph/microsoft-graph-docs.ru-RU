---
title: Обновление Иосвппаппассигнеддевицелиценсе
description: Обновление свойств объекта Иосвппаппассигнеддевицелиценсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c1f08f221bb6f3c97619bf25c64f32576910743
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394386"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="eaf2c-103">Обновление Иосвппаппассигнеддевицелиценсе</span><span class="sxs-lookup"><span data-stu-id="eaf2c-103">Update iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="eaf2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaf2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaf2c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaf2c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaf2c-107">Обновление свойств объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf2c-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaf2c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eaf2c-108">Prerequisites</span></span>
<span data-ttu-id="eaf2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf2c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf2c-111">Permission type</span></span>|<span data-ttu-id="eaf2c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaf2c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaf2c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf2c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eaf2c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaf2c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-116">Not supported.</span></span>|
|<span data-ttu-id="eaf2c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaf2c-117">Application</span></span>|<span data-ttu-id="eaf2c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf2c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaf2c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaf2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="eaf2c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eaf2c-120">Request headers</span></span>
|<span data-ttu-id="eaf2c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaf2c-121">Header</span></span>|<span data-ttu-id="eaf2c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eaf2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaf2c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eaf2c-123">Authorization</span></span>|<span data-ttu-id="eaf2c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaf2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eaf2c-125">Accept</span></span>|<span data-ttu-id="eaf2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eaf2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf2c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eaf2c-127">Request body</span></span>
<span data-ttu-id="eaf2c-128">В тексте запроса добавьте представление объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="eaf2c-129">В следующей таблице приведены свойства, необходимые при создании [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="eaf2c-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="eaf2c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaf2c-130">Property</span></span>|<span data-ttu-id="eaf2c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eaf2c-131">Type</span></span>|<span data-ttu-id="eaf2c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf2c-133">id</span><span class="sxs-lookup"><span data-stu-id="eaf2c-133">id</span></span>|<span data-ttu-id="eaf2c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="eaf2c-134">String</span></span>|<span data-ttu-id="eaf2c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-135">Key of the entity.</span></span> <span data-ttu-id="eaf2c-136">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="eaf2c-137">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="eaf2c-137">userEmailAddress</span></span>|<span data-ttu-id="eaf2c-138">String</span><span class="sxs-lookup"><span data-stu-id="eaf2c-138">String</span></span>|<span data-ttu-id="eaf2c-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-139">The user email address.</span></span> <span data-ttu-id="eaf2c-140">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="eaf2c-141">userId</span><span class="sxs-lookup"><span data-stu-id="eaf2c-141">userId</span></span>|<span data-ttu-id="eaf2c-142">String</span><span class="sxs-lookup"><span data-stu-id="eaf2c-142">String</span></span>|<span data-ttu-id="eaf2c-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-143">The user ID.</span></span> <span data-ttu-id="eaf2c-144">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="eaf2c-145">userName</span><span class="sxs-lookup"><span data-stu-id="eaf2c-145">userName</span></span>|<span data-ttu-id="eaf2c-146">String</span><span class="sxs-lookup"><span data-stu-id="eaf2c-146">String</span></span>|<span data-ttu-id="eaf2c-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-147">The user name.</span></span> <span data-ttu-id="eaf2c-148">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="eaf2c-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eaf2c-149">userPrincipalName</span></span>|<span data-ttu-id="eaf2c-150">Строка</span><span class="sxs-lookup"><span data-stu-id="eaf2c-150">String</span></span>|<span data-ttu-id="eaf2c-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-151">The user principal name.</span></span> <span data-ttu-id="eaf2c-152">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="eaf2c-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="eaf2c-153">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="eaf2c-153">managedDeviceId</span></span>|<span data-ttu-id="eaf2c-154">String</span><span class="sxs-lookup"><span data-stu-id="eaf2c-154">String</span></span>|<span data-ttu-id="eaf2c-155">Идентификатор управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-155">The managed device ID.</span></span>|
|<span data-ttu-id="eaf2c-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="eaf2c-156">deviceName</span></span>|<span data-ttu-id="eaf2c-157">String</span><span class="sxs-lookup"><span data-stu-id="eaf2c-157">String</span></span>|<span data-ttu-id="eaf2c-158">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="eaf2c-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="eaf2c-159">Response</span></span>
<span data-ttu-id="eaf2c-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaf2c-161">Пример</span><span class="sxs-lookup"><span data-stu-id="eaf2c-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaf2c-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaf2c-162">Request</span></span>
<span data-ttu-id="eaf2c-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eaf2c-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaf2c-164">Response</span></span>
<span data-ttu-id="eaf2c-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaf2c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



