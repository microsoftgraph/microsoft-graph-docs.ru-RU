---
title: Обновление mobileAppInstallSummary
description: Обновление свойства объекта mobileAppInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3886512ff2524ccf2ac424d198533ebaafae20ee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930063"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="5e449-103">Обновление mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e449-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="5e449-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e449-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e449-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e449-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e449-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e449-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e449-107">Обновление свойства объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5e449-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e449-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e449-108">Prerequisites</span></span>
<span data-ttu-id="5e449-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e449-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e449-111">Permission type</span></span>|<span data-ttu-id="5e449-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e449-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e449-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e449-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e449-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e449-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5e449-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e449-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e449-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e449-116">Not supported.</span></span>|
|<span data-ttu-id="5e449-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e449-117">Application</span></span>|<span data-ttu-id="5e449-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e449-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e449-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e449-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="5e449-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e449-120">Request headers</span></span>
|<span data-ttu-id="5e449-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e449-121">Header</span></span>|<span data-ttu-id="5e449-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e449-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e449-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e449-123">Authorization</span></span>|<span data-ttu-id="5e449-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5e449-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e449-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e449-125">Accept</span></span>|<span data-ttu-id="5e449-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e449-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e449-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e449-127">Request body</span></span>
<span data-ttu-id="5e449-128">В тексте запроса укажите представление JSON для объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="5e449-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="5e449-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="5e449-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="5e449-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e449-130">Property</span></span>|<span data-ttu-id="5e449-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5e449-131">Type</span></span>|<span data-ttu-id="5e449-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5e449-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e449-133">id</span><span class="sxs-lookup"><span data-stu-id="5e449-133">id</span></span>|<span data-ttu-id="5e449-134">String</span><span class="sxs-lookup"><span data-stu-id="5e449-134">String</span></span>|<span data-ttu-id="5e449-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e449-135">Key of the entity.</span></span>|
|<span data-ttu-id="5e449-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e449-136">installedDeviceCount</span></span>|<span data-ttu-id="5e449-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-137">Int32</span></span>|<span data-ttu-id="5e449-138">Количество устройств, которые были успешно установлены этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5e449-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="5e449-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e449-139">failedDeviceCount</span></span>|<span data-ttu-id="5e449-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-140">Int32</span></span>|<span data-ttu-id="5e449-141">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="5e449-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="5e449-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e449-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="5e449-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-143">Int32</span></span>|<span data-ttu-id="5e449-144">Количество устройств, которые не применимы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5e449-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="5e449-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e449-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="5e449-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-146">Int32</span></span>|<span data-ttu-id="5e449-147">Количество устройств, для которого не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="5e449-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="5e449-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e449-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="5e449-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-149">Int32</span></span>|<span data-ttu-id="5e449-150">Количество устройств, которые были уведомлены для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5e449-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="5e449-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="5e449-151">installedUserCount</span></span>|<span data-ttu-id="5e449-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-152">Int32</span></span>|<span data-ttu-id="5e449-153">Число пользователей, чьи устройств успешно для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5e449-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="5e449-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5e449-154">failedUserCount</span></span>|<span data-ttu-id="5e449-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-155">Int32</span></span>|<span data-ttu-id="5e449-156">Число пользователей, имеющих 1 или другие устройства, который не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="5e449-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="5e449-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5e449-157">notApplicableUserCount</span></span>|<span data-ttu-id="5e449-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-158">Int32</span></span>|<span data-ttu-id="5e449-159">Число пользователей, которых устройства не все для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5e449-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="5e449-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="5e449-160">notInstalledUserCount</span></span>|<span data-ttu-id="5e449-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-161">Int32</span></span>|<span data-ttu-id="5e449-162">Число пользователей, которые имеют 1 или более устройства, на которых не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="5e449-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="5e449-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="5e449-163">pendingInstallUserCount</span></span>|<span data-ttu-id="5e449-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5e449-164">Int32</span></span>|<span data-ttu-id="5e449-165">Число пользователей, имеющих 1 или другие устройства, уведомлены для установки этого приложения и 0 устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="5e449-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="5e449-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e449-166">Response</span></span>
<span data-ttu-id="5e449-167">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5e449-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e449-168">Пример</span><span class="sxs-lookup"><span data-stu-id="5e449-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e449-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e449-169">Request</span></span>
<span data-ttu-id="5e449-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e449-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a><span data-ttu-id="5e449-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e449-171">Response</span></span>
<span data-ttu-id="5e449-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e449-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```





