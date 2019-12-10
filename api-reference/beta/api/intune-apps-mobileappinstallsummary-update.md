---
title: Обновление Мобилеаппинсталлсуммари
description: Обновление свойств объекта Мобилеаппинсталлсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6e68e11ffca04ce890aa93bb23b484f8a9295816
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935010"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="eb5ad-103">Обновление Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="eb5ad-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="eb5ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb5ad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb5ad-106">Обновление свойств объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="eb5ad-106">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb5ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eb5ad-107">Prerequisites</span></span>
<span data-ttu-id="eb5ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb5ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb5ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb5ad-110">Permission type</span></span>|<span data-ttu-id="eb5ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb5ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb5ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb5ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb5ad-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb5ad-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eb5ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb5ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb5ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-115">Not supported.</span></span>|
|<span data-ttu-id="eb5ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb5ad-116">Application</span></span>|<span data-ttu-id="eb5ad-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb5ad-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb5ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb5ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="eb5ad-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eb5ad-119">Request headers</span></span>
|<span data-ttu-id="eb5ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb5ad-120">Header</span></span>|<span data-ttu-id="eb5ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eb5ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb5ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb5ad-122">Authorization</span></span>|<span data-ttu-id="eb5ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb5ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eb5ad-124">Accept</span></span>|<span data-ttu-id="eb5ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb5ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb5ad-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb5ad-126">Request body</span></span>
<span data-ttu-id="eb5ad-127">В тексте запроса добавьте представление объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-127">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="eb5ad-128">В следующей таблице приведены свойства, необходимые при создании [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="eb5ad-128">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="eb5ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb5ad-129">Property</span></span>|<span data-ttu-id="eb5ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eb5ad-130">Type</span></span>|<span data-ttu-id="eb5ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eb5ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb5ad-132">id</span><span class="sxs-lookup"><span data-stu-id="eb5ad-132">id</span></span>|<span data-ttu-id="eb5ad-133">Строка</span><span class="sxs-lookup"><span data-stu-id="eb5ad-133">String</span></span>|<span data-ttu-id="eb5ad-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-134">Key of the entity.</span></span>|
|<span data-ttu-id="eb5ad-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-135">installedDeviceCount</span></span>|<span data-ttu-id="eb5ad-136">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-136">Int32</span></span>|<span data-ttu-id="eb5ad-137">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-137">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="eb5ad-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-138">failedDeviceCount</span></span>|<span data-ttu-id="eb5ad-139">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-139">Int32</span></span>|<span data-ttu-id="eb5ad-140">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-140">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="eb5ad-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="eb5ad-142">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-142">Int32</span></span>|<span data-ttu-id="eb5ad-143">Количество устройств, неприменимых к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-143">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="eb5ad-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="eb5ad-145">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-145">Int32</span></span>|<span data-ttu-id="eb5ad-146">Количество устройств, на которых не установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-146">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="eb5ad-147">пендингинсталлдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="eb5ad-147">pendingInstallDeviceCount</span></span>|<span data-ttu-id="eb5ad-148">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-148">Int32</span></span>|<span data-ttu-id="eb5ad-149">Количество устройств, которые были уведомлены об установке этого приложения.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-149">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="eb5ad-150">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-150">installedUserCount</span></span>|<span data-ttu-id="eb5ad-151">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-151">Int32</span></span>|<span data-ttu-id="eb5ad-152">Количество пользователей, чьи устройства успешно выполнили установку этого приложения.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-152">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="eb5ad-153">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-153">failedUserCount</span></span>|<span data-ttu-id="eb5ad-154">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-154">Int32</span></span>|<span data-ttu-id="eb5ad-155">Количество пользователей с 1 или больше устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-155">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="eb5ad-156">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-156">notApplicableUserCount</span></span>|<span data-ttu-id="eb5ad-157">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-157">Int32</span></span>|<span data-ttu-id="eb5ad-158">Количество пользователей, чьи устройства были неприменимы к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-158">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="eb5ad-159">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="eb5ad-159">notInstalledUserCount</span></span>|<span data-ttu-id="eb5ad-160">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-160">Int32</span></span>|<span data-ttu-id="eb5ad-161">Количество пользователей с 1 или больше устройств, которые не установили это приложение.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-161">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="eb5ad-162">пендингинсталлусеркаунт</span><span class="sxs-lookup"><span data-stu-id="eb5ad-162">pendingInstallUserCount</span></span>|<span data-ttu-id="eb5ad-163">Int32</span><span class="sxs-lookup"><span data-stu-id="eb5ad-163">Int32</span></span>|<span data-ttu-id="eb5ad-164">Количество пользователей с 1 или больше устройств, которые были уведомлены об установке этого приложения и имеют 0 устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-164">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="eb5ad-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb5ad-165">Response</span></span>
<span data-ttu-id="eb5ad-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-166">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb5ad-167">Пример</span><span class="sxs-lookup"><span data-stu-id="eb5ad-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb5ad-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb5ad-168">Request</span></span>
<span data-ttu-id="eb5ad-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb5ad-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb5ad-170">Response</span></span>
<span data-ttu-id="eb5ad-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb5ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





