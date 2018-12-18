---
title: Обновление mobileAppInstallSummary
description: Обновление свойства объекта mobileAppInstallSummary.
author: tfitzmac
ms.openlocfilehash: 94dc7fa5023d26de91b4d64efda27332dd51de63
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315640"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="50819-103">Обновление mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="50819-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="50819-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50819-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50819-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50819-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50819-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50819-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50819-107">Обновление свойства объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="50819-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50819-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50819-108">Prerequisites</span></span>
<span data-ttu-id="50819-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50819-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50819-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50819-111">Permission type</span></span>|<span data-ttu-id="50819-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50819-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50819-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50819-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50819-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50819-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50819-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50819-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50819-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50819-116">Not supported.</span></span>|
|<span data-ttu-id="50819-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50819-117">Application</span></span>|<span data-ttu-id="50819-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50819-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50819-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50819-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="50819-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50819-120">Request headers</span></span>
|<span data-ttu-id="50819-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50819-121">Header</span></span>|<span data-ttu-id="50819-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50819-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50819-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50819-123">Authorization</span></span>|<span data-ttu-id="50819-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="50819-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50819-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50819-125">Accept</span></span>|<span data-ttu-id="50819-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50819-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50819-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50819-127">Request body</span></span>
<span data-ttu-id="50819-128">В тексте запроса укажите представление JSON для объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="50819-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="50819-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="50819-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="50819-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50819-130">Property</span></span>|<span data-ttu-id="50819-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50819-131">Type</span></span>|<span data-ttu-id="50819-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50819-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50819-133">id</span><span class="sxs-lookup"><span data-stu-id="50819-133">id</span></span>|<span data-ttu-id="50819-134">Строка</span><span class="sxs-lookup"><span data-stu-id="50819-134">String</span></span>|<span data-ttu-id="50819-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50819-135">Key of the entity.</span></span>|
|<span data-ttu-id="50819-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50819-136">installedDeviceCount</span></span>|<span data-ttu-id="50819-137">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-137">Int32</span></span>|<span data-ttu-id="50819-138">Количество устройств, которые были успешно установлены этого приложения.</span><span class="sxs-lookup"><span data-stu-id="50819-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="50819-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50819-139">failedDeviceCount</span></span>|<span data-ttu-id="50819-140">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-140">Int32</span></span>|<span data-ttu-id="50819-141">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="50819-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="50819-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50819-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="50819-143">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-143">Int32</span></span>|<span data-ttu-id="50819-144">Количество устройств, которые не применимы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="50819-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="50819-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50819-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="50819-146">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-146">Int32</span></span>|<span data-ttu-id="50819-147">Количество устройств, для которого не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="50819-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="50819-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="50819-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="50819-149">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-149">Int32</span></span>|<span data-ttu-id="50819-150">Количество устройств, которые были уведомлены для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="50819-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="50819-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="50819-151">installedUserCount</span></span>|<span data-ttu-id="50819-152">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-152">Int32</span></span>|<span data-ttu-id="50819-153">Число пользователей, чьи устройств успешно для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="50819-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="50819-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="50819-154">failedUserCount</span></span>|<span data-ttu-id="50819-155">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-155">Int32</span></span>|<span data-ttu-id="50819-156">Число пользователей, имеющих 1 или другие устройства, который не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="50819-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="50819-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="50819-157">notApplicableUserCount</span></span>|<span data-ttu-id="50819-158">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-158">Int32</span></span>|<span data-ttu-id="50819-159">Число пользователей, которых устройства не все для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="50819-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="50819-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="50819-160">notInstalledUserCount</span></span>|<span data-ttu-id="50819-161">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-161">Int32</span></span>|<span data-ttu-id="50819-162">Число пользователей, которые имеют 1 или более устройства, на которых не установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="50819-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="50819-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="50819-163">pendingInstallUserCount</span></span>|<span data-ttu-id="50819-164">Int32</span><span class="sxs-lookup"><span data-stu-id="50819-164">Int32</span></span>|<span data-ttu-id="50819-165">Число пользователей, имеющих 1 или другие устройства, уведомлены для установки этого приложения и 0 устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="50819-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="50819-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="50819-166">Response</span></span>
<span data-ttu-id="50819-167">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="50819-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50819-168">Пример</span><span class="sxs-lookup"><span data-stu-id="50819-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="50819-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="50819-169">Request</span></span>
<span data-ttu-id="50819-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50819-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50819-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="50819-171">Response</span></span>
<span data-ttu-id="50819-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="50819-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





