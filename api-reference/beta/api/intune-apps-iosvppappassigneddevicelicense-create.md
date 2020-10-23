---
title: Создание Иосвппаппассигнеддевицелиценсе
description: Создание нового объекта Иосвппаппассигнеддевицелиценсе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34493235d82c4c241f6c4652ca53abdd37848177
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700138"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="ca8eb-103">Создание Иосвппаппассигнеддевицелиценсе</span><span class="sxs-lookup"><span data-stu-id="ca8eb-103">Create iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="ca8eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca8eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca8eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca8eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca8eb-107">Создание нового объекта [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="ca8eb-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca8eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ca8eb-108">Prerequisites</span></span>
<span data-ttu-id="ca8eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca8eb-111">Permission type</span></span>|<span data-ttu-id="ca8eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca8eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca8eb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8eb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ca8eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca8eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-116">Not supported.</span></span>|
|<span data-ttu-id="ca8eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca8eb-117">Application</span></span>|<span data-ttu-id="ca8eb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8eb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca8eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca8eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="ca8eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ca8eb-120">Request headers</span></span>
|<span data-ttu-id="ca8eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca8eb-121">Header</span></span>|<span data-ttu-id="ca8eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca8eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca8eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca8eb-123">Authorization</span></span>|<span data-ttu-id="ca8eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca8eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca8eb-125">Accept</span></span>|<span data-ttu-id="ca8eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca8eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca8eb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca8eb-127">Request body</span></span>
<span data-ttu-id="ca8eb-128">В тексте запроса добавьте представление объекта Иосвппаппассигнеддевицелиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="ca8eb-129">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнеддевицелиценсе.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="ca8eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca8eb-130">Property</span></span>|<span data-ttu-id="ca8eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca8eb-131">Type</span></span>|<span data-ttu-id="ca8eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca8eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca8eb-133">id</span><span class="sxs-lookup"><span data-stu-id="ca8eb-133">id</span></span>|<span data-ttu-id="ca8eb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8eb-134">String</span></span>|<span data-ttu-id="ca8eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-135">Key of the entity.</span></span> <span data-ttu-id="ca8eb-136">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ca8eb-137">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="ca8eb-137">userEmailAddress</span></span>|<span data-ttu-id="ca8eb-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8eb-138">String</span></span>|<span data-ttu-id="ca8eb-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-139">The user email address.</span></span> <span data-ttu-id="ca8eb-140">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ca8eb-141">userId</span><span class="sxs-lookup"><span data-stu-id="ca8eb-141">userId</span></span>|<span data-ttu-id="ca8eb-142">String</span><span class="sxs-lookup"><span data-stu-id="ca8eb-142">String</span></span>|<span data-ttu-id="ca8eb-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-143">The user ID.</span></span> <span data-ttu-id="ca8eb-144">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ca8eb-145">userName</span><span class="sxs-lookup"><span data-stu-id="ca8eb-145">userName</span></span>|<span data-ttu-id="ca8eb-146">String</span><span class="sxs-lookup"><span data-stu-id="ca8eb-146">String</span></span>|<span data-ttu-id="ca8eb-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-147">The user name.</span></span> <span data-ttu-id="ca8eb-148">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ca8eb-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ca8eb-149">userPrincipalName</span></span>|<span data-ttu-id="ca8eb-150">String</span><span class="sxs-lookup"><span data-stu-id="ca8eb-150">String</span></span>|<span data-ttu-id="ca8eb-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-151">The user principal name.</span></span> <span data-ttu-id="ca8eb-152">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ca8eb-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ca8eb-153">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="ca8eb-153">managedDeviceId</span></span>|<span data-ttu-id="ca8eb-154">Строка</span><span class="sxs-lookup"><span data-stu-id="ca8eb-154">String</span></span>|<span data-ttu-id="ca8eb-155">Идентификатор управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-155">The managed device ID.</span></span>|
|<span data-ttu-id="ca8eb-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="ca8eb-156">deviceName</span></span>|<span data-ttu-id="ca8eb-157">String</span><span class="sxs-lookup"><span data-stu-id="ca8eb-157">String</span></span>|<span data-ttu-id="ca8eb-158">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="ca8eb-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca8eb-159">Response</span></span>
<span data-ttu-id="ca8eb-160">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнеддевицелиценсе](../resources/intune-apps-iosvppappassigneddevicelicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8eb-161">Пример</span><span class="sxs-lookup"><span data-stu-id="ca8eb-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca8eb-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca8eb-162">Request</span></span>
<span data-ttu-id="ca8eb-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca8eb-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca8eb-164">Response</span></span>
<span data-ttu-id="ca8eb-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca8eb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





