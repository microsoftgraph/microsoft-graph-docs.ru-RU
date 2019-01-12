---
title: Создание mobileAppInstallStatus
description: Создание нового объекта mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2425ee773068eea2446b19534f907f48a43fe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970768"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="22ae4-103">Создание mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="22ae4-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="22ae4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22ae4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22ae4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22ae4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22ae4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="22ae4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22ae4-107">Создание нового объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="22ae4-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22ae4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22ae4-108">Prerequisites</span></span>
<span data-ttu-id="22ae4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22ae4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ae4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22ae4-111">Permission type</span></span>|<span data-ttu-id="22ae4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22ae4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22ae4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22ae4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22ae4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22ae4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22ae4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22ae4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22ae4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22ae4-116">Not supported.</span></span>|
|<span data-ttu-id="22ae4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22ae4-117">Application</span></span>|<span data-ttu-id="22ae4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22ae4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22ae4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22ae4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="22ae4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22ae4-120">Request headers</span></span>
|<span data-ttu-id="22ae4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22ae4-121">Header</span></span>|<span data-ttu-id="22ae4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22ae4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22ae4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22ae4-123">Authorization</span></span>|<span data-ttu-id="22ae4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="22ae4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22ae4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22ae4-125">Accept</span></span>|<span data-ttu-id="22ae4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22ae4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22ae4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22ae4-127">Request body</span></span>
<span data-ttu-id="22ae4-128">В тексте запроса укажите представление JSON для объекта mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="22ae4-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="22ae4-129">В следующей таблице показаны свойства, которые необходимы для создания mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="22ae4-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="22ae4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="22ae4-130">Property</span></span>|<span data-ttu-id="22ae4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="22ae4-131">Type</span></span>|<span data-ttu-id="22ae4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="22ae4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ae4-133">id</span><span class="sxs-lookup"><span data-stu-id="22ae4-133">id</span></span>|<span data-ttu-id="22ae4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="22ae4-134">String</span></span>|<span data-ttu-id="22ae4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="22ae4-135">Key of the entity.</span></span>|
|<span data-ttu-id="22ae4-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="22ae4-136">deviceName</span></span>|<span data-ttu-id="22ae4-137">String</span><span class="sxs-lookup"><span data-stu-id="22ae4-137">String</span></span>|<span data-ttu-id="22ae4-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="22ae4-138">Device name</span></span>|
|<span data-ttu-id="22ae4-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="22ae4-139">deviceId</span></span>|<span data-ttu-id="22ae4-140">String</span><span class="sxs-lookup"><span data-stu-id="22ae4-140">String</span></span>|<span data-ttu-id="22ae4-141">Идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="22ae4-141">Device ID</span></span>|
|<span data-ttu-id="22ae4-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="22ae4-142">lastSyncDateTime</span></span>|<span data-ttu-id="22ae4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ae4-143">DateTimeOffset</span></span>|<span data-ttu-id="22ae4-144">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="22ae4-144">Last sync date time</span></span>|
|<span data-ttu-id="22ae4-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="22ae4-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="22ae4-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="22ae4-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="22ae4-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="22ae4-147">The install state of the app.</span></span> <span data-ttu-id="22ae4-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="22ae4-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="22ae4-149">installState</span><span class="sxs-lookup"><span data-stu-id="22ae4-149">installState</span></span>|[<span data-ttu-id="22ae4-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="22ae4-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="22ae4-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="22ae4-151">The install state of the app.</span></span> <span data-ttu-id="22ae4-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="22ae4-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="22ae4-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="22ae4-153">installStateDetail</span></span>|[<span data-ttu-id="22ae4-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="22ae4-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="22ae4-155">Сведений о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="22ae4-155">The install state detail of the app.</span></span> <span data-ttu-id="22ae4-156">Возможные значения: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="22ae4-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="22ae4-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="22ae4-157">errorCode</span></span>|<span data-ttu-id="22ae4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="22ae4-158">Int32</span></span>|<span data-ttu-id="22ae4-159">Сообщение об ошибке примеры кода для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="22ae4-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="22ae4-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="22ae4-160">osVersion</span></span>|<span data-ttu-id="22ae4-161">String</span><span class="sxs-lookup"><span data-stu-id="22ae4-161">String</span></span>|<span data-ttu-id="22ae4-162">Версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="22ae4-162">OS Version</span></span>|
|<span data-ttu-id="22ae4-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="22ae4-163">osDescription</span></span>|<span data-ttu-id="22ae4-164">String</span><span class="sxs-lookup"><span data-stu-id="22ae4-164">String</span></span>|<span data-ttu-id="22ae4-165">Описание операционная система</span><span class="sxs-lookup"><span data-stu-id="22ae4-165">OS Description</span></span>|
|<span data-ttu-id="22ae4-166">userName</span><span class="sxs-lookup"><span data-stu-id="22ae4-166">userName</span></span>|<span data-ttu-id="22ae4-167">String</span><span class="sxs-lookup"><span data-stu-id="22ae4-167">String</span></span>|<span data-ttu-id="22ae4-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="22ae4-168">Device User Name</span></span>|
|<span data-ttu-id="22ae4-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="22ae4-169">userPrincipalName</span></span>|<span data-ttu-id="22ae4-170">Строка</span><span class="sxs-lookup"><span data-stu-id="22ae4-170">String</span></span>|<span data-ttu-id="22ae4-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="22ae4-171">User Principal Name</span></span>|
|<span data-ttu-id="22ae4-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="22ae4-172">displayVersion</span></span>|<span data-ttu-id="22ae4-173">Строка</span><span class="sxs-lookup"><span data-stu-id="22ae4-173">String</span></span>|<span data-ttu-id="22ae4-174">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="22ae4-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="22ae4-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="22ae4-175">Response</span></span>
<span data-ttu-id="22ae4-176">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22ae4-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22ae4-177">Пример</span><span class="sxs-lookup"><span data-stu-id="22ae4-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="22ae4-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="22ae4-178">Request</span></span>
<span data-ttu-id="22ae4-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22ae4-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="22ae4-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="22ae4-180">Response</span></span>
<span data-ttu-id="22ae4-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="22ae4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```





