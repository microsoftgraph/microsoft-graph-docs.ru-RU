---
title: Создание Иосвппаппассигнеддевицелиценсе
description: Создание нового объекта Иосвппаппассигнеддевицелиценсе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e541e2233835a13c6c0fa348c6d57e0ceab03c9a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761925"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="354be-103">Создание Иосвппаппассигнеддевицелиценсе</span><span class="sxs-lookup"><span data-stu-id="354be-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="354be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="354be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="354be-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="354be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="354be-106">Создание нового объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="354be-106">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="354be-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="354be-107">Prerequisites</span></span>
<span data-ttu-id="354be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="354be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="354be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="354be-110">Permission type</span></span>|<span data-ttu-id="354be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="354be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="354be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="354be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="354be-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="354be-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="354be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="354be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="354be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="354be-115">Not supported.</span></span>|
|<span data-ttu-id="354be-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="354be-116">Application</span></span>|<span data-ttu-id="354be-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="354be-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="354be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="354be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="354be-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="354be-119">Request headers</span></span>
|<span data-ttu-id="354be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="354be-120">Header</span></span>|<span data-ttu-id="354be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="354be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="354be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="354be-122">Authorization</span></span>|<span data-ttu-id="354be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="354be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="354be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="354be-124">Accept</span></span>|<span data-ttu-id="354be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="354be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="354be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="354be-126">Request body</span></span>
<span data-ttu-id="354be-127">В тексте запроса добавьте представление объекта Иосвппаппассигнеддевицелиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="354be-127">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="354be-128">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнеддевицелиценсе.</span><span class="sxs-lookup"><span data-stu-id="354be-128">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="354be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="354be-129">Property</span></span>|<span data-ttu-id="354be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="354be-130">Type</span></span>|<span data-ttu-id="354be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="354be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="354be-132">id</span><span class="sxs-lookup"><span data-stu-id="354be-132">id</span></span>|<span data-ttu-id="354be-133">Строка</span><span class="sxs-lookup"><span data-stu-id="354be-133">String</span></span>|<span data-ttu-id="354be-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="354be-134">Key of the entity.</span></span> <span data-ttu-id="354be-135">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="354be-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="354be-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="354be-136">userEmailAddress</span></span>|<span data-ttu-id="354be-137">String</span><span class="sxs-lookup"><span data-stu-id="354be-137">String</span></span>|<span data-ttu-id="354be-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="354be-138">The user email address.</span></span> <span data-ttu-id="354be-139">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="354be-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="354be-140">userId</span><span class="sxs-lookup"><span data-stu-id="354be-140">userId</span></span>|<span data-ttu-id="354be-141">String</span><span class="sxs-lookup"><span data-stu-id="354be-141">String</span></span>|<span data-ttu-id="354be-142">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="354be-142">The user ID.</span></span> <span data-ttu-id="354be-143">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="354be-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="354be-144">userName</span><span class="sxs-lookup"><span data-stu-id="354be-144">userName</span></span>|<span data-ttu-id="354be-145">String</span><span class="sxs-lookup"><span data-stu-id="354be-145">String</span></span>|<span data-ttu-id="354be-146">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="354be-146">The user name.</span></span> <span data-ttu-id="354be-147">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="354be-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="354be-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="354be-148">userPrincipalName</span></span>|<span data-ttu-id="354be-149">Строка</span><span class="sxs-lookup"><span data-stu-id="354be-149">String</span></span>|<span data-ttu-id="354be-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="354be-150">The user principal name.</span></span> <span data-ttu-id="354be-151">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="354be-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="354be-152">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="354be-152">managedDeviceId</span></span>|<span data-ttu-id="354be-153">String</span><span class="sxs-lookup"><span data-stu-id="354be-153">String</span></span>|<span data-ttu-id="354be-154">Идентификатор управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="354be-154">The managed device ID.</span></span>|
|<span data-ttu-id="354be-155">deviceName</span><span class="sxs-lookup"><span data-stu-id="354be-155">deviceName</span></span>|<span data-ttu-id="354be-156">String</span><span class="sxs-lookup"><span data-stu-id="354be-156">String</span></span>|<span data-ttu-id="354be-157">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="354be-157">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="354be-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="354be-158">Response</span></span>
<span data-ttu-id="354be-159">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="354be-159">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="354be-160">Пример</span><span class="sxs-lookup"><span data-stu-id="354be-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="354be-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="354be-161">Request</span></span>
<span data-ttu-id="354be-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="354be-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="354be-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="354be-163">Response</span></span>
<span data-ttu-id="354be-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="354be-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




