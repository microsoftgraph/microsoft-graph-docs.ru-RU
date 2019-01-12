---
title: Создание iosVppAppAssignedDeviceLicense
description: Создание нового объекта iosVppAppAssignedDeviceLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c4eecadae91eb857a5b90c88d66af1721f268ddb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914383"
---
# <a name="create-iosvppappassigneddevicelicense"></a><span data-ttu-id="1d4cd-103">Создание iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="1d4cd-103">Create iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="1d4cd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d4cd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d4cd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d4cd-107">Создание нового объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1d4cd-107">Create a new [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d4cd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d4cd-108">Prerequisites</span></span>
<span data-ttu-id="1d4cd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d4cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d4cd-111">Permission type</span></span>|<span data-ttu-id="1d4cd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d4cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d4cd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4cd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d4cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d4cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-116">Not supported.</span></span>|
|<span data-ttu-id="1d4cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d4cd-117">Application</span></span>|<span data-ttu-id="1d4cd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d4cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d4cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="1d4cd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d4cd-120">Request headers</span></span>
|<span data-ttu-id="1d4cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d4cd-121">Header</span></span>|<span data-ttu-id="1d4cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d4cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d4cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d4cd-123">Authorization</span></span>|<span data-ttu-id="1d4cd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1d4cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d4cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d4cd-125">Accept</span></span>|<span data-ttu-id="1d4cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d4cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d4cd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d4cd-127">Request body</span></span>
<span data-ttu-id="1d4cd-128">В тексте запроса укажите представление JSON для объекта iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-128">In the request body, supply a JSON representation for the iosVppAppAssignedDeviceLicense object.</span></span>

<span data-ttu-id="1d4cd-129">В следующей таблице показаны свойства, которые необходимы для создания iosVppAppAssignedDeviceLicense.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-129">The following table shows the properties that are required when you create the iosVppAppAssignedDeviceLicense.</span></span>

|<span data-ttu-id="1d4cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d4cd-130">Property</span></span>|<span data-ttu-id="1d4cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1d4cd-131">Type</span></span>|<span data-ttu-id="1d4cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1d4cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4cd-133">id</span><span class="sxs-lookup"><span data-stu-id="1d4cd-133">id</span></span>|<span data-ttu-id="1d4cd-134">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-134">String</span></span>|<span data-ttu-id="1d4cd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-135">Key of the entity.</span></span> <span data-ttu-id="1d4cd-136">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1d4cd-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1d4cd-137">userEmailAddress</span></span>|<span data-ttu-id="1d4cd-138">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-138">String</span></span>|<span data-ttu-id="1d4cd-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-139">The user email address.</span></span> <span data-ttu-id="1d4cd-140">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1d4cd-141">userId</span><span class="sxs-lookup"><span data-stu-id="1d4cd-141">userId</span></span>|<span data-ttu-id="1d4cd-142">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-142">String</span></span>|<span data-ttu-id="1d4cd-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-143">The user ID.</span></span> <span data-ttu-id="1d4cd-144">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1d4cd-145">userName</span><span class="sxs-lookup"><span data-stu-id="1d4cd-145">userName</span></span>|<span data-ttu-id="1d4cd-146">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-146">String</span></span>|<span data-ttu-id="1d4cd-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-147">The user name.</span></span> <span data-ttu-id="1d4cd-148">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1d4cd-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1d4cd-149">userPrincipalName</span></span>|<span data-ttu-id="1d4cd-150">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-150">String</span></span>|<span data-ttu-id="1d4cd-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-151">The user principal name.</span></span> <span data-ttu-id="1d4cd-152">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1d4cd-153">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1d4cd-153">managedDeviceId</span></span>|<span data-ttu-id="1d4cd-154">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-154">String</span></span>|<span data-ttu-id="1d4cd-155">С идентификатором управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-155">The managed device ID.</span></span>|
|<span data-ttu-id="1d4cd-156">deviceName</span><span class="sxs-lookup"><span data-stu-id="1d4cd-156">deviceName</span></span>|<span data-ttu-id="1d4cd-157">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-157">String</span></span>|<span data-ttu-id="1d4cd-158">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-158">The device name.</span></span>|



## <a name="response"></a><span data-ttu-id="1d4cd-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d4cd-159">Response</span></span>
<span data-ttu-id="1d4cd-160">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-160">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d4cd-161">Пример</span><span class="sxs-lookup"><span data-stu-id="1d4cd-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d4cd-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d4cd-162">Request</span></span>
<span data-ttu-id="1d4cd-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d4cd-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d4cd-164">Response</span></span>
<span data-ttu-id="1d4cd-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





