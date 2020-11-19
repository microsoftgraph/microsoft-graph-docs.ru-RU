---
title: Обновление Мобилеаппинсталлсуммари
description: Обновление свойств объекта Мобилеаппинсталлсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efe0816dc084dd0ff4f8c95e9a4b3aac8f5a6097
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248317"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="93c45-103">Обновление Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="93c45-103">Update mobileAppInstallSummary</span></span>

<span data-ttu-id="93c45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93c45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93c45-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93c45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93c45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93c45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93c45-107">Обновление свойств объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="93c45-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93c45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93c45-108">Prerequisites</span></span>
<span data-ttu-id="93c45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93c45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93c45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93c45-111">Permission type</span></span>|<span data-ttu-id="93c45-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93c45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93c45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93c45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93c45-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c45-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93c45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93c45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93c45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93c45-116">Not supported.</span></span>|
|<span data-ttu-id="93c45-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="93c45-117">Application</span></span>|<span data-ttu-id="93c45-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c45-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93c45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93c45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="93c45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93c45-120">Request headers</span></span>
|<span data-ttu-id="93c45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93c45-121">Header</span></span>|<span data-ttu-id="93c45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="93c45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93c45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93c45-123">Authorization</span></span>|<span data-ttu-id="93c45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93c45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93c45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93c45-125">Accept</span></span>|<span data-ttu-id="93c45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93c45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93c45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93c45-127">Request body</span></span>
<span data-ttu-id="93c45-128">В тексте запроса добавьте представление объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93c45-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="93c45-129">В следующей таблице приведены свойства, необходимые при создании [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="93c45-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="93c45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="93c45-130">Property</span></span>|<span data-ttu-id="93c45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="93c45-131">Type</span></span>|<span data-ttu-id="93c45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="93c45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93c45-133">id</span><span class="sxs-lookup"><span data-stu-id="93c45-133">id</span></span>|<span data-ttu-id="93c45-134">String</span><span class="sxs-lookup"><span data-stu-id="93c45-134">String</span></span>|<span data-ttu-id="93c45-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="93c45-135">Key of the entity.</span></span>|
|<span data-ttu-id="93c45-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93c45-136">installedDeviceCount</span></span>|<span data-ttu-id="93c45-137">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-137">Int32</span></span>|<span data-ttu-id="93c45-138">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="93c45-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="93c45-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93c45-139">failedDeviceCount</span></span>|<span data-ttu-id="93c45-140">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-140">Int32</span></span>|<span data-ttu-id="93c45-141">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="93c45-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="93c45-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93c45-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="93c45-143">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-143">Int32</span></span>|<span data-ttu-id="93c45-144">Количество устройств, неприменимых к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="93c45-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="93c45-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93c45-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="93c45-146">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-146">Int32</span></span>|<span data-ttu-id="93c45-147">Количество устройств, на которых не установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="93c45-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="93c45-148">пендингинсталлдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="93c45-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="93c45-149">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-149">Int32</span></span>|<span data-ttu-id="93c45-150">Количество устройств, которые были уведомлены об установке этого приложения.</span><span class="sxs-lookup"><span data-stu-id="93c45-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="93c45-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="93c45-151">installedUserCount</span></span>|<span data-ttu-id="93c45-152">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-152">Int32</span></span>|<span data-ttu-id="93c45-153">Количество пользователей, чьи устройства успешно выполнили установку этого приложения.</span><span class="sxs-lookup"><span data-stu-id="93c45-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="93c45-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="93c45-154">failedUserCount</span></span>|<span data-ttu-id="93c45-155">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-155">Int32</span></span>|<span data-ttu-id="93c45-156">Количество пользователей с 1 или больше устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="93c45-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="93c45-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="93c45-157">notApplicableUserCount</span></span>|<span data-ttu-id="93c45-158">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-158">Int32</span></span>|<span data-ttu-id="93c45-159">Количество пользователей, чьи устройства были неприменимы к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="93c45-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="93c45-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="93c45-160">notInstalledUserCount</span></span>|<span data-ttu-id="93c45-161">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-161">Int32</span></span>|<span data-ttu-id="93c45-162">Количество пользователей с 1 или больше устройств, которые не установили это приложение.</span><span class="sxs-lookup"><span data-stu-id="93c45-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="93c45-163">пендингинсталлусеркаунт</span><span class="sxs-lookup"><span data-stu-id="93c45-163">pendingInstallUserCount</span></span>|<span data-ttu-id="93c45-164">Int32</span><span class="sxs-lookup"><span data-stu-id="93c45-164">Int32</span></span>|<span data-ttu-id="93c45-165">Количество пользователей с 1 или больше устройств, которые были уведомлены об установке этого приложения и имеют 0 устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="93c45-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="93c45-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="93c45-166">Response</span></span>
<span data-ttu-id="93c45-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93c45-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93c45-168">Пример</span><span class="sxs-lookup"><span data-stu-id="93c45-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="93c45-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="93c45-169">Request</span></span>
<span data-ttu-id="93c45-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93c45-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93c45-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="93c45-171">Response</span></span>
<span data-ttu-id="93c45-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93c45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




