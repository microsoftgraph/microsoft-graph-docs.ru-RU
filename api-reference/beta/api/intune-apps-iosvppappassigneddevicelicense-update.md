---
title: Обновление iosVppAppAssignedDeviceLicense
description: Обновление свойства объекта iosVppAppAssignedDeviceLicense.
author: tfitzmac
ms.openlocfilehash: 69ccb35896864a29bf594da74afeb702a4b963bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353230"
---
# <a name="update-iosvppappassigneddevicelicense"></a><span data-ttu-id="1ec31-103">Обновление iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="1ec31-103">Update iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="1ec31-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1ec31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ec31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ec31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ec31-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ec31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ec31-107">Обновление свойства объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1ec31-107">Update the properties of a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ec31-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ec31-108">Prerequisites</span></span>
<span data-ttu-id="1ec31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ec31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ec31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ec31-111">Permission type</span></span>|<span data-ttu-id="1ec31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ec31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ec31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ec31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ec31-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ec31-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ec31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ec31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ec31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ec31-116">Not supported.</span></span>|
|<span data-ttu-id="1ec31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ec31-117">Application</span></span>|<span data-ttu-id="1ec31-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ec31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ec31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ec31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="1ec31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ec31-120">Request headers</span></span>
|<span data-ttu-id="1ec31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ec31-121">Header</span></span>|<span data-ttu-id="1ec31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1ec31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ec31-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ec31-123">Authorization</span></span>|<span data-ttu-id="1ec31-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1ec31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ec31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ec31-125">Accept</span></span>|<span data-ttu-id="1ec31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ec31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ec31-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ec31-127">Request body</span></span>
<span data-ttu-id="1ec31-128">В тексте запроса укажите представление JSON для объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1ec31-128">In the request body, supply a JSON representation for the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>

<span data-ttu-id="1ec31-129">В следующей таблице показаны свойства, которые необходимы для создания [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span><span class="sxs-lookup"><span data-stu-id="1ec31-129">The following table shows the properties that are required when you create the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).</span></span>

|<span data-ttu-id="1ec31-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ec31-130">Property</span></span>|<span data-ttu-id="1ec31-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ec31-131">Type</span></span>|<span data-ttu-id="1ec31-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ec31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ec31-133">id</span><span class="sxs-lookup"><span data-stu-id="1ec31-133">id</span></span>|<span data-ttu-id="1ec31-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1ec31-134">String</span></span>|<span data-ttu-id="1ec31-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1ec31-135">Key of the entity.</span></span> <span data-ttu-id="1ec31-136">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1ec31-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1ec31-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1ec31-137">userEmailAddress</span></span>|<span data-ttu-id="1ec31-138">String.</span><span class="sxs-lookup"><span data-stu-id="1ec31-138">String</span></span>|<span data-ttu-id="1ec31-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ec31-139">The user email address.</span></span> <span data-ttu-id="1ec31-140">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1ec31-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1ec31-141">userId</span><span class="sxs-lookup"><span data-stu-id="1ec31-141">userId</span></span>|<span data-ttu-id="1ec31-142">String</span><span class="sxs-lookup"><span data-stu-id="1ec31-142">String</span></span>|<span data-ttu-id="1ec31-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ec31-143">The user ID.</span></span> <span data-ttu-id="1ec31-144">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1ec31-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1ec31-145">userName</span><span class="sxs-lookup"><span data-stu-id="1ec31-145">userName</span></span>|<span data-ttu-id="1ec31-146">String</span><span class="sxs-lookup"><span data-stu-id="1ec31-146">String</span></span>|<span data-ttu-id="1ec31-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ec31-147">The user name.</span></span> <span data-ttu-id="1ec31-148">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1ec31-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1ec31-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1ec31-149">userPrincipalName</span></span>|<span data-ttu-id="1ec31-150">Строка</span><span class="sxs-lookup"><span data-stu-id="1ec31-150">String</span></span>|<span data-ttu-id="1ec31-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ec31-151">The user principal name.</span></span> <span data-ttu-id="1ec31-152">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1ec31-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1ec31-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1ec31-153">managedDeviceId</span></span>|<span data-ttu-id="1ec31-154">String.</span><span class="sxs-lookup"><span data-stu-id="1ec31-154">String</span></span>|<span data-ttu-id="1ec31-155">С идентификатором управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="1ec31-155">The managed device ID.</span></span>|
|<span data-ttu-id="1ec31-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="1ec31-156">deviceName</span></span>|<span data-ttu-id="1ec31-157">String</span><span class="sxs-lookup"><span data-stu-id="1ec31-157">String</span></span>|<span data-ttu-id="1ec31-158">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="1ec31-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="1ec31-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ec31-159">Response</span></span>
<span data-ttu-id="1ec31-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1ec31-160">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ec31-161">Пример</span><span class="sxs-lookup"><span data-stu-id="1ec31-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ec31-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ec31-162">Request</span></span>
<span data-ttu-id="1ec31-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ec31-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 258

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="1ec31-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ec31-164">Response</span></span>
<span data-ttu-id="1ec31-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1ec31-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





