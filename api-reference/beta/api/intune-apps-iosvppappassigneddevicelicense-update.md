---
title: Обновление Иосвппаппассигнеддевицелиценсе
description: Обновление свойств объекта Иосвппаппассигнеддевицелиценсе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88d82be7a799e520093772eb7f449e659353fb55
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761897"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="60212-103">Обновление Иосвппаппассигнеддевицелиценсе</span><span class="sxs-lookup"><span data-stu-id="60212-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="60212-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60212-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60212-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60212-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60212-106">Обновление свойств объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="60212-106">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60212-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="60212-107">Prerequisites</span></span>
<span data-ttu-id="60212-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60212-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60212-110">Permission type</span></span>|<span data-ttu-id="60212-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="60212-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60212-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60212-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60212-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60212-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60212-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60212-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60212-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60212-115">Not supported.</span></span>|
|<span data-ttu-id="60212-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="60212-116">Application</span></span>|<span data-ttu-id="60212-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60212-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60212-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60212-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="60212-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="60212-119">Request headers</span></span>
|<span data-ttu-id="60212-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="60212-120">Header</span></span>|<span data-ttu-id="60212-121">Значение</span><span class="sxs-lookup"><span data-stu-id="60212-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60212-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60212-122">Authorization</span></span>|<span data-ttu-id="60212-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60212-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60212-124">Accept</span><span class="sxs-lookup"><span data-stu-id="60212-124">Accept</span></span>|<span data-ttu-id="60212-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60212-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60212-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60212-126">Request body</span></span>
<span data-ttu-id="60212-127">В тексте запроса добавьте представление объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60212-127">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="60212-128">В следующей таблице приведены свойства, необходимые при создании [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="60212-128">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="60212-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="60212-129">Property</span></span>|<span data-ttu-id="60212-130">Тип</span><span class="sxs-lookup"><span data-stu-id="60212-130">Type</span></span>|<span data-ttu-id="60212-131">Описание</span><span class="sxs-lookup"><span data-stu-id="60212-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60212-132">id</span><span class="sxs-lookup"><span data-stu-id="60212-132">id</span></span>|<span data-ttu-id="60212-133">Строка</span><span class="sxs-lookup"><span data-stu-id="60212-133">String</span></span>|<span data-ttu-id="60212-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="60212-134">Key of the entity.</span></span> <span data-ttu-id="60212-135">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60212-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60212-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="60212-136">userEmailAddress</span></span>|<span data-ttu-id="60212-137">String</span><span class="sxs-lookup"><span data-stu-id="60212-137">String</span></span>|<span data-ttu-id="60212-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="60212-138">The user email address.</span></span> <span data-ttu-id="60212-139">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60212-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60212-140">userId</span><span class="sxs-lookup"><span data-stu-id="60212-140">userId</span></span>|<span data-ttu-id="60212-141">String</span><span class="sxs-lookup"><span data-stu-id="60212-141">String</span></span>|<span data-ttu-id="60212-142">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="60212-142">The user ID.</span></span> <span data-ttu-id="60212-143">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60212-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60212-144">userName</span><span class="sxs-lookup"><span data-stu-id="60212-144">userName</span></span>|<span data-ttu-id="60212-145">String</span><span class="sxs-lookup"><span data-stu-id="60212-145">String</span></span>|<span data-ttu-id="60212-146">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="60212-146">The user name.</span></span> <span data-ttu-id="60212-147">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60212-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60212-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="60212-148">userPrincipalName</span></span>|<span data-ttu-id="60212-149">Строка</span><span class="sxs-lookup"><span data-stu-id="60212-149">String</span></span>|<span data-ttu-id="60212-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="60212-150">The user principal name.</span></span> <span data-ttu-id="60212-151">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="60212-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="60212-152">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="60212-152">managedDeviceId</span></span>|<span data-ttu-id="60212-153">String</span><span class="sxs-lookup"><span data-stu-id="60212-153">String</span></span>|<span data-ttu-id="60212-154">Идентификатор управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="60212-154">The managed device ID.</span></span>|
|<span data-ttu-id="60212-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="60212-155">deviceName</span></span>|<span data-ttu-id="60212-156">String</span><span class="sxs-lookup"><span data-stu-id="60212-156">String</span></span>|<span data-ttu-id="60212-157">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="60212-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="60212-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="60212-158">Response</span></span>
<span data-ttu-id="60212-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60212-159">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60212-160">Пример</span><span class="sxs-lookup"><span data-stu-id="60212-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="60212-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="60212-161">Request</span></span>
<span data-ttu-id="60212-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60212-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60212-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="60212-163">Response</span></span>
<span data-ttu-id="60212-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60212-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




