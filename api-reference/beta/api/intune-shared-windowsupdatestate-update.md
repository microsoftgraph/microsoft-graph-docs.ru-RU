---
title: Обновление windowsUpdateState
description: Обновление свойств объекта WindowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6505707c957ad890d07c9d418512b41e09ff5109
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443799"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="8803d-103">Обновление windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="8803d-103">Update windowsUpdateState</span></span>

<span data-ttu-id="8803d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8803d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8803d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8803d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8803d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8803d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8803d-107">Обновление свойств объекта [WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="8803d-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8803d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8803d-108">Prerequisites</span></span>
<span data-ttu-id="8803d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8803d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8803d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8803d-111">Permission type</span></span>|<span data-ttu-id="8803d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8803d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8803d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8803d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8803d-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8803d-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8803d-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8803d-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8803d-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="8803d-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8803d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8803d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8803d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8803d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8803d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8803d-119">Not supported.</span></span>|
|<span data-ttu-id="8803d-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="8803d-120">Application</span></span>||
| <span data-ttu-id="8803d-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8803d-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8803d-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8803d-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8803d-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="8803d-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8803d-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8803d-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8803d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8803d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8803d-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8803d-126">Request headers</span></span>
|<span data-ttu-id="8803d-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8803d-127">Header</span></span>|<span data-ttu-id="8803d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8803d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8803d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8803d-129">Authorization</span></span>|<span data-ttu-id="8803d-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8803d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8803d-131">Accept</span><span class="sxs-lookup"><span data-stu-id="8803d-131">Accept</span></span>|<span data-ttu-id="8803d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8803d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8803d-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8803d-133">Request body</span></span>
<span data-ttu-id="8803d-134">В теле запроса укажи представление JSON для [объекта WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="8803d-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="8803d-135">В следующей таблице показаны свойства, необходимые при создании [windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="8803d-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="8803d-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="8803d-136">Property</span></span>|<span data-ttu-id="8803d-137">Тип</span><span class="sxs-lookup"><span data-stu-id="8803d-137">Type</span></span>|<span data-ttu-id="8803d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8803d-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8803d-139">id</span><span class="sxs-lookup"><span data-stu-id="8803d-139">id</span></span>|<span data-ttu-id="8803d-140">String</span><span class="sxs-lookup"><span data-stu-id="8803d-140">String</span></span>|<span data-ttu-id="8803d-141">Это Id объекта.</span><span class="sxs-lookup"><span data-stu-id="8803d-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="8803d-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="8803d-142">deviceId</span></span>|<span data-ttu-id="8803d-143">String</span><span class="sxs-lookup"><span data-stu-id="8803d-143">String</span></span>|<span data-ttu-id="8803d-144">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="8803d-144">The id of the device.</span></span>|
|<span data-ttu-id="8803d-145">userId</span><span class="sxs-lookup"><span data-stu-id="8803d-145">userId</span></span>|<span data-ttu-id="8803d-146">String</span><span class="sxs-lookup"><span data-stu-id="8803d-146">String</span></span>|<span data-ttu-id="8803d-147">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="8803d-147">The id of the user.</span></span>|
|<span data-ttu-id="8803d-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8803d-148">deviceDisplayName</span></span>|<span data-ttu-id="8803d-149">String</span><span class="sxs-lookup"><span data-stu-id="8803d-149">String</span></span>|<span data-ttu-id="8803d-150">Имя отображения устройства.</span><span class="sxs-lookup"><span data-stu-id="8803d-150">Device display name.</span></span>|
|<span data-ttu-id="8803d-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8803d-151">userPrincipalName</span></span>|<span data-ttu-id="8803d-152">String</span><span class="sxs-lookup"><span data-stu-id="8803d-152">String</span></span>|<span data-ttu-id="8803d-153">Имя основного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8803d-153">User principal name.</span></span>|
|<span data-ttu-id="8803d-154">status</span><span class="sxs-lookup"><span data-stu-id="8803d-154">status</span></span>|[<span data-ttu-id="8803d-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="8803d-155">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="8803d-156">Состояние udpate Windows.</span><span class="sxs-lookup"><span data-stu-id="8803d-156">Windows udpate status.</span></span> <span data-ttu-id="8803d-157">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8803d-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="8803d-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="8803d-158">qualityUpdateVersion</span></span>|<span data-ttu-id="8803d-159">String</span><span class="sxs-lookup"><span data-stu-id="8803d-159">String</span></span>|<span data-ttu-id="8803d-160">Версия обновления качества устройства.</span><span class="sxs-lookup"><span data-stu-id="8803d-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="8803d-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="8803d-161">featureUpdateVersion</span></span>|<span data-ttu-id="8803d-162">String</span><span class="sxs-lookup"><span data-stu-id="8803d-162">String</span></span>|<span data-ttu-id="8803d-163">Текущая версия обновления функций устройства.</span><span class="sxs-lookup"><span data-stu-id="8803d-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="8803d-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8803d-164">lastScanDateTime</span></span>|<span data-ttu-id="8803d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8803d-165">DateTimeOffset</span></span>|<span data-ttu-id="8803d-166">Время даты успешного сканирования агентом обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="8803d-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="8803d-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8803d-167">lastSyncDateTime</span></span>|<span data-ttu-id="8803d-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8803d-168">DateTimeOffset</span></span>|<span data-ttu-id="8803d-169">Последний раз, когда устройство синхронизируется с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8803d-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="8803d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="8803d-170">Response</span></span>
<span data-ttu-id="8803d-171">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsUpdateState](../resources/intune-shared-windowsupdatestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8803d-171">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8803d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="8803d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="8803d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="8803d-173">Request</span></span>
<span data-ttu-id="8803d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8803d-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8803d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="8803d-175">Response</span></span>
<span data-ttu-id="8803d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8803d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "3d92af00-af00-3d92-00af-923d00af923d",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```







