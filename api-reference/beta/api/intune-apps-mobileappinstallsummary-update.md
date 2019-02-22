---
title: Обновление Мобилеаппинсталлсуммари
description: Обновление свойств объекта Мобилеаппинсталлсуммари.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6065083d5ceb5892a95a6b12bc99657eca7d3eeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152957"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="53c75-103">Обновление Мобилеаппинсталлсуммари</span><span class="sxs-lookup"><span data-stu-id="53c75-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="53c75-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53c75-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53c75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53c75-106">Обновление свойств объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="53c75-106">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53c75-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53c75-107">Prerequisites</span></span>
<span data-ttu-id="53c75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="53c75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53c75-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53c75-110">Permission type</span></span>|<span data-ttu-id="53c75-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53c75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53c75-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53c75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53c75-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c75-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53c75-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53c75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53c75-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c75-115">Not supported.</span></span>|
|<span data-ttu-id="53c75-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53c75-116">Application</span></span>|<span data-ttu-id="53c75-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c75-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53c75-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53c75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="53c75-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53c75-119">Request headers</span></span>
|<span data-ttu-id="53c75-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53c75-120">Header</span></span>|<span data-ttu-id="53c75-121">Значение</span><span class="sxs-lookup"><span data-stu-id="53c75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53c75-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53c75-122">Authorization</span></span>|<span data-ttu-id="53c75-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="53c75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53c75-124">Accept</span><span class="sxs-lookup"><span data-stu-id="53c75-124">Accept</span></span>|<span data-ttu-id="53c75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53c75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53c75-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53c75-126">Request body</span></span>
<span data-ttu-id="53c75-127">В тексте запроса добавьте представление объекта [Мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53c75-127">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="53c75-128">В следующей таблице приведены свойства, необходимые при создании [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="53c75-128">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="53c75-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="53c75-129">Property</span></span>|<span data-ttu-id="53c75-130">Тип</span><span class="sxs-lookup"><span data-stu-id="53c75-130">Type</span></span>|<span data-ttu-id="53c75-131">Описание</span><span class="sxs-lookup"><span data-stu-id="53c75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53c75-132">id</span><span class="sxs-lookup"><span data-stu-id="53c75-132">id</span></span>|<span data-ttu-id="53c75-133">String</span><span class="sxs-lookup"><span data-stu-id="53c75-133">String</span></span>|<span data-ttu-id="53c75-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53c75-134">Key of the entity.</span></span>|
|<span data-ttu-id="53c75-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53c75-135">installedDeviceCount</span></span>|<span data-ttu-id="53c75-136">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-136">Int32</span></span>|<span data-ttu-id="53c75-137">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="53c75-137">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="53c75-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53c75-138">failedDeviceCount</span></span>|<span data-ttu-id="53c75-139">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-139">Int32</span></span>|<span data-ttu-id="53c75-140">Количество устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="53c75-140">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="53c75-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53c75-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="53c75-142">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-142">Int32</span></span>|<span data-ttu-id="53c75-143">Количество устройств, неприменимых к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="53c75-143">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="53c75-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53c75-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="53c75-145">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-145">Int32</span></span>|<span data-ttu-id="53c75-146">Количество устройств, на которых не установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="53c75-146">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="53c75-147">Пендингинсталлдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="53c75-147">pendingInstallDeviceCount</span></span>|<span data-ttu-id="53c75-148">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-148">Int32</span></span>|<span data-ttu-id="53c75-149">Количество устройств, которые были уведомлены об установке этого приложения.</span><span class="sxs-lookup"><span data-stu-id="53c75-149">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="53c75-150">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="53c75-150">installedUserCount</span></span>|<span data-ttu-id="53c75-151">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-151">Int32</span></span>|<span data-ttu-id="53c75-152">Количество пользователей, чьи устройства успешно выполнили установку этого приложения.</span><span class="sxs-lookup"><span data-stu-id="53c75-152">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="53c75-153">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="53c75-153">failedUserCount</span></span>|<span data-ttu-id="53c75-154">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-154">Int32</span></span>|<span data-ttu-id="53c75-155">Количество пользователей с 1 или больше устройств, которые не удалось установить это приложение.</span><span class="sxs-lookup"><span data-stu-id="53c75-155">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="53c75-156">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="53c75-156">notApplicableUserCount</span></span>|<span data-ttu-id="53c75-157">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-157">Int32</span></span>|<span data-ttu-id="53c75-158">Количество пользователей, чьи устройства были неприменимы к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="53c75-158">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="53c75-159">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="53c75-159">notInstalledUserCount</span></span>|<span data-ttu-id="53c75-160">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-160">Int32</span></span>|<span data-ttu-id="53c75-161">Количество пользователей с 1 или больше устройств, которые не установили это приложение.</span><span class="sxs-lookup"><span data-stu-id="53c75-161">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="53c75-162">Пендингинсталлусеркаунт</span><span class="sxs-lookup"><span data-stu-id="53c75-162">pendingInstallUserCount</span></span>|<span data-ttu-id="53c75-163">Int32</span><span class="sxs-lookup"><span data-stu-id="53c75-163">Int32</span></span>|<span data-ttu-id="53c75-164">Количество пользователей с 1 или больше устройств, которые были уведомлены об установке этого приложения и имеют 0 устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="53c75-164">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="53c75-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c75-165">Response</span></span>
<span data-ttu-id="53c75-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53c75-166">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c75-167">Пример</span><span class="sxs-lookup"><span data-stu-id="53c75-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="53c75-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c75-168">Request</span></span>
<span data-ttu-id="53c75-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c75-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53c75-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c75-170">Response</span></span>
<span data-ttu-id="53c75-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53c75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




