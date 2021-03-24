---
title: Обновление mobileAppInstallSummary
description: Обновление свойств объекта mobileAppInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ecf2214cd2853112a23c4dab105d32a2e1a839e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143152"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="5b7eb-103">Обновление mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5b7eb-103">Update mobileAppInstallSummary</span></span>

<span data-ttu-id="5b7eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b7eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b7eb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b7eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b7eb-107">Обновление свойств объекта [mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)</span><span class="sxs-lookup"><span data-stu-id="5b7eb-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b7eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b7eb-108">Prerequisites</span></span>
<span data-ttu-id="5b7eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b7eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b7eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b7eb-111">Permission type</span></span>|<span data-ttu-id="5b7eb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b7eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b7eb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b7eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b7eb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b7eb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b7eb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b7eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b7eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-116">Not supported.</span></span>|
|<span data-ttu-id="5b7eb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b7eb-117">Application</span></span>|<span data-ttu-id="5b7eb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b7eb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b7eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b7eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="5b7eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b7eb-120">Request headers</span></span>
|<span data-ttu-id="5b7eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b7eb-121">Header</span></span>|<span data-ttu-id="5b7eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b7eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b7eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b7eb-123">Authorization</span></span>|<span data-ttu-id="5b7eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b7eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b7eb-125">Accept</span></span>|<span data-ttu-id="5b7eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b7eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b7eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b7eb-127">Request body</span></span>
<span data-ttu-id="5b7eb-128">В теле запроса поставляем представление JSON для [объекта mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)</span><span class="sxs-lookup"><span data-stu-id="5b7eb-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="5b7eb-129">В следующей таблице показаны свойства, необходимые при создании [mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)</span><span class="sxs-lookup"><span data-stu-id="5b7eb-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="5b7eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b7eb-130">Property</span></span>|<span data-ttu-id="5b7eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b7eb-131">Type</span></span>|<span data-ttu-id="5b7eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b7eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b7eb-133">id</span><span class="sxs-lookup"><span data-stu-id="5b7eb-133">id</span></span>|<span data-ttu-id="5b7eb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5b7eb-134">String</span></span>|<span data-ttu-id="5b7eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-135">Key of the entity.</span></span>|
|<span data-ttu-id="5b7eb-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-136">installedDeviceCount</span></span>|<span data-ttu-id="5b7eb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-137">Int32</span></span>|<span data-ttu-id="5b7eb-138">Количество устройств, успешно установленных в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="5b7eb-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-139">failedDeviceCount</span></span>|<span data-ttu-id="5b7eb-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-140">Int32</span></span>|<span data-ttu-id="5b7eb-141">Количество устройств, которые не смогли установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="5b7eb-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="5b7eb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-143">Int32</span></span>|<span data-ttu-id="5b7eb-144">Количество устройств, которые не применимы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="5b7eb-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="5b7eb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-146">Int32</span></span>|<span data-ttu-id="5b7eb-147">Количество устройств, на которые не установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="5b7eb-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="5b7eb-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-149">Int32</span></span>|<span data-ttu-id="5b7eb-150">Количество устройств, которые были уведомлены об установке этого приложения.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="5b7eb-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-151">installedUserCount</span></span>|<span data-ttu-id="5b7eb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-152">Int32</span></span>|<span data-ttu-id="5b7eb-153">Число пользователей, устройства которых успешно установили это приложение.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="5b7eb-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-154">failedUserCount</span></span>|<span data-ttu-id="5b7eb-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-155">Int32</span></span>|<span data-ttu-id="5b7eb-156">Число пользователей, у них есть 1 или более устройств, которые не смогли установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="5b7eb-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-157">notApplicableUserCount</span></span>|<span data-ttu-id="5b7eb-158">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-158">Int32</span></span>|<span data-ttu-id="5b7eb-159">Число пользователей, устройства которых не были применимы к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="5b7eb-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-160">notInstalledUserCount</span></span>|<span data-ttu-id="5b7eb-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-161">Int32</span></span>|<span data-ttu-id="5b7eb-162">Число пользователей с 1 или более устройствами, которые не установили это приложение.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="5b7eb-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="5b7eb-163">pendingInstallUserCount</span></span>|<span data-ttu-id="5b7eb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5b7eb-164">Int32</span></span>|<span data-ttu-id="5b7eb-165">Число пользователей с 1 или более устройствами, которые были уведомлены об установке этого приложения, и имеют 0 устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="5b7eb-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b7eb-166">Response</span></span>
<span data-ttu-id="5b7eb-167">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b7eb-168">Пример</span><span class="sxs-lookup"><span data-stu-id="5b7eb-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b7eb-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b7eb-169">Request</span></span>
<span data-ttu-id="5b7eb-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b7eb-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b7eb-171">Response</span></span>
<span data-ttu-id="5b7eb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b7eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




