---
title: Обновление iosVppAppAssignedDeviceLicense
description: Обновление свойства объекта iosVppAppAssignedDeviceLicense.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2edd886b0ab9b302e7f224511bb329fe8269a7d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402127"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="27baf-103">Обновление iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="27baf-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="27baf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="27baf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27baf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27baf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27baf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27baf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27baf-107">Обновление свойства объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="27baf-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27baf-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="27baf-108">Prerequisites</span></span>
<span data-ttu-id="27baf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="27baf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="27baf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27baf-111">Permission type</span></span>|<span data-ttu-id="27baf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27baf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27baf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27baf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27baf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27baf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27baf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27baf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27baf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27baf-116">Not supported.</span></span>|
|<span data-ttu-id="27baf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27baf-117">Application</span></span>|<span data-ttu-id="27baf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27baf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27baf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27baf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="27baf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27baf-120">Request headers</span></span>
|<span data-ttu-id="27baf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27baf-121">Header</span></span>|<span data-ttu-id="27baf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="27baf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27baf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27baf-123">Authorization</span></span>|<span data-ttu-id="27baf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="27baf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27baf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27baf-125">Accept</span></span>|<span data-ttu-id="27baf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27baf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27baf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27baf-127">Request body</span></span>
<span data-ttu-id="27baf-128">В тексте запроса укажите представление JSON для объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="27baf-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="27baf-129">В следующей таблице показаны свойства, которые необходимы для создания [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="27baf-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="27baf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="27baf-130">Property</span></span>|<span data-ttu-id="27baf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="27baf-131">Type</span></span>|<span data-ttu-id="27baf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="27baf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27baf-133">id</span><span class="sxs-lookup"><span data-stu-id="27baf-133">id</span></span>|<span data-ttu-id="27baf-134">String</span><span class="sxs-lookup"><span data-stu-id="27baf-134">String</span></span>|<span data-ttu-id="27baf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="27baf-135">Key of the entity.</span></span> <span data-ttu-id="27baf-136">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="27baf-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="27baf-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="27baf-137">userEmailAddress</span></span>|<span data-ttu-id="27baf-138">String</span><span class="sxs-lookup"><span data-stu-id="27baf-138">String</span></span>|<span data-ttu-id="27baf-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="27baf-139">The user email address.</span></span> <span data-ttu-id="27baf-140">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="27baf-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="27baf-141">userId</span><span class="sxs-lookup"><span data-stu-id="27baf-141">userId</span></span>|<span data-ttu-id="27baf-142">String</span><span class="sxs-lookup"><span data-stu-id="27baf-142">String</span></span>|<span data-ttu-id="27baf-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="27baf-143">The user ID.</span></span> <span data-ttu-id="27baf-144">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="27baf-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="27baf-145">userName</span><span class="sxs-lookup"><span data-stu-id="27baf-145">userName</span></span>|<span data-ttu-id="27baf-146">String</span><span class="sxs-lookup"><span data-stu-id="27baf-146">String</span></span>|<span data-ttu-id="27baf-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="27baf-147">The user name.</span></span> <span data-ttu-id="27baf-148">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="27baf-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="27baf-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27baf-149">userPrincipalName</span></span>|<span data-ttu-id="27baf-150">String</span><span class="sxs-lookup"><span data-stu-id="27baf-150">String</span></span>|<span data-ttu-id="27baf-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="27baf-151">The user principal name.</span></span> <span data-ttu-id="27baf-152">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="27baf-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="27baf-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="27baf-153">managedDeviceId</span></span>|<span data-ttu-id="27baf-154">String</span><span class="sxs-lookup"><span data-stu-id="27baf-154">String</span></span>|<span data-ttu-id="27baf-155">С идентификатором управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="27baf-155">The managed device ID.</span></span>|
|<span data-ttu-id="27baf-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="27baf-156">deviceName</span></span>|<span data-ttu-id="27baf-157">String</span><span class="sxs-lookup"><span data-stu-id="27baf-157">String</span></span>|<span data-ttu-id="27baf-158">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="27baf-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="27baf-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="27baf-159">Response</span></span>
<span data-ttu-id="27baf-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="27baf-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27baf-161">Пример</span><span class="sxs-lookup"><span data-stu-id="27baf-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="27baf-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="27baf-162">Request</span></span>
<span data-ttu-id="27baf-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27baf-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27baf-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="27baf-164">Response</span></span>
<span data-ttu-id="27baf-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="27baf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




