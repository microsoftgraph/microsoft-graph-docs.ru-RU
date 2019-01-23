---
title: Обновление mobileAppInstallSummary
description: Обновление свойства объекта mobileAppInstallSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1975e8dae02876f6d083279e814f5199530aa1ab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413299"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="fc2f0-103">Обновление mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="fc2f0-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="fc2f0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc2f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc2f0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc2f0-107">Обновление свойства объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="fc2f0-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc2f0-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fc2f0-108">Prerequisites</span></span>
<span data-ttu-id="fc2f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc2f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fc2f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc2f0-111">Permission type</span></span>|<span data-ttu-id="fc2f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc2f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc2f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc2f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc2f0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc2f0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc2f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc2f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc2f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-116">Not supported.</span></span>|
|<span data-ttu-id="fc2f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc2f0-117">Application</span></span>|<span data-ttu-id="fc2f0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc2f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc2f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="fc2f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc2f0-120">Request headers</span></span>
|<span data-ttu-id="fc2f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc2f0-121">Header</span></span>|<span data-ttu-id="fc2f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc2f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc2f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc2f0-123">Authorization</span></span>|<span data-ttu-id="fc2f0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fc2f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc2f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc2f0-125">Accept</span></span>|<span data-ttu-id="fc2f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc2f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc2f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc2f0-127">Request body</span></span>
<span data-ttu-id="fc2f0-128">В тексте запроса укажите представление JSON для объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="fc2f0-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="fc2f0-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="fc2f0-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="fc2f0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc2f0-130">Property</span></span>|<span data-ttu-id="fc2f0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fc2f0-131">Type</span></span>|<span data-ttu-id="fc2f0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fc2f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2f0-133">id</span><span class="sxs-lookup"><span data-stu-id="fc2f0-133">id</span></span>|<span data-ttu-id="fc2f0-134">String</span><span class="sxs-lookup"><span data-stu-id="fc2f0-134">String</span></span>|<span data-ttu-id="fc2f0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-135">Key of the entity.</span></span>|
|<span data-ttu-id="fc2f0-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-136">installedDeviceCount</span></span>|<span data-ttu-id="fc2f0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-137">Int32</span></span>|<span data-ttu-id="fc2f0-138">Количество устройств, которые были успешно установлены этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="fc2f0-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-139">failedDeviceCount</span></span>|<span data-ttu-id="fc2f0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-140">Int32</span></span>|<span data-ttu-id="fc2f0-141">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="fc2f0-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="fc2f0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-143">Int32</span></span>|<span data-ttu-id="fc2f0-144">Количество устройств, которые не применимы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="fc2f0-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="fc2f0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-146">Int32</span></span>|<span data-ttu-id="fc2f0-147">Количество устройств, для которого не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="fc2f0-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="fc2f0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-149">Int32</span></span>|<span data-ttu-id="fc2f0-150">Количество устройств, которые были уведомлены для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="fc2f0-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-151">installedUserCount</span></span>|<span data-ttu-id="fc2f0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-152">Int32</span></span>|<span data-ttu-id="fc2f0-153">Число пользователей, чьи устройств успешно для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="fc2f0-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-154">failedUserCount</span></span>|<span data-ttu-id="fc2f0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-155">Int32</span></span>|<span data-ttu-id="fc2f0-156">Число пользователей, имеющих 1 или другие устройства, который не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="fc2f0-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-157">notApplicableUserCount</span></span>|<span data-ttu-id="fc2f0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-158">Int32</span></span>|<span data-ttu-id="fc2f0-159">Число пользователей, которых устройства не все для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="fc2f0-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-160">notInstalledUserCount</span></span>|<span data-ttu-id="fc2f0-161">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-161">Int32</span></span>|<span data-ttu-id="fc2f0-162">Число пользователей, которые имеют 1 или более устройства, на которых не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="fc2f0-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="fc2f0-163">pendingInstallUserCount</span></span>|<span data-ttu-id="fc2f0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f0-164">Int32</span></span>|<span data-ttu-id="fc2f0-165">Число пользователей, имеющих 1 или другие устройства, уведомлены для установки этого приложения и 0 устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="fc2f0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc2f0-166">Response</span></span>
<span data-ttu-id="fc2f0-167">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc2f0-168">Пример</span><span class="sxs-lookup"><span data-stu-id="fc2f0-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc2f0-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc2f0-169">Request</span></span>
<span data-ttu-id="fc2f0-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
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

### <a name="response"></a><span data-ttu-id="fc2f0-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc2f0-171">Response</span></span>
<span data-ttu-id="fc2f0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fc2f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




