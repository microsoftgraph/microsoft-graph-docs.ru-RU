---
title: Создание iosVppAppAssignedDeviceLicense
description: Создайте новый объект iosVppAppAssignedDeviceLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6ea8cf269a3b5735a366000fb49fd8479eebef2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140644"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="fa22a-103">Создание iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="fa22a-103">Create iosVppAppAssignedDeviceLicense</span></span>

<span data-ttu-id="fa22a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa22a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa22a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa22a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa22a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa22a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa22a-107">Создайте новый [объект iosVppAppAssignedDeviceLicense.](../resources/intune-apps-iosvppappassigneddevicelicense.md)</span><span class="sxs-lookup"><span data-stu-id="fa22a-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa22a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa22a-108">Prerequisites</span></span>
<span data-ttu-id="fa22a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa22a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa22a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa22a-111">Permission type</span></span>|<span data-ttu-id="fa22a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa22a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa22a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa22a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa22a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa22a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa22a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa22a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa22a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa22a-116">Not supported.</span></span>|
|<span data-ttu-id="fa22a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fa22a-117">Application</span></span>|<span data-ttu-id="fa22a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa22a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa22a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa22a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="fa22a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa22a-120">Request headers</span></span>
|<span data-ttu-id="fa22a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa22a-121">Header</span></span>|<span data-ttu-id="fa22a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa22a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa22a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa22a-123">Authorization</span></span>|<span data-ttu-id="fa22a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa22a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa22a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa22a-125">Accept</span></span>|<span data-ttu-id="fa22a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa22a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa22a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa22a-127">Request body</span></span>
<span data-ttu-id="fa22a-128">В теле запроса поставляем представление JSON для объекта iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="fa22a-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="fa22a-129">В следующей таблице показаны свойства, необходимые при создании iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="fa22a-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="fa22a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa22a-130">Property</span></span>|<span data-ttu-id="fa22a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa22a-131">Type</span></span>|<span data-ttu-id="fa22a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa22a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa22a-133">id</span><span class="sxs-lookup"><span data-stu-id="fa22a-133">id</span></span>|<span data-ttu-id="fa22a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fa22a-134">String</span></span>|<span data-ttu-id="fa22a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fa22a-135">Key of the entity.</span></span> <span data-ttu-id="fa22a-136">Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fa22a-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fa22a-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fa22a-137">userEmailAddress</span></span>|<span data-ttu-id="fa22a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fa22a-138">String</span></span>|<span data-ttu-id="fa22a-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa22a-139">The user email address.</span></span> <span data-ttu-id="fa22a-140">Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fa22a-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fa22a-141">userId</span><span class="sxs-lookup"><span data-stu-id="fa22a-141">userId</span></span>|<span data-ttu-id="fa22a-142">String</span><span class="sxs-lookup"><span data-stu-id="fa22a-142">String</span></span>|<span data-ttu-id="fa22a-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa22a-143">The user ID.</span></span> <span data-ttu-id="fa22a-144">Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fa22a-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fa22a-145">userName</span><span class="sxs-lookup"><span data-stu-id="fa22a-145">userName</span></span>|<span data-ttu-id="fa22a-146">String</span><span class="sxs-lookup"><span data-stu-id="fa22a-146">String</span></span>|<span data-ttu-id="fa22a-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa22a-147">The user name.</span></span> <span data-ttu-id="fa22a-148">Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fa22a-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fa22a-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fa22a-149">userPrincipalName</span></span>|<span data-ttu-id="fa22a-150">String</span><span class="sxs-lookup"><span data-stu-id="fa22a-150">String</span></span>|<span data-ttu-id="fa22a-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa22a-151">The user principal name.</span></span> <span data-ttu-id="fa22a-152">Унаследованный от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fa22a-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="fa22a-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="fa22a-153">managedDeviceId</span></span>|<span data-ttu-id="fa22a-154">Строка</span><span class="sxs-lookup"><span data-stu-id="fa22a-154">String</span></span>|<span data-ttu-id="fa22a-155">ID управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="fa22a-155">The managed device ID.</span></span>|
|<span data-ttu-id="fa22a-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="fa22a-156">deviceName</span></span>|<span data-ttu-id="fa22a-157">String</span><span class="sxs-lookup"><span data-stu-id="fa22a-157">String</span></span>|<span data-ttu-id="fa22a-158">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="fa22a-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="fa22a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa22a-159">Response</span></span>
<span data-ttu-id="fa22a-160">В случае успеха этот метод возвращает код ответа и `201 Created` [объект iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fa22a-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa22a-161">Пример</span><span class="sxs-lookup"><span data-stu-id="fa22a-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa22a-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa22a-162">Request</span></span>
<span data-ttu-id="fa22a-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa22a-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa22a-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa22a-164">Response</span></span>
<span data-ttu-id="fa22a-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa22a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




